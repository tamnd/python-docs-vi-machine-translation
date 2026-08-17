# Audit

Fail. 41 checks, 19 failing, 3,109 findings.

## Structure

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `S01` | yes | 0 | the pin's counts match a recount |
| `S02` | yes | 28 | no msgid was edited |
| `S03` | yes | 228 | entry count, order and msgctxt match upstream |
| `S04` | yes | 367 | no unmarked machine translation |
| `S05` | yes | 0 | format flags preserved |
| `S06` | yes | 0 | obsolete entries preserved |
| `S07` | yes | 0 | no msgid_plural |
| `S08` | yes | 548 | apply --check is byte-identical |

## Placeholders

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `P01` | yes | 26 | protected spans survive |
| `P02` | yes | 0 | no placeholder marker survives |
| `P03` | yes | 26 | role targets unchanged |
| `P04` | yes | 46 | surrounding whitespace matches |
| `P05` | yes | 1 | format specifiers match |
| `P06` | yes | 0 | link targets unchanged |
| `P07` | yes | 48 | code entries copied exactly |
| `P08` | yes | 0 | no fence or horizontal rule |

## Glossary

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `G01` | no | 0 | the glossary is self-consistent |
| `G02` | no | 327 | glossary renderings are used |
| `G03` | no | 122 | kept terms stayed in English |
| `G04` | no | 236 | no untranslated glossary term |
| `G05` | no | 0 | GLOSSARY.md matches the YAML |
| `G06` | no | 0 | no entry is on a stale glossary |

## Language

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `L01` | yes | 12 | the translation is in Vietnamese |
| `L02` | yes | 12 | no entry is the English verbatim |
| `L03` | yes | 0 | no narration |
| `L04` | yes | 0 | no English sentence copied through |
| `L05` | no | 4 | second-person pronoun policy |
| `L06` | no | 0 | headings are noun phrases |
| `L07` | no | 306 | no cut-down model wrote an entry |
| `L08` | no | 2 | sentence counts are close |

## Availability

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `A01` | yes | 0 | the coverage report is current |
| `A02` | yes | 0 | every dead job is accounted for |
| `A03` | yes | 388 | the memory and the catalogs agree |
| `A04` | no | 0 | dead entries per file below a ceiling |
| `A05` | no | 0 | heavily refused batches are named |

## Hygiene

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `H01` | yes | 0 | no compiled catalog is tracked |
| `H02` | yes | 0 | no oversized file is tracked |
| `H03` | yes | 0 | no secret-shaped string is tracked |
| `H04` | yes | 382 | text files are well formed |
| `H05` | yes | 0 | no working-copy directory is tracked |
| `H06` | yes | 0 | the README agrees with the coverage report |

## Findings

### `S02` no msgid was edited

- about.po:75  msgid is not in the upstream pin, so it was edited here
- bugs.po:113  msgid is not in the upstream pin, so it was edited here
- bugs.po:119  msgid is not in the upstream pin, so it was edited here
- library/functions.po:1883  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2407  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2420  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2427  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2434  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2441  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2454  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2463  msgid is not in the upstream pin, so it was edited here
- library/functions.po:2470  msgid is not in the upstream pin, so it was edited here
- library/functions.po:3000  msgid is not in the upstream pin, so it was edited here
- tutorial/datastructures.po:722  msgid is not in the upstream pin, so it was edited here
- tutorial/datastructures.po:949  msgid is not in the upstream pin, so it was edited here
- tutorial/datastructures.po:957  msgid is not in the upstream pin, so it was edited here
- tutorial/interpreter.po:42  msgid is not in the upstream pin, so it was edited here
- tutorial/interpreter.po:196  msgid is not in the upstream pin, so it was edited here
- tutorial/stdlib.po:36  msgid is not in the upstream pin, so it was edited here
- tutorial/stdlib2.po:21  msgid is not in the upstream pin, so it was edited here
- and 8 more, not printed

### `S03` entry count, order and msgctxt match upstream

