# Audit

Fail. 41 checks, 13 failing, 1,492 findings.

## Structure

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `S01` | yes | 0 | the pin's counts match a recount |
| `S02` | yes | 0 | no msgid was edited |
| `S03` | yes | 0 | entry count, order and msgctxt match upstream |
| `S04` | yes | 0 | no unmarked machine translation |
| `S05` | yes | 0 | format flags preserved |
| `S06` | yes | 0 | obsolete entries preserved |
| `S07` | yes | 0 | no msgid_plural |
| `S08` | yes | 0 | apply --check is byte-identical |

## Placeholders

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `P01` | yes | 27 | protected spans survive |
| `P02` | yes | 0 | no placeholder marker survives |
| `P03` | yes | 27 | role targets unchanged |
| `P04` | yes | 0 | surrounding whitespace matches |
| `P05` | yes | 1 | format specifiers match |
| `P06` | yes | 0 | link targets unchanged |
| `P07` | yes | 31 | code entries copied exactly |
| `P08` | yes | 0 | no fence or horizontal rule |

## Glossary

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `G01` | no | 0 | the glossary is self-consistent |
| `G02` | no | 196 | glossary renderings are used |
| `G03` | no | 81 | kept terms stayed in English |
| `G04` | no | 148 | no untranslated glossary term |
| `G05` | no | 0 | GLOSSARY.md matches the YAML |
| `G06` | no | 0 | no entry is on a stale glossary |

## Language

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `L01` | yes | 9 | the translation is in Vietnamese |
| `L02` | yes | 144 | no entry is the English verbatim |
| `L03` | yes | 0 | no narration |
| `L04` | yes | 0 | no English sentence copied through |
| `L05` | no | 3 | second-person pronoun policy |
| `L06` | no | 0 | headings are noun phrases |
| `L07` | no | 816 | no cut-down model wrote an entry |
| `L08` | no | 5 | sentence counts are close |

## Availability

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `A01` | yes | 0 | the coverage report is current |
| `A02` | yes | 0 | every dead job is accounted for |
| `A03` | yes | 0 | the memory and the catalogs agree |
| `A04` | no | 4 | dead entries per file below a ceiling |
| `A05` | no | 0 | heavily refused batches are named |

## Hygiene

| Check | Hard | Findings | What it checks |
| --- | --- | --- | --- |
| `H01` | yes | 0 | no compiled catalog is tracked |
| `H02` | yes | 0 | no oversized file is tracked |
| `H03` | yes | 0 | no secret-shaped string is tracked |
| `H04` | yes | 0 | text files are well formed |
| `H05` | yes | 0 | no working-copy directory is tracked |
| `H06` | yes | 0 | the README agrees with the coverage report |

## Findings

### `P01` protected spans survive

- bugs.po:38  ':ref:`contribute <contributing-to-python>`' appears 0 time(s), the source has 1
- bugs.po:220  ' <https://bugzilla.mozilla.org/page.cgi?id=bug-writing.html>`_' appears 0 time(s), the source has 1
- library/functions.po:439  ':ref:`truth testing procedure <truth>`' appears 0 time(s), the source has 1
- library/functions.po:784  ':ref:`filter <warning-filter>`' appears 0 time(s), the source has 1
- library/functions.po:1343  ':term:`free (closure) variables <closure variable>`' appears 0 time(s), the source has 1
- library/functions.po:1817  ':ref:`integer literal in code <integers>`' appears 0 time(s), the source has 1
- library/functions.po:1866  ':ref:`integer string conversion length limitation <int_max_str_digits>`' appears 0 time(s), the source has 1
- library/functions.po:1887  ':term:`virtual <abstract base class>`' appears 0 time(s), the source has 1
- library/functions.po:1912  ':term:`virtual <abstract base class>`' appears 0 time(s), the source has 1
- library/functions.po:2511  ':ref:`non-inheritable <fd_inheritance>`' appears 0 time(s), the source has 1
- library/functions.po:2575  ':ref:`auditing event <auditing>`' appears 0 time(s), the source has 1
- library/functions.po:3086  ':ref:`private name mangling <private-name-mangling>`' appears 0 time(s), the source has 1
- library/functions.po:3209  ':ref:`slicing syntax <slicings>`' appears 0 time(s), the source has 1
- library/functions.po:3281  ':ref:`rich comparisons <comparisons>`' appears 0 time(s), the source has 1
- library/functions.po:3455  ':term:`method resolution order`' appears 0 time(s), the source has 1
- library/functions.po:3606  ':mod:`pickleable <pickle>`' appears 0 time(s), the source has 1
- library/functions.po:3606  ':mod:`copyable <copy>`' appears 0 time(s), the source has 1
- library/functions.po:3659  ':ref:`Documentation on attributes and methods on classes <class-attrs-and-methods>`' appears 0 time(s), the source has 1
- library/io.po:862  ':ref:`non-inheritable <fd_inheritance>`' appears 0 time(s), the source has 1
- library/os.po:1167  ':ref:`auditing event <auditing>`' appears 0 time(s), the source has 1
- and 7 more, not printed

