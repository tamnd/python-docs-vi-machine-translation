# Quality

## Invariants, recounted

862 machine-written entries in the corpus. Every one of them passed the invariants when it was accepted, so anything below is a rule that was tightened afterwards or an entry something else edited.

| Rule | Failing | Pass rate |
| --- | ---: | ---: |
| `P01` | 372 | 56.84% |
| `P02` | 372 | 56.84% |

## Refusals

1 runs, 27 batches, 414 entries accepted, 26 refused, 0 batches refused whole, 6 entries out of rungs. Acceptance rate 94.09%.

| Rule | Refusals | Share |
| --- | ---: | ---: |
| `P05` | 24 | 75.0% |
| `P08` | 4 | 12.5% |
| `P01` | 2 | 6.2% |
| `P02` | 2 | 6.2% |

| Rung | Refusals |
| --- | ---: |
| 1 | 21 |
| 2 | 7 |
| 3 | 4 |

## Glossary adherence

639 terms against 2,030 translated entries. 277 misses over 91 terms.

| Written by | Entries | Misses | Misses per entry | Terms |
| --- | ---: | ---: | ---: | ---: |
| human | 1,168 | 246 | 0.21 | 85 |
| machine | 862 | 31 | 0.04 | 18 |

| Term | Misses |
| --- | ---: |
| type | 39 |
| list | 30 |
| sequence | 22 |
| dictionary | 10 |
| newline | 8 |
| iterator | 6 |
| key | 6 |
| class | 5 |
| namespace | 5 |
| positional arguments | 5 |
| slice | 5 |
| callable | 4 |
| file | 4 |
| local namespace | 4 |
| mapping | 4 |
| package | 4 |
| attribute | 3 |
| base classes | 3 |
| data types | 3 |
| different types | 3 |

## Dead entries

6 jobs out of rungs, 29 entries between them.

| Job | File | Entries | Reason |
| --- | --- | ---: | --- |
| `5d1f704cdc373879` | tutorial/datastructures.po | 2 | 1 entries refused, rung 3 already climbed |
| `6bb4383c38465217` | tutorial/modules.po | 1 | 1 entries refused, out of rungs |
| `b07df84f784f7a08` | tutorial/classes.po | 23 | 1 entries refused, rung 2 already climbed |
| `d0e0b58b8358d0f5` | tutorial/inputoutput.po | 1 | 1 entries refused, out of rungs |
| `f95296a5ce7f88a6` | tutorial/inputoutput.po | 1 | 1 entries refused, out of rungs |
| `fa8a9850ecbb91fb` | tutorial/modules.po | 1 | 1 entries refused, out of rungs |

## Routes

27 calls over 0.3 hours.

| Route | Calls | Share |
| --- | ---: | ---: |
| server3 | 27 | 100.0% |