- about.po:75  entry is not the upstream entry at this position
- bugs.po:113  entry is not the upstream entry at this position
- c-api/allocation.po:22  entry is not the upstream entry at this position
- c-api/apiabiversion.po  60 entries here against 62 upstream
- c-api/arg.po  205 entries here against 208 upstream
- c-api/buffer.po:378  entry is not the upstream entry at this position
- c-api/bytes.po  77 entries here against 119 upstream
- c-api/code.po:262  entry is not the upstream entry at this position
- c-api/complex.po  35 entries here against 37 upstream
- c-api/conversion.po:165  entry is not the upstream entry at this position
- c-api/datetime.po  65 entries here against 67 upstream
- c-api/descriptor.po  17 entries here against 35 upstream
- c-api/dict.po  108 entries here against 123 upstream
- c-api/exceptions.po  269 entries here against 286 upstream
- c-api/extension-modules.po  50 entries here against 69 upstream
- c-api/file.po:25  entry is not the upstream entry at this position
- c-api/float.po  58 entries here against 57 upstream
- c-api/frame.po  51 entries here against 50 upstream
- c-api/function.po  43 entries here against 44 upstream
- c-api/gcsupport.po  68 entries here against 107 upstream
- and 208 more, not printed

### `S04` no unmarked machine translation

- about.po:75  translated, not fuzzy, and not human in the memory
- bugs.po:113  translated, not fuzzy, and not human in the memory
- bugs.po:119  translated, not fuzzy, and not human in the memory
- library/functions.po:1883  translated, not fuzzy, and not human in the memory
- library/functions.po:2407  translated, not fuzzy, and not human in the memory
- library/functions.po:2420  translated, not fuzzy, and not human in the memory
- library/functions.po:2427  translated, not fuzzy, and not human in the memory
- library/functions.po:2434  translated, not fuzzy, and not human in the memory
- library/functions.po:2441  translated, not fuzzy, and not human in the memory
- library/functions.po:2454  translated, not fuzzy, and not human in the memory
- library/functions.po:2463  translated, not fuzzy, and not human in the memory
- library/functions.po:2470  translated, not fuzzy, and not human in the memory
- library/functions.po:3000  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:22  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:26  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:36  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:40  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:48  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:62  translated, not fuzzy, and not human in the memory
- tutorial/errors.po:74  translated, not fuzzy, and not human in the memory
- and 347 more, not printed

### `S08` apply --check is byte-identical

- about.po  committed bytes differ from what apply would write
- bugs.po  committed bytes differ from what apply would write
- c-api/abstract.po  committed bytes differ from what apply would write
- c-api/allocation.po  committed bytes differ from what apply would write
- c-api/apiabiversion.po  committed bytes differ from what apply would write
- c-api/arg.po  committed bytes differ from what apply would write
- c-api/bool.po  committed bytes differ from what apply would write
- c-api/buffer.po  committed bytes differ from what apply would write
- c-api/bytearray.po  committed bytes differ from what apply would write
- c-api/bytes.po  committed bytes differ from what apply would write
- c-api/call.po  committed bytes differ from what apply would write
- c-api/capsule.po  committed bytes differ from what apply would write
- c-api/cell.po  committed bytes differ from what apply would write
- c-api/code.po  committed bytes differ from what apply would write
- c-api/codec.po  committed bytes differ from what apply would write
- c-api/complex.po  committed bytes differ from what apply would write
- c-api/concrete.po  committed bytes differ from what apply would write
- c-api/contextvars.po  committed bytes differ from what apply would write
- c-api/conversion.po  committed bytes differ from what apply would write
- c-api/coro.po  committed bytes differ from what apply would write
- and 528 more, not printed

### `P01` protected spans survive