### `P03` role targets unchanged

- bugs.po:38  :ref:`contribute <contributing-to-python>` is not in the translation
- library/functions.po:439  :ref:`truth testing procedure <truth>` is not in the translation
- library/functions.po:678  :attr:`~function.__annotations__` is not in the translation
- library/functions.po:784  :ref:`filter <warning-filter>` is not in the translation
- library/functions.po:1343  :term:`free (closure) variables <closure variable>` is not in the translation
- library/functions.po:1535  :class:`frozenset` is not in the translation
- library/functions.po:1817  :ref:`integer literal in code <integers>` is not in the translation
- library/functions.po:1866  :ref:`integer string conversion length limitation <int_max_str_digits>` is not in the translation
- library/functions.po:1887  :term:`virtual <abstract base class>` is not in the translation
- library/functions.po:1912  :term:`virtual <abstract base class>` is not in the translation
- library/functions.po:2511  :ref:`non-inheritable <fd_inheritance>` is not in the translation
- library/functions.po:2575  :ref:`auditing event <auditing>` is not in the translation
- library/functions.po:3086  :ref:`private name mangling <private-name-mangling>` is not in the translation
- library/functions.po:3209  :ref:`slicing syntax <slicings>` is not in the translation
- library/functions.po:3281  :ref:`rich comparisons <comparisons>` is not in the translation
- library/functions.po:3455  :term:`method resolution order` is not in the translation
- library/functions.po:3606  :mod:`copyable <copy>` is not in the translation
- library/functions.po:3606  :mod:`pickleable <pickle>` is not in the translation
- library/functions.po:3659  :ref:`Documentation on attributes and methods on classes <class-attrs-and-methods>` is not in the translation
- library/io.po:862  :ref:`non-inheritable <fd_inheritance>` is not in the translation
- and 7 more, not printed

### `P05` format specifiers match

- tutorial/introduction.po:146  source has ['% o'], translation has []

### `P07` code entries copied exactly

- tutorial/errors.po:755  literal_block entry differs from its source
- tutorial/interpreter.po:198  literal_block entry differs from its source
- tutorial/interpreter.po:222  doctest entry differs from its source
- tutorial/introduction.po:73  literal_block entry differs from its source
- tutorial/introduction.po:109  doctest entry differs from its source
- tutorial/introduction.po:146  doctest entry differs from its source
- tutorial/introduction.po:172  doctest entry differs from its source
- tutorial/introduction.po:208  doctest entry differs from its source
- tutorial/introduction.po:298  doctest entry differs from its source
- tutorial/introduction.po:320  doctest entry differs from its source
- tutorial/introduction.po:354  doctest entry differs from its source
- tutorial/introduction.po:381  doctest entry differs from its source
- tutorial/introduction.po:417  doctest entry differs from its source
- tutorial/introduction.po:447  doctest entry differs from its source
- tutorial/introduction.po:474  doctest entry differs from its source
- tutorial/introduction.po:491  doctest entry differs from its source
- tutorial/introduction.po:538  doctest entry differs from its source
- tutorial/introduction.po:555  doctest entry differs from its source
- tutorial/introduction.po:582  doctest entry differs from its source
- tutorial/introduction.po:601  doctest entry differs from its source
- and 11 more, not printed

