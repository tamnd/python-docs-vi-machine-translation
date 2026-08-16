# Retired scripts

Three ad-hoc scripts lived in `scripts/` and produced the first pass over `MACHINE/`.
They are kept here because they are the provenance of everything currently in that tree, not because anything still runs them.
Nothing in the repo imports them and no workflow calls them.

| file | what it did |
| --- | --- |
| `mt.py` | Translated one `.po` file at a time through deep-translator's Google backend, filling only empty `msgstr` and flagging every result fuzzy. |
| `mt_batch.py` | Packed many strings into one `translate_a/single` request with `QQZSEP` markers, falling back to one request per string when the marker count came back wrong. |
| `mt_machine.py` | Retranslated every `msgid` in `MACHINE/` regardless of existing `msgstr`, to get a pure machine snapshot for comparison. |

## Why they are retired

All three protect reST markup by substituting placeholder tokens, translating, and substituting back.
That is the right idea and it is where the replacement's segmentation rules came from, but the implementations drifted apart.
Each script grew its own copy of the pattern list, so a construct one of them protected another would hand to the translator as prose.

They also share three limits that no amount of patching fixes.
They have no terminology contract, so the same English term comes back rendered differently in different files.
They keep no record of which strings were touched by which run, so a bad pass cannot be found afterwards and undone.
And they translate against a moving upstream with nothing pinned, so a rerun months later silently mixes two source versions.

## What replaced them

The [python-docs-vi-translator](https://github.com/tamnd/python-docs-vi-translator) tool.
It pins the upstream commit with `pydocvi sync`, keeps one segmentation implementation in `pydocvi.segment` rather than three, and carries a reviewed glossary that every prompt cites and every audit checks against.

The command that actually writes translations lands in M5.
Until it does, `MACHINE/` is exactly what these scripts left behind, and it should be read as a starting point rather than as output anyone has reviewed.