- bugs.po:38  ':ref:`contribute <contributing-to-python>`' appears 0 time(s), the source has 1
- bugs.po:219  ' <https://bugzilla.mozilla.org/page.cgi?id=bug-writing.html>`_' appears 0 time(s), the source has 1
- library/functions.po:434  ':ref:`truth testing procedure <truth>`' appears 0 time(s), the source has 1
- library/functions.po:1319  ':term:`free (closure) variables <closure variable>`' appears 0 time(s), the source has 1
- library/functions.po:1789  ':ref:`integer literal in code <integers>`' appears 0 time(s), the source has 1
- library/functions.po:1838  ':ref:`integer string conversion length limitation <int_max_str_digits>`' appears 0 time(s), the source has 1
- library/functions.po:1858  ':term:`virtual <abstract base class>`' appears 0 time(s), the source has 1
- library/functions.po:1883  ':term:`virtual <abstract base class>`' appears 0 time(s), the source has 1
- library/functions.po:2545  ':ref:`non-inheritable <fd_inheritance>`' appears 0 time(s), the source has 1
- library/functions.po:2609  ':ref:`auditing event <auditing>`' appears 0 time(s), the source has 1
- library/functions.po:3120  ':ref:`private name mangling <private-name-mangling>`' appears 0 time(s), the source has 1
- library/functions.po:3138  ':ref:`slicing syntax <slicings>`' appears 0 time(s), the source has 1
- library/functions.po:3211  ':ref:`rich comparisons <comparisons>`' appears 0 time(s), the source has 1
- library/functions.po:3381  ':term:`method resolution order`' appears 0 time(s), the source has 1
- library/functions.po:3533  ':mod:`pickleable <pickle>`' appears 0 time(s), the source has 1
- library/functions.po:3533  ':mod:`copyable <copy>`' appears 0 time(s), the source has 1
- library/functions.po:3587  ':ref:`Documentation on attributes and methods on classes <class-attrs-and-methods>`' appears 0 time(s), the source has 1
- tutorial/controlflow.po:2097  ':ref:`Function annotations <function>`' appears 0 time(s), the source has 1
- tutorial/floatingpoint.po:557  ':dfn:`Representation error`' appears 0 time(s), the source has 1
- tutorial/interactive.po:43  ':ref:`automatically enabled <rlcompleter-config>`' appears 0 time(s), the source has 1
- and 6 more, not printed

### `P03` role targets unchanged

- bugs.po:38  :ref:`contribute <contributing-to-python>` is not in the translation
- library/functions.po:434  :ref:`truth testing procedure <truth>` is not in the translation
- library/functions.po:671  :attr:`~function.__annotations__` is not in the translation
- library/functions.po:1319  :term:`free (closure) variables <closure variable>` is not in the translation
- library/functions.po:1511  :class:`frozenset` is not in the translation
- library/functions.po:1789  :ref:`integer literal in code <integers>` is not in the translation
- library/functions.po:1838  :ref:`integer string conversion length limitation <int_max_str_digits>` is not in the translation
- library/functions.po:1858  :term:`virtual <abstract base class>` is not in the translation
- library/functions.po:1883  :term:`virtual <abstract base class>` is not in the translation
- library/functions.po:2545  :ref:`non-inheritable <fd_inheritance>` is not in the translation
- library/functions.po:2609  :ref:`auditing event <auditing>` is not in the translation
- library/functions.po:3120  :ref:`private name mangling <private-name-mangling>` is not in the translation
- library/functions.po:3138  :ref:`slicing syntax <slicings>` is not in the translation
- library/functions.po:3211  :ref:`rich comparisons <comparisons>` is not in the translation
- library/functions.po:3381  :term:`method resolution order` is not in the translation
- library/functions.po:3533  :mod:`copyable <copy>` is not in the translation
- library/functions.po:3533  :mod:`pickleable <pickle>` is not in the translation
- library/functions.po:3587  :ref:`Documentation on attributes and methods on classes <class-attrs-and-methods>` is not in the translation
- tutorial/controlflow.po:2097  :ref:`Function annotations <function>` is not in the translation
- tutorial/floatingpoint.po:557  :dfn:`Representation error` is not in the translation
- and 6 more, not printed

### `P04` surrounding whitespace matches