### `G02` glossary renderings are used

- about.po:28  'generator' should render as 'trình sinh'
- bugs.po:175  'comment' should render as 'chú thích'
- bugs.po:186  'comment' should render as 'chú thích'
- library/functions.po:312  'floating-point number' should render as 'số dấu phẩy động'
- library/functions.po:439  'argument' should render as 'đối số'
- library/functions.po:502  'sequence' should render as 'dãy'
- library/functions.po:502  'mutable' should render as 'có thể thay đổi'
- library/functions.po:521  'encoding' should render as 'mã hóa'
- library/functions.po:558  'immutable' should render as 'bất biến'
- library/functions.po:558  'sequence' should render as 'dãy'
- library/functions.po:575  'bytes objects' should render as 'các đối tượng bytes'
- library/functions.po:626  'instance method' should render as 'phương thức thể hiện'
- library/functions.po:718  'sequence' should render as 'dãy'
- library/functions.po:798  'python code' should render as 'mã Python'
- library/functions.po:814  'newline' should render as 'ký tự xuống dòng'
- library/functions.po:834  'newline' should render as 'ký tự xuống dòng'
- library/functions.po:904  'trailing whitespace' should render as 'khoảng trắng ở cuối'
- library/functions.po:1058  'different types' should render as 'các kiểu khác nhau'
- library/functions.po:1073  'class object' should render as 'đối tượng lớp'
- library/functions.po:1092  'metaclass' should render as 'siêu lớp'
- and 176 more, not printed

### `G03` kept terms stayed in English

- bugs.po:88  'list' is kept in English and did not survive
- bugs.po:120  'list' is kept in English and did not survive
- bugs.po:158  'list' is kept in English and did not survive
- library/asyncio-sync.po:80  'Lock' is kept in English and did not survive
- library/functions.po:457  'type' is kept in English and did not survive
- library/functions.po:502  'type' is kept in English and did not survive
- library/functions.po:584  'callable' is kept in English and did not survive
- library/functions.po:944  'type' is kept in English and did not survive
- library/functions.po:971  'type' is kept in English and did not survive
- library/functions.po:1023  'list' is kept in English and did not survive
- library/functions.po:1032  'list' is kept in English and did not survive
- library/functions.po:1045  'list' is kept in English and did not survive
- library/functions.po:1066  'list' is kept in English and did not survive
- library/functions.po:1073  'list' is kept in English and did not survive
- library/functions.po:1073  'type' is kept in English and did not survive
- library/functions.po:1080  'list' is kept in English and did not survive
- library/functions.po:1089  'list' is kept in English and did not survive
- library/functions.po:1092  'list' is kept in English and did not survive
- library/functions.po:1485  'type' is kept in English and did not survive
- library/functions.po:1495  'type' is kept in English and did not survive
- and 61 more, not printed

### `G04` no untranslated glossary term

- bugs.po:175  'comment' is still in English, and renders as 'chú thích'
- bugs.po:186  'comment' is still in English, and renders as 'chú thích'
- library/functions.po:521  'encoding' is still in English, and renders as 'mã hóa'
- library/functions.po:1092  'metaclass' is still in English, and renders as 'siêu lớp'
- library/functions.po:1159  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1162  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1184  'Condition' is still in English, and renders as 'Điều kiện'
- library/functions.po:1184  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1269  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1354  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1363  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1375  'function' is still in English, and renders as 'hàm'
- library/functions.po:1387  'generator' is still in English, and renders as 'trình sinh'
- library/functions.po:1387  'function' is still in English, and renders as 'hàm'
- library/functions.po:1398  'function' is still in English, and renders as 'hàm'
- library/functions.po:1580  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1649  'namespace' is still in English, and renders as 'không gian tên'
- library/functions.po:1927  'iterator' is still in English, and renders as 'trình lặp'
- library/functions.po:1927  'sequence' is still in English, and renders as 'dãy'
- library/functions.po:1978  'dictionary' is still in English, and renders as 'từ điển'
- and 128 more, not printed