- extending/extending.po:1747  leading whitespace '' became ' '
- extending/newtypes_tutorial.po:1871  leading whitespace '' became ' '
- library/abc.po:420  leading whitespace '' became ' '
- library/collections.abc.po:375  leading whitespace '' became ' '
- library/configparser.po:1557  leading whitespace '' became ' '
- library/csv.po:680  leading whitespace '' became ' '
- library/datetime.po:3531  leading whitespace '' became ' '
- library/doctest.po:2267  leading whitespace '' became ' '
- library/email.contentmanager.po:248  leading whitespace '' became ' '
- library/email.encoders.po:102  leading whitespace '' became ' '
- library/email.examples.po:462  leading whitespace '' became ' '
- library/email.generator.po:281  leading whitespace '' became ' '
- library/email.headerregistry.po:560  leading whitespace '' became ' '
- library/email.message.po:769  leading whitespace '' became ' '
- library/email.policy.po:694  leading whitespace '' became ' '
- library/email.utils.po:236  leading whitespace '' became ' '
- library/functions.po:1150  leading whitespace '' became ' '
- library/functions.po:3959  leading whitespace '' became ' '
- library/gettext.po:751  leading whitespace '' became ' '
- library/heapq.po:500  leading whitespace '' became ' '
- and 26 more, not printed

### `P05` format specifiers match

- tutorial/introduction.po:146  source has ['% o'], translation has []

### `P07` code entries copied exactly

- tutorial/datastructures.po:138  doctest entry differs from its source
- tutorial/datastructures.po:287  doctest entry differs from its source
- tutorial/datastructures.po:438  doctest entry differs from its source
- tutorial/datastructures.po:588  doctest entry differs from its source
- tutorial/datastructures.po:722  doctest entry differs from its source
- tutorial/datastructures.po:811  doctest entry differs from its source
- tutorial/datastructures.po:901  doctest entry differs from its source
- tutorial/errors.po:709  literal_block entry differs from its source
- tutorial/floatingpoint.po:213  doctest entry differs from its source
- tutorial/floatingpoint.po:511  doctest entry differs from its source
- tutorial/interpreter.po:218  doctest entry differs from its source
- tutorial/introduction.po:73  literal_block entry differs from its source
- tutorial/introduction.po:109  doctest entry differs from its source
- tutorial/introduction.po:146  doctest entry differs from its source
- tutorial/introduction.po:172  doctest entry differs from its source
- tutorial/introduction.po:208  doctest entry differs from its source
- tutorial/introduction.po:298  doctest entry differs from its source
- tutorial/introduction.po:320  doctest entry differs from its source
- tutorial/introduction.po:354  doctest entry differs from its source
- tutorial/introduction.po:381  doctest entry differs from its source
- and 28 more, not printed

### `G02` glossary renderings are used

- about.po:28  'generator' should render as 'trình sinh'
- about.po:75  'python standard library' should render as 'thư viện chuẩn Python'
- bugs.po:174  'comment' should render as 'chú thích'
- bugs.po:185  'comment' should render as 'chú thích'
- library/functions.po:309  'floating-point number' should render as 'số dấu phẩy động'
- library/functions.po:434  'argument' should render as 'đối số'
- library/functions.po:496  'sequence' should render as 'dãy'
- library/functions.po:496  'mutable' should render as 'có thể thay đổi'
- library/functions.po:515  'encoding' should render as 'mã hóa'
- library/functions.po:552  'immutable' should render as 'bất biến'
- library/functions.po:552  'sequence' should render as 'dãy'
- library/functions.po:569  'bytes objects' should render as 'các đối tượng bytes'
- library/functions.po:619  'instance method' should render as 'phương thức thể hiện'
- library/functions.po:628  'class' should render as 'lớp'
- library/functions.po:710  'sequence' should render as 'dãy'
- library/functions.po:782  'python code' should render as 'mã Python'
- library/functions.po:798  'newline' should render as 'ký tự xuống dòng'
- library/functions.po:818  'newline' should render as 'ký tự xuống dòng'
- library/functions.po:885  'trailing whitespace' should render as 'khoảng trắng ở cuối'
- library/functions.po:1037  'different types' should render as 'các kiểu khác nhau'
- and 307 more, not printed

### `G03` kept terms stayed in English

- about.po:75  'list' is kept in English and did not survive
- bugs.po:88  'list' is kept in English and did not survive
- bugs.po:119  'list' is kept in English and did not survive
- bugs.po:157  'list' is kept in English and did not survive
- library/asyncio-sync.po:68  'Lock' is kept in English and did not survive
- library/functions.po:452  'type' is kept in English and did not survive
- library/functions.po:496  'type' is kept in English and did not survive
- library/functions.po:578  'callable' is kept in English and did not survive
- library/functions.po:925  'type' is kept in English and did not survive
- library/functions.po:952  'type' is kept in English and did not survive
- library/functions.po:1002  'list' is kept in English and did not survive
- library/functions.po:1011  'list' is kept in English and did not survive
- library/functions.po:1024  'list' is kept in English and did not survive
- library/functions.po:1045  'list' is kept in English and did not survive
- library/functions.po:1052  'list' is kept in English and did not survive
- library/functions.po:1052  'type' is kept in English and did not survive
- library/functions.po:1059  'list' is kept in English and did not survive
- library/functions.po:1068  'list' is kept in English and did not survive
- library/functions.po:1071  'list' is kept in English and did not survive
- library/functions.po:1461  'type' is kept in English and did not survive
- and 102 more, not printed

### `G04` no untranslated glossary term

- bugs.po:174  'comment' is still in English, and renders as 'chú thích'
- bugs.po:185  'comment' is still in English, and renders as 'chú thích'
- library/functions.po:515  'encoding' is still in English, and renders as 'mã hóa'
- library/functions.po:628  'class' is still in English, and renders as 'lớp'
- library/functions.po:1071  'metaclass' is still in English, and renders as 'siêu lớp'
- library/functions.po:1138  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1141  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1163  'Condition' is still in English, and renders as 'Điều kiện'
- library/functions.po:1163  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1248  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1330  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1339  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1351  'function' is still in English, and renders as 'hàm'
- library/functions.po:1363  'generator' is still in English, and renders as 'trình sinh'
- library/functions.po:1363  'function' is still in English, and renders as 'hàm'
- library/functions.po:1374  'function' is still in English, and renders as 'hàm'
- library/functions.po:1555  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1622  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1883  'class' is still in English, and renders as 'lớp'
- library/functions.po:1899  'iterator' is still in English, and renders as 'trình lặp'
- and 216 more, not printed

### `L01` the translation is in Vietnamese

- copyright.po:34  49 characters of prose with no Vietnamese diacritic
- copyright.po:37  89 characters of prose with no Vietnamese diacritic
- copyright.po:44  74 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:873  46 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1349  463 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1373  258 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1475  245 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1812  48 characters of prose with no Vietnamese diacritic
- tutorial/datastructures.po:1486  264 characters of prose with no Vietnamese diacritic
- tutorial/errors.po:608  54 characters of prose with no Vietnamese diacritic
- tutorial/stdlib2.po:477  241 characters of prose with no Vietnamese diacritic
- tutorial/stdlib2.po:498  126 characters of prose with no Vietnamese diacritic

### `L02` no entry is the English verbatim

- bugs.po:93  identical to the English
- copyright.po:34  identical to the English
- copyright.po:37  identical to the English
- copyright.po:44  identical to the English
- tutorial/controlflow.po:873  identical to the English
- tutorial/controlflow.po:1349  identical to the English
- tutorial/controlflow.po:1373  identical to the English
- tutorial/controlflow.po:1475  identical to the English
- tutorial/controlflow.po:1812  identical to the English
- tutorial/datastructures.po:1486  identical to the English
- tutorial/stdlib2.po:477  identical to the English
- tutorial/stdlib2.po:498  identical to the English

### `L05` second-person pronoun policy

- tutorial/appetite.po:188  'bạn' where the English does not address the reader
- tutorial/datastructures.po:212  'bạn' where the English does not address the reader
- tutorial/interpreter.po:112  'bạn' where the English does not address the reader
- tutorial/introduction.po:53  'bạn' where the English does not address the reader

### `L07` no cut-down model wrote an entry