### `L01` the translation is in Vietnamese

- copyright.po:34  49 characters of prose with no Vietnamese diacritic
- copyright.po:37  89 characters of prose with no Vietnamese diacritic
- copyright.po:44  74 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:873  46 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1348  463 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1366  258 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1465  245 characters of prose with no Vietnamese diacritic
- tutorial/controlflow.po:1799  48 characters of prose with no Vietnamese diacritic
- whatsnew/3.10.po:1072  46 characters of prose with no Vietnamese diacritic

### `L02` no entry is the English verbatim

- bugs.po:93  identical to the English
- c-api/bytearray.po:107  identical to the English
- c-api/bytes.po:562  identical to the English
- c-api/capsule.po:199  identical to the English
- c-api/code.po:409  identical to the English
- c-api/complex.po:199  identical to the English
- c-api/concrete.po:76  identical to the English
- c-api/dict.po:727  identical to the English
- c-api/exceptions.po:1573  identical to the English
- c-api/file.po:175  identical to the English
- c-api/float.po:271  identical to the English
- c-api/function.po:240  identical to the English
- c-api/interp-lifecycle.po:1140  identical to the English
- c-api/interp-lifecycle.po:1143  identical to the English
- c-api/interp-lifecycle.po:1151  identical to the English
- c-api/intro.po:1516  identical to the English
- c-api/intro.po:1519  identical to the English
- c-api/intro.po:1581  identical to the English
- c-api/intro.po:1584  identical to the English
- c-api/intro.po:1592  identical to the English
- and 124 more, not printed

### `L05` second-person pronoun policy

- tutorial/appetite.po:188  'bạn' where the English does not address the reader
- tutorial/interpreter.po:114  'bạn' where the English does not address the reader
- tutorial/introduction.po:53  'bạn' where the English does not address the reader

### `L07` no cut-down model wrote an entry

- c-api/dict.po:304  written by gpt-5-6-mini
- c-api/exceptions.po:442  written by gpt-5-6-mini
- c-api/function.po:243  written by gpt-5-6-mini
- c-api/init_config.po:148  written by gpt-5-6-mini
- c-api/interp-lifecycle.po:1154  written by gpt-5-6-mini
- c-api/interp-lifecycle.po:1159  written by gpt-5-6-mini
- c-api/intro.po:26  written by gpt-5-6-mini
- c-api/intro.po:318  written by gpt-5-6-mini
- c-api/intro.po:1131  written by gpt-5-6-mini
- c-api/intro.po:1595  written by gpt-5-6-mini
- c-api/intro.po:1600  written by gpt-5-6-mini
- c-api/method.po:59  written by gpt-5-6-mini
- c-api/method.po:105  written by gpt-5-6-mini
- c-api/refcounting.po:124  written by gpt-5-6-mini
- c-api/threads.po:248  written by gpt-5-6-mini
- extending/extending.po:35  written by gpt-5-6-mini
- faq/library.po:632  written by gpt-5-6-mini
- faq/programming.po:2885  written by gpt-5-6-mini
- faq/programming.po:3348  written by gpt-5-6-mini
- glossary.po:939  written by gpt-5-6-mini
- and 796 more, not printed

### `L08` sentence counts are close

- tutorial/controlflow.po:1377  the English has 6 sentences, the translation has 4
- tutorial/datastructures.po:959  the English has 2 sentences, the translation has 4
- tutorial/datastructures.po:1001  the English has 3 sentences, the translation has 6
- tutorial/datastructures.po:1058  the English has 3 sentences, the translation has 6
- tutorial/introduction.po:128  the English has 4 sentences, the translation has 2

### `A04` dead entries per file below a ceiling

- tutorial/classes.po  23 of 154 entries dead, over the 1% ceiling
- tutorial/datastructures.po  2 of 139 entries dead, over the 1% ceiling
- tutorial/inputoutput.po  2 of 112 entries dead, over the 1% ceiling
- tutorial/modules.po  2 of 117 entries dead, over the 1% ceiling