- tutorial/datastructures.po:24  written by gpt-5-6-mini
- tutorial/datastructures.po:28  written by gpt-5-6-mini
- tutorial/datastructures.po:36  written by gpt-5-6-mini
- tutorial/datastructures.po:40  written by gpt-5-6-mini
- tutorial/datastructures.po:48  written by gpt-5-6-mini
- tutorial/datastructures.po:52  written by gpt-5-6-mini
- tutorial/datastructures.po:60  written by gpt-5-6-mini
- tutorial/datastructures.po:70  written by gpt-5-6-mini
- tutorial/datastructures.po:78  written by gpt-5-6-mini
- tutorial/datastructures.po:90  written by gpt-5-6-mini
- tutorial/datastructures.po:94  written by gpt-5-6-mini
- tutorial/datastructures.po:102  written by gpt-5-6-mini
- tutorial/datastructures.po:114  written by gpt-5-6-mini
- tutorial/datastructures.po:118  written by gpt-5-6-mini
- tutorial/datastructures.po:126  written by gpt-5-6-mini
- tutorial/datastructures.po:130  written by gpt-5-6-mini
- tutorial/datastructures.po:134  written by gpt-5-6-mini
- tutorial/datastructures.po:182  written by gpt-5-6-mini
- tutorial/datastructures.po:194  written by gpt-5-6-mini
- tutorial/datastructures.po:208  written by gpt-5-6-mini
- and 286 more, not printed

### `L08` sentence counts are close

- tutorial/controlflow.po:1386  the English has 6 sentences, the translation has 4
- tutorial/introduction.po:128  the English has 4 sentences, the translation has 2

### `A03` the memory and the catalogs agree

- c-api/dict.po:333  the memory has a machine translation and the catalog is empty
- c-api/exceptions.po:518  the memory has a machine translation and the catalog is empty
- c-api/init_config.po:113  the memory has a machine translation and the catalog is empty
- c-api/intro.po:216  the memory has a machine translation and the catalog is empty
- c-api/method.po:63  the memory has a machine translation and the catalog is empty
- c-api/refcounting.po:151  the memory has a machine translation and the catalog is empty
- c-api/threads.po:280  the memory has a machine translation and the catalog is empty
- faq/library.po:642  the memory has a machine translation and the catalog is empty
- faq/programming.po:2722  the memory has a machine translation and the catalog is empty
- glossary.po:3091  the memory has a machine translation and the catalog is empty
- howto/gdb_helpers.po:418  the memory has a machine translation and the catalog is empty
- howto/isolating-extensions.po:807  the memory has a machine translation and the catalog is empty
- howto/sorting.po:541  the memory has a machine translation and the catalog is empty
- howto/urllib2.po:266  the memory has a machine translation and the catalog is empty
- library/argparse.po:3242  the memory has a machine translation and the catalog is empty
- library/ast.po:3240  the memory has a machine translation and the catalog is empty
- library/asyncio-llapi-index.po:396  the memory has a machine translation and the catalog is empty
- library/constants.po:163  the memory has a machine translation and the catalog is empty
- library/contextlib.po:399  the memory has a machine translation and the catalog is empty
- library/contextvars.po:165  the memory has a machine translation and the catalog is empty
- and 368 more, not printed

### `H04` text files are well formed

- c-api/abstract.po  ends in more than one newline
- c-api/allocation.po  ends in more than one newline
- c-api/apiabiversion.po  ends in more than one newline
- c-api/bool.po  ends in more than one newline
- c-api/buffer.po  ends in more than one newline
- c-api/bytearray.po  ends in more than one newline
- c-api/bytes.po  ends in more than one newline
- c-api/call.po  ends in more than one newline
- c-api/capsule.po  ends in more than one newline
- c-api/cell.po  ends in more than one newline
- c-api/code.po  ends in more than one newline
- c-api/codec.po  ends in more than one newline
- c-api/complex.po  ends in more than one newline
- c-api/concrete.po  ends in more than one newline
- c-api/contextvars.po  ends in more than one newline
- c-api/conversion.po  ends in more than one newline
- c-api/coro.po  ends in more than one newline
- c-api/curses.po  ends in more than one newline
- c-api/datetime.po  ends in more than one newline
- c-api/descriptor.po  ends in more than one newline
- and 362 more, not printed
