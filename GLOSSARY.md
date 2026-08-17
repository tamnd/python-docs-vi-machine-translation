# Glossary

Terminology and style rules for the Vietnamese translation. Read this
before touching a `.po` file, and update it whenever a judgment call
comes up during review.

The goal is not to be prescriptive for every word. It is to keep
consistent choices across hundreds of files and dozens of reviewers.
When in doubt, prefer what is already in here; if you disagree, open
a PR that updates the glossary and sweep the affected files.

## Style rules

### Pronoun

Drop the second-person pronoun where Vietnamese grammar allows it. Use
`bạn` only when the text directly addresses the reader in a way that
would feel incomplete without a pronoun (e.g. a call to action, a
tutorial instruction with an implied subject).

Examples:

- `msgid`: "You can create a list by..."
  `msgstr`: "Có thể tạo danh sách bằng..." (dropped pronoun, neutral)
  `msgstr`: "Bạn có thể tạo danh sách bằng..." (acceptable when the tone
  is explicitly addressing the reader)
- `msgid`: "If you find a bug..."
  `msgstr`: "Nếu bạn tìm thấy lỗi..." (keep `bạn`, it is a call to
  action)

Never use `anh`, `chị`, `em`, or other age/gender-specific pronouns.

### Imperative vs. noun form

Section headings and titles use noun form, not imperative. This matches
the Vietnamese convention for reference documentation.

- `msgid`: "Defining Functions"
  `msgstr`: "Định nghĩa hàm" (noun form)
  Avoid: "Hãy định nghĩa hàm" (imperative, too instructional)

Body text may use imperative when it is a direct instruction:

- `msgid`: "Run the command to see the output."
  `msgstr`: "Chạy lệnh để xem kết quả." (imperative is fine here)

### Sentence case

Headings use Vietnamese sentence case: first letter of the heading
capitalized, everything else lowercase unless it is a proper noun or a
code identifier.

- `msgid`: "Dealing with Bugs"
  `msgstr`: "Xử lý lỗi"
  Avoid: "Xử Lý Lỗi" (title case)

### Code, identifiers, file paths

Never translate. Keep them in backticks.

### reST directives

Preserve exactly. `:func:` / `:class:` / `:mod:` / `:ref:` and their
arguments stay identical. Word order in the Vietnamese sentence may
change around them.

### Quotes

Use Vietnamese guillemets `« »` only in prose that already uses them.
For the docs, follow upstream punctuation as-is: if `msgid` uses `"..."`
so does `msgstr`. Do not convert to typographic quotes (`“...”`).

### Numbers and units

Keep Arabic numerals. Do not spell out numbers that are digits in the
source. "32-bit" stays "32-bit".

## Terminology

### The term list

The table below is generated from `manifests/glossary.yaml` and it is the
part of this file a tool reads. Every row is quoted in the prompt for any
batch whose English contains the term, and `G02` fails an entry whose
Vietnamese is missing a rendering the prompt asked for. So a row here is a
contract rather than a suggestion, and a wrong row costs more than a
missing one: a wrong row fails translations that were correct, while a
missing one only leaves a term unenforced.

Do not edit the table by hand. Edit `manifests/glossary.yaml` and run
`pydocvi glossary bump`, which regenerates it. `G05` fails when the two
disagree.

<!-- generated: terms -->

Version 1. 639 terms, 52 of them kept in English.

| English | Vietnamese | Notes |
| --- | --- | --- |
| asynchronous generator iterator | trình lặp sinh bất đồng bộ |  |
| format() (built-in function) | format() (hàm tích hợp sẵn) |  |
| context management protocol | giao thức quản lý ngữ cảnh |  |
| Positional-Only Parameters | Tham số chỉ vị trí |  |
| multi-phase initialization | khởi tạo nhiều giai đoạn |  |
| current working directory | thư mục làm việc hiện hành |  |
| multiphase initialization | khởi tạo nhiều giai đoạn |  |
| str() (built-in function) | str() (hàm tích hợp sẵn) |  |
| synchronization primitive | nguyên thủy đồng bộ hóa |  |
| Arbitrary Argument Lists | Danh sách đối số tùy ý |  |
| Unpacking Argument Lists | Giải nén danh sách đối số |  |
| dictionary comprehension | `dictionary comprehension` (kept) |  |
| open() built-in function | hàm tích hợp sẵn open() |  |
| Default Argument Values | Giá trị đối số mặc định |  |
| backwards compatibility | tương thích ngược |  |
| concurrent modification | sửa đổi đồng thời |  |
| global interpreter lock | khóa trình thông dịch toàn cục |  |
| interactive interpreter | trình thông dịch tương tác |  |
| method resolution order | thứ tự phân giải phương thức |  |
| python standard library | thư viện chuẩn Python |  |
| Keyword-Only Arguments | Đối số chỉ từ khóa |  |
| asynchronous generator | trình sinh bất đồng bộ |  |
| backward compatibility | tương thích ngược |  |
| command line arguments | đối số dòng lệnh |  |
| command-line arguments | đối số dòng lệnh |  |
| command-line interface | giao diện dòng lệnh |  |
| cpython implementation | triển khai CPython |  |
| default implementation | triển khai mặc định |  |
| floating-point numbers | các số dấu phẩy động |  |
| implementation details | chi tiết triển khai |  |
| keyword-only parameter | tham số chỉ từ khóa |  |
| python implementations | các triển khai Python |  |
| python install manager | trình quản lý cài đặt Python |  |
| abstract base classes | lớp cơ sở trừu tượng |  |
| asynchronous iterable | đối tượng lặp bất đồng bộ |  |
| asynchronous iterator | trình lặp bất đồng bộ |  |
| attached thread state | trạng thái luồng được gắn |  |
| configuration options | tùy chọn cấu hình |  |
| convenience functions | hàm tiện ích |  |
| environment variables | các biến môi trường |  |
| exception information | thông tin ngoại lệ |  |
| floating-point number | số dấu phẩy động |  |
| generator expressions | biểu thức sinh |  |
| implementation detail | chi tiết triển khai |  |
| keyword-only argument | đối số chỉ từ khóa |  |
| logging configuration | cấu hình logging |  |
| multiple interpreters | nhiều trình thông dịch |  |
| python implementation | triển khai Python |  |
| python initialization | khởi tạo Python |  |
| string representation | biểu diễn chuỗi |  |
| Function Annotations | Chú thích hàm |  |
| Source Code Encoding | Mã hóa mã nguồn |  |
| command line options | các tùy chọn dòng lệnh |  |
| command-line options | các tùy chọn dòng lệnh |  |
| environment variable | biến môi trường |  |
| free-threaded builds | bản dựng free-threaded |  |
| generator expression | biểu thức sinh |  |
| interpreter shutdown | tắt trình thông dịch |  |
| multiple inheritance | đa kế thừa |  |
| non-ascii characters | ký tự không phải ASCII |  |
| positional arguments | các đối số vị trí |  |
| programming language | ngôn ngữ lập trình |  |
| python documentation | tài liệu Python |  |
| static type checkers | trình kiểm tra kiểu tĩnh |  |
| triple-quoted string | chuỗi ba dấu nháy |  |
| virtual environments | môi trường ảo |  |
| abstract base class | lớp cơ sở trừu tượng |  |
| command line option | tùy chọn dòng lệnh |  |
| command-line option | tùy chọn dòng lệnh |  |
| configuration files | các tệp cấu hình |  |
| current interpreter | trình thông dịch hiện tại |  |
| deprecation warning | cảnh báo ngừng dùng |  |
| free-threaded build | bản dựng free-threaded |  |
| function annotation | chú thích hàm |  |
| function definition | định nghĩa hàm |  |
| instance attributes | thuộc tính thể hiện |  |
| positional argument | đối số vị trí |  |
| provisional package | gói tạm thời |  |
| python installation | cài đặt Python |  |
| read-only attribute | thuộc tính chỉ đọc |  |
| regular expressions | các biểu thức chính quy |  |
| static type checker | trình kiểm tra kiểu tĩnh |  |
| text mode (default) | chế độ văn bản (mặc định) |  |
| trailing whitespace | khoảng trắng ở cuối |  |
| variable annotation | chú thích biến |  |
| virtual environment | môi trường ảo |  |
| Built-in Functions | Các hàm tích hợp sẵn |  |
| Lambda Expressions | Biểu thức lambda |  |
| Special parameters | Tham số đặc biệt |  |
| borrowed reference | tham chiếu mượn |  |
| calling convention | quy ước gọi |  |
| configuration file | tệp cấu hình |  |
| context management | quản lý ngữ cảnh |  |
| control characters | ký tự điều khiển |  |
| coroutine function | hàm coroutine |  |
| exception handling | xử lý ngoại lệ |  |
| exception instance | thể hiện ngoại lệ |  |
| garbage collection | thu gom rác |  |
| generator function | hàm sinh |  |
| generator iterator | trình lặp sinh |  |
| instance variables | biến thể hiện |  |
| list comprehension | `list comprehension` (kept) |  |
| namespace packages | gói không gian tên |  |
| optional arguments | các đối số tùy chọn |  |
| optional parameter | tham số tùy chọn |  |
| python interpreter | trình thông dịch Python |  |
| python source code | mã nguồn Python |  |
| reference counting | đếm tham chiếu |  |
| regular expression | biểu thức chính quy |  |
| segmentation fault | lỗi phân đoạn |  |
| special characters | ký tự đặc biệt |  |
| undefined behavior | hành vi không xác định |  |
| unicode characters | các ký tự Unicode |  |
| universal newlines | ký tự xuống dòng phổ quát |  |
| Keyword Arguments | Đối số từ khóa |  |
| built-in function | hàm tích hợp sẵn |  |
| bytes-like object | đối tượng dạng bytes |  |
| callback function | hàm gọi lại |  |
| compression level | mức nén |  |
| context variables | biến ngữ cảnh |  |
| critical sections | các đoạn găng |  |
| current directory | thư mục hiện tại |  |
| current exception | ngoại lệ hiện tại |  |
| exception handler | trình xử lý ngoại lệ |  |
| extension modules | mô-đun mở rộng |  |
| garbage collected | được thu gom rác |  |
| garbage collector | bộ thu gom rác |  |
| keyword parameter | tham số từ khóa |  |
| line-buffered I/O | I/O có bộ đệm theo dòng |  |
| memory allocation | cấp phát bộ nhớ |  |
| memory allocators | bộ cấp phát bộ nhớ |  |
| method resolution | phân giải phương thức |  |
| namespace package | gói không gian tên |  |
| non-deterministic | không xác định |  |
| operating systems | các hệ điều hành |  |
| optional argument | đối số tùy chọn |  |
| path based finder | `path based finder` (kept) |  |
| path entry finder | `path entry finder` (kept) |  |
| python executable | tệp thực thi Python |  |
| python expression | biểu thức Python |  |
| release candidate | bản phát hành ứng viên |  |
| set comprehension | `set comprehension` (kept) |  |
| string formatting | định dạng chuỗi |  |
| timeout parameter | tham số timeout |  |
| unicode character | ký tự Unicode |  |
| working directory | thư mục làm việc |  |
| Argument Passing | Truyền đối số |  |
| Interactive Mode | Chế độ tương tác |  |
| ascii characters | ký tự ASCII |  |
| atomic operation | thao tác nguyên tử |  |
| attribute access | truy cập thuộc tính |  |
| buffer size, I/O | kích thước bộ đệm, I/O |  |
| c implementation | cài đặt C |  |
| class definition | định nghĩa lớp |  |
| closure variable | biến đóng |  |
| context managers | trình quản lý ngữ cảnh |  |
| context variable | biến ngữ cảnh |  |
| critical section | đoạn găng |  |
| current position | vị trí hiện tại |  |
| default behavior | hành vi mặc định |  |
| default encoding | mã hóa mặc định |  |
| deprecated alias | bí danh đã ngừng dùng |  |
| escape sequences | các chuỗi thoát |  |
| exception object | đối tượng ngoại lệ |  |
| extension module | mô-đun mở rộng |  |
| factory function | hàm tạo |  |
| file descriptors | bộ mô tả tệp |  |
| file-like object | đối tượng giống tệp |  |
| format specifier | `format specifier` (kept) |  |
| generator object | đối tượng sinh |  |
| generic function | hàm tổng quát |  |
| global namespace | không gian tên toàn cục |  |
| global variables | các biến toàn cục |  |
| import machinery | cơ chế import |  |
| integer overflow | tràn số nguyên |  |
| keyword argument | đối số từ khóa |  |
| lexical analyzer | bộ phân tích từ vựng |  |
| main interpreter | trình thông dịch chính |  |
| meta path finder | `meta path finder` (kept) |  |
| module attribute | thuộc tính mô-đun |  |
| multiple threads | đa luồng |  |
| non-empty string | chuỗi không rỗng |  |
| operating system | hệ điều hành |  |
| optional keyword | từ khóa tùy chọn |  |
| path-like object | đối tượng dạng đường dẫn |  |
| pattern matching | khớp mẫu |  |
| positive integer | số nguyên dương |  |
| protocol version | phiên bản giao thức |  |
| python functions | các hàm Python |  |
| python statement | câu lệnh Python |  |
| reference cycles | các vòng tham chiếu |  |
| relative imports | nhập tương đối |  |
| shared libraries | thư viện dùng chung |  |
| standard library | thư viện chuẩn |  |
| strong reference | tham chiếu mạnh |  |
| type annotations | chú thích kiểu |  |
| worker processes | các tiến trình worker |  |
| abstract method | phương thức trừu tượng |  |
| attribute names | tên thuộc tính |  |
| attribute value | giá trị thuộc tính |  |
| buffer protocol | giao thức bộ đệm |  |
| callable object | đối tượng gọi được |  |
| child processes | các tiến trình con |  |
| class attribute | thuộc tính lớp |  |
| class instances | các thể hiện lớp |  |
| complex numbers | số phức |  |
| context manager | trình quản lý ngữ cảnh |  |
| current context | ngữ cảnh hiện tại |  |
| current process | tiến trình hiện tại |  |
| data structures | các cấu trúc dữ liệu |  |
| dictionary view | chế độ xem từ điển |  |
| different types | các kiểu khác nhau |  |
| error indicator | chỉ báo lỗi |  |
| escape sequence | chuỗi thoát |  |
| exception class | lớp ngoại lệ |  |
| exception state | trạng thái ngoại lệ |  |
| expected output | đầu ra mong đợi |  |
| extension types | kiểu mở rộng |  |
| file descriptor | bộ mô tả tệp |  |
| follow symlinks | theo liên kết tượng trưng |  |
| fully qualified | đủ điều kiện |  |
| function object | đối tượng hàm |  |
| generic classes | lớp tổng quát |  |
| global variable | biến toàn cục |  |
| imported module | mô-đun đã nhập |  |
| install manager | trình quản lý cài đặt |  |
| instance method | phương thức thể hiện |  |
| internal buffer | bộ đệm nội bộ |  |
| library modules | mô-đun thư viện |  |
| local namespace | không gian tên cục bộ |  |
| local variables | các biến cục bộ |  |
| locale encoding | mã hóa locale |  |
| new-style class | lớp kiểu mới |  |
| optimized scope | phạm vi được tối ưu |  |
| optional module | mô-đun tùy chọn |  |
| path entry hook | `path entry hook` (kept) |  |
| pending removal | chờ loại bỏ |  |
| per-object lock | khóa theo đối tượng |  |
| posix platforms | nền tảng POSIX |  |
| provisional API | API tạm thời |  |
| python function | hàm Python |  |
| python language | ngôn ngữ Python |  |
| python programs | các chương trình Python |  |
| python versions | các phiên bản Python |  |
| reference count | số lượng tham chiếu |  |
| reference cycle | vòng tham chiếu |  |
| regular package | gói thông thường |  |
| signal handlers | các trình xử lý tín hiệu |  |
| single dispatch | điều phối đơn |  |
| soft deprecated | `soft deprecated` (kept) |  |
| special methods | phương thức đặc biệt |  |
| square brackets | dấu ngoặc vuông |  |
| standard output | đầu ra tiêu chuẩn |  |
| string literals | chuỗi ký tự |  |
| type parameters | tham số kiểu |  |
| underlying file | tệp nền tảng |  |
| unicode strings | các chuỗi Unicode |  |
| virtual machine | máy ảo |  |
| walrus operator | toán tử walrus |  |
| warning message | thông báo cảnh báo |  |
| weak references | các tham chiếu yếu |  |
| absolute value | giá trị tuyệt đối |  |
| address family | họ địa chỉ |  |
| attribute name | tên thuộc tính |  |
| built-in types | kiểu tích hợp sẵn |  |
| calling thread | luồng gọi |  |
| class creation | tạo lớp |  |
| class instance | thể hiện lớp |  |
| class variable | biến lớp |  |
| complex number | số phức |  |
| context object | đối tượng ngữ cảnh |  |
| current locale | locale hiện tại |  |
| current thread | luồng hiện tại |  |
| data structure | cấu trúc dữ liệu |  |
| decimal number | số thập phân |  |
| default values | các giá trị mặc định |  |
| directory tree | cây thư mục |  |
| error checking | kiểm tra lỗi |  |
| error handlers | trình xử lý lỗi |  |
| error handling | xử lý lỗi |  |
| error messages | các thông báo lỗi |  |
| exception type | kiểu ngoại lệ |  |
| flags argument | đối số cờ |  |
| floating point | dấu phẩy động |  |
| floor division | phép chia lấy phần nguyên |  |
| format strings | các chuỗi định dạng |  |
| free threading | luồng tự do |  |
| frozen modules | mô-đun đông lạnh |  |
| function calls | các lời gọi hàm |  |
| hash-based pyc | pyc dựa trên hash |  |
| home directory | thư mục home |  |
| internal state | trạng thái nội bộ |  |
| local variable | biến cục bộ |  |
| message object | đối tượng thông điệp |  |
| option strings | các chuỗi tùy chọn |  |
| parent process | tiến trình cha |  |
| python integer | số nguyên Python |  |
| python modules | các mô-đun Python |  |
| python objects | các đối tượng Python |  |
| python process | tiến trình Python |  |
| python program | chương trình Python |  |
| python runtime | môi trường chạy Python |  |
| python version | phiên bản Python |  |
| qualified name | tên đủ điều kiện |  |
| race condition | điều kiện tranh đua |  |
| reference leak | rò rỉ tham chiếu |  |
| running python | chạy Python |  |
| sequence types | kiểu dữ liệu tuần tự |  |
| shared library | thư viện dùng chung |  |
| signal handler | trình xử lý tín hiệu |  |
| special method | phương thức đặc biệt |  |
| standard error | lỗi tiêu chuẩn |  |
| standard input | đầu vào tiêu chuẩn |  |
| static methods | phương thức tĩnh |  |
| string literal | chuỗi ký tự |  |
| symbolic links | các liên kết tượng trưng |  |
| target process | tiến trình đích |  |
| trace function | hàm trace |  |
| type parameter | tham số kiểu |  |
| type variables | biến kiểu |  |
| unbuffered I/O | I/O không có bộ đệm |  |
| unicode object | đối tượng Unicode |  |
| unicode string | chuỗi Unicode |  |
| unix platforms | nền tảng Unix |  |
| value ellipsis | giá trị Ellipsis |  |
| version number | số phiên bản |  |
| weak reference | tham chiếu yếu |  |
| worker process | tiến trình worker |  |
| Zen of Python | `Zen of Python` (kept) |  |
| absolute path | đường dẫn tuyệt đối |  |
| abstract base | cơ sở trừu tượng |  |
| api functions | hàm API |  |
| argument list | danh sách đối số |  |
| boolean value | giá trị Boolean |  |
| builtin types | kiểu tích hợp sẵn |  |
| bytes objects | các đối tượng bytes |  |
| character set | bộ ký tự |  |
| child process | tiến trình con |  |
| class methods | các phương thức lớp |  |
| current frame | frame hiện tại |  |
| current value | giá trị hiện tại |  |
| decimal point | dấu chấm thập phân |  |
| default value | giá trị mặc định |  |
| email package | gói email |  |
| empty strings | các chuỗi rỗng |  |
| encoded bytes | byte đã mã hóa |  |
| error handler | trình xử lý lỗi |  |
| error message | thông báo lỗi |  |
| exception set | tập ngoại lệ |  |
| existing file | tệp hiện có |  |
| file position | vị trí tệp |  |
| format string | chuỗi định dạng |  |
| frame objects | các đối tượng frame |  |
| free variable | biến tự do |  |
| function call | lời gọi hàm |  |
| function name | tên hàm |  |
| hash function | hàm băm |  |
| import system | hệ thống import |  |
| initial value | giá trị ban đầu |  |
| integer value | giá trị số nguyên |  |
| memory blocks | các khối bộ nhớ |  |
| method object | đối tượng phương thức |  |
| module object | đối tượng mô-đun |  |
| new reference | tham chiếu mới |  |
| numeric types | kiểu số |  |
| option string | chuỗi tùy chọn |  |
| posix systems | hệ thống POSIX |  |
| python module | mô-đun Python |  |
| python object | đối tượng Python |  |
| python script | tập lệnh Python |  |
| python thread | luồng Python |  |
| return values | các giá trị trả về |  |
| shared memory | bộ nhớ chia sẻ |  |
| shared object | đối tượng dùng chung |  |
| string object | đối tượng chuỗi |  |
| symbolic link | liên kết tượng trưng |  |
| syntax errors | lỗi cú pháp |  |
| text encoding | mã hóa văn bản |  |
| thread safety | tính an toàn luồng |  |
| type checkers | trình kiểm tra kiểu |  |
| type checking | kiểm tra kiểu |  |
| type variable | biến kiểu |  |
| variable name | tên biến |  |
| base classes | các lớp cơ sở |  |
| bytes object | đối tượng bytes |  |
| bytes string | chuỗi byte |  |
| c extensions | các phần mở rộng C |  |
| class method | phương thức lớp |  |
| class object | đối tượng lớp |  |
| code objects | các đối tượng mã |  |
| command line | dòng lệnh |  |
| compile time | thời gian biên dịch |  |
| content type | kiểu nội dung |  |
| current time | thời gian hiện tại |  |
| empty string | chuỗi rỗng |  |
| entry points | các điểm vào |  |
| enum members | thành viên enum |  |
| file objects | đối tượng tệp |  |
| frame object | đối tượng frame |  |
| generic type | kiểu generic |  |
| global state | trạng thái toàn cục |  |
| header files | các tệp tiêu đề |  |
| help message | thông báo trợ giúp |  |
| http headers | `http headers` (kept) |  |
| key function | hàm khóa |  |
| lazy imports | import lười |  |
| line numbers | các số dòng |  |
| linker flags | cờ liên kết |  |
| magic method | phương thức ma thuật |  |
| match object | đối tượng Match |  |
| memory block | khối bộ nhớ |  |
| memory usage | mức sử dụng bộ nhớ |  |
| method calls | lời gọi phương thức |  |
| module level | cấp mô-đun |  |
| module names | tên các mô-đun |  |
| module state | trạng thái mô-đun |  |
| nested scope | phạm vi lồng nhau |  |
| object types | các kiểu đối tượng |  |
| package name | tên gói |  |
| python c api | C API của Python |  |
| release date | ngày phát hành |  |
| return value | giá trị trả về |  |
| side effects | các tác dụng phụ |  |
| source files | các tệp mã nguồn |  |
| start method | phương thức khởi động |  |
| string value | giá trị chuỗi |  |
| syntax error | lỗi cú pháp |  |
| system calls | các lời gọi hệ thống |  |
| thread state | trạng thái luồng |  |
| type aliases | bí danh kiểu |  |
| type checker | trình kiểm tra kiểu |  |
| type objects | đối tượng kiểu |  |
| unicode code | mã Unicode |  |
| xml document | tài liệu XML |  |
| I/O control | điều khiển I/O |  |
| Python 3000 | `Python 3000` (kept) |  |
| binary data | dữ liệu nhị phân |  |
| binary file | tệp nhị phân |  |
| binary mode | chế độ nhị phân |  |
| buffer size | kích thước bộ đệm |  |
| byte string | chuỗi byte |  |
| c extension | phần mở rộng C |  |
| c functions | hàm C |  |
| code object | đối tượng mã |  |
| code points | điểm mã |  |
| concurrency | đồng thời |  |
| debug hooks | hook gỡ lỗi |  |
| duck-typing | kiểu vịt |  |
| empty tuple | tuple rỗng |  |
| entry point | điểm vào |  |
| exit status | trạng thái thoát |  |
| false value | giá trị sai |  |
| fatal error | lỗi nghiêm trọng |  |
| field names | tên trường |  |
| file format | định dạng tệp |  |
| file object | đối tượng tệp |  |
| file system | hệ thống tệp |  |
| format code | mã định dạng |  |
| format spec | `format spec` (kept) |  |
| header file | tệp tiêu đề |  |
| import path | đường dẫn import |  |
| interactive | tương tác |  |
| line number | số dòng |  |
| main module | mô-đun chính |  |
| main thread | luồng chính |  |
| memory leak | rò rỉ bộ nhớ |  |
| mock object | đối tượng mock |  |
| module name | tên mô-đun |  |
| module spec | đặc tả mô-đun |  |
| named tuple | tuple có tên |  |
| native code | mã gốc |  |
| object type | kiểu đối tượng |  |
| parallelism | tính song song |  |
| pure python | Python thuần túy |  |
| python code | mã Python |  |
| python type | kiểu Python |  |
| return code | mã trả về |  |
| return type | kiểu trả về |  |
| root logger | logger gốc |  |
| search path | đường dẫn tìm kiếm |  |
| side effect | tác dụng phụ |  |
| source code | mã nguồn |  |
| source file | tệp mã nguồn |  |
| source tree | cây mã nguồn |  |
| stack trace | dấu vết ngăn xếp |  |
| static type | kiểu tĩnh |  |
| system call | lời gọi hệ thống |  |
| test method | phương thức kiểm thử |  |
| test runner | trình chạy kiểm thử |  |
| third party | bên thứ ba |  |
| thread-safe | an toàn luồng |  |
| truth value | giá trị logic |  |
| type object | đối tượng kiểu |  |
| zip archive | tệp lưu trữ ZIP |  |
| __format__ | `__format__` (kept) |  |
| __future__ | `__future__` (kept) |  |
| base class | lớp cơ sở |  |
| blank line | dòng trống |  |
| byte order | thứ tự byte |  |
| c compiler | trình biên dịch C |  |
| c function | hàm C |  |
| c standard | tiêu chuẩn C |  |
| call stack | ngăn xếp lời gọi |  |
| class body | thân lớp |  |
| class name | tên lớp |  |
| code block | khối mã |  |
| code point | điểm mã |  |
| contiguous | liên tục |  |
| data types | các kiểu dữ liệu |  |
| debug mode | chế độ gỡ lỗi |  |
| descriptor | bộ mô tả |  |
| dictionary | từ điển |  |
| empty list | danh sách rỗng |  |
| error code | mã lỗi |  |
| event loop | vòng lặp sự kiện |  |
| expression | biểu thức |  |
| file names | tên tệp |  |
| hash value | giá trị băm |  |
| heap types | kiểu trên heap |  |
| input data | dữ liệu đầu vào |  |
| ip address | địa chỉ IP |  |
| local time | giờ địa phương |  |
| path entry | `path entry` (kept) |  |
| process id | ID tiến trình |  |
| public api | API công khai |  |
| raw string | chuỗi thô |  |
| ssl module | mô-đun ssl |  |
| stable abi | ABI ổn định |  |
| stack size | kích thước ngăn xếp |  |
| test cases | các trường hợp kiểm thử |  |
| test suite | bộ kiểm thử |  |
| text files | tệp văn bản |  |
| text plain | văn bản thuần túy |  |
| true value | giá trị đúng |  |
| type alias | bí danh kiểu |  |
| type hints | `type hints` (kept) |  |
| web server | máy chủ web |  |
| whitespace | khoảng trắng |  |
| Character | Ký tự |  |
| Condition | Điều kiện |  |
| __slots__ | `__slots__` (kept) |  |
| ast nodes | nút AST |  |
| attribute | thuộc tính |  |
| awaitable | `awaitable` (kept) |  |
| base type | kiểu cơ sở |  |
| buffering | bộ đệm |  |
| c library | thư viện C |  |
| code page | trang mã |  |
| data race | tranh chấp dữ liệu |  |
| data type | kiểu dữ liệu |  |
| decorator | trình trang trí |  |
| directory | thư mục |  |
| docstring | `docstring` (kept) |  |
| exit code | mã thoát |  |
| f-strings | chuỗi f |  |
| file name | tên tệp |  |
| file path | đường dẫn tệp |  |
| generator | trình sinh |  |
| immutable | bất biến |  |
| lock-free | không khóa |  |
| lru cache | bộ nhớ đệm LRU |  |
| metaclass | siêu lớp |  |
| mime type | kiểu MIME |  |
| namespace | không gian tên |  |
| open file | tệp mở |  |
| parameter | tham số |  |
| reentrant | tái nhập |  |
| statement | câu lệnh |  |
| subscript | truy cập theo chỉ số |  |
| t-strings | `t-strings` (kept) |  |
| test case | trường hợp kiểm thử |  |
| text file | tệp văn bản |  |
| text mode | chế độ văn bản |  |
| time zone | múi giờ |  |
| top level | cấp cao nhất |  |
| traceback | `traceback` (kept) |  |
| type hint | `type hint` (kept) |  |
| user code | mã người dùng |  |
| zip files | các tệp ZIP |  |
| # (hash) | `# (hash)` (kept) |  |
| Glossary | bảng thuật ngữ |  |
| Infinity | vô cực |  |
| Pythonic | `Pythonic` (kept) |  |
| argument | đối số |  |
| builtins | `builtins` (kept) |  |
| bytecode | `bytecode` (kept) |  |
| c string | chuỗi C |  |
| callable | `callable` (kept) |  |
| callback | hàm callback |  |
| deadlock | khóa chết |  |
| encoding | mã hóa |  |
| function | hàm |  |
| hashable | `hashable` (kept) |  |
| immortal | `immortal` (kept) |  |
| importer | trình nhập |  |
| iterable | `iterable` (kept) |  |
| iterator | trình lặp |  |
| sequence | dãy |  |
| zip file | tệp ZIP |  |
| Boolean | `Boolean` (kept) |  |
| CPython | `CPython` (kept) |  |
| c stack | ngăn xếp C |  |
| comment | chú thích |  |
| context | ngữ cảnh |  |
| mapping | ánh xạ |  |
| mutable | có thể thay đổi |  |
| newline | ký tự xuống dòng |  |
| package | gói |  |
| portion | phần |  |
| timeout | thời gian chờ |  |
| c type | kiểu C |  |
| finder | trình tìm |  |
| lambda | `lambda` (kept) |  |
| loader | trình tải |  |
| method | phương thức |  |
| stdlib | `stdlib` (kept) |  |
| string | chuỗi |  |
| Event | Sự kiện |  |
| class | lớp |  |
| float | `float` (kept) |  |
| index | chỉ số |  |
| slice | `slice` (kept) |  |
| token | `token` (kept) |  |
| BDFL | `BDFL` (kept) |  |
| EAFP | `EAFP` (kept) |  |
| IDLE | `IDLE` (kept) |  |
| LBYL | `LBYL` (kept) |  |
| Lock | `Lock` (kept) |  |
| REPL | `REPL` (kept) |  |
| exec | `exec` (kept) |  |
| file | tệp |  |
| list | `list` (kept) |  |
| type | `type` (kept) |  |
| GIL | `GIL` (kept) |  |
| MRO | `MRO` (kept) |  |
| NaN | `NaN` (kept) |  |
| PEP | `PEP` (kept) |  |
| key | khóa |  |
| sys | `sys` (kept) |  |

<!-- /generated: terms -->

### Notes on terms that are easy to get wrong

The table carries the rendering. These are the reasons behind the ones
that have caught people out, and the wordings to avoid.

| English | Notes |
|---|---|
| tuple, dict, set, frozenset | built-in container types |
| str, int, float, bool, bytes, bytearray | built-in scalar types |
| None, True, False | literals |
| iterator, iterable, generator | iteration protocol |
| decorator | `@foo` decorator syntax |
| callable | anything with `__call__` |
| context manager | `with` statement protocol |
| module, package | code organization |
| namespace | scopes, not the same as "vùng tên" in casual usage |
| attribute, method, property | object members; do not translate to "thuộc tính/phương thức" which are heavier and less precise |
| class, instance, object | OOP terms |
| exception | error-handling terms |
| traceback | stack trace |
| comprehension | list/dict/set/generator comprehensions |
| slice, slicing | list/string indexing |
| unpacking, packing | `*args`, tuple unpacking |
| closure | nested-function variable capture |
| thread, process | concurrency primitives |
| socket | networking |
| regex, regular expression | pattern matching |
| docstring | function/class documentation string |
| REPL, prompt | interactive interpreter |
| REPL | `>>>` prompt |
| API, CLI, URL, HTTP, JSON, XML | standard acronyms |
| boolean | the type is `bool` and the adjective is "boolean" |
| Unicode, ASCII, UTF-8 | encoding names |
| path, pathname | file system paths (see also "đường dẫn" below) |
| shell script | Unix shell scripts; do not translate to "tập lệnh shell" |
| batch file | Windows batch files; do not translate to "tệp bó" |
| script | kept English; do not translate to "tập lệnh" |
| tty | terminal device; kept English |
| shebang | `#!/usr/bin/env python3` line; kept English |
| literal | string/number literal in source code; kept English
| GUI, I/O | interface and I/O acronyms |
| issue, issue tracker | kept English in prose (e.g. "trên issue tracker") |
| raw string | Python raw-string literal (e.g. `r"..."`) |
| stdin, stdout, stderr | standard streams |

### Translate

These are general computing terms where Vietnamese already has a
settled, widely-understood translation.

| English | Vietnamese |
|---|---|
| documentation | tài liệu |
| example | ví dụ |
| error | lỗi |
| warning | cảnh báo |
| variable | biến |
| value | giá trị |
| expression | biểu thức |
| statement | câu lệnh |
| loop | vòng lặp |
| condition | điều kiện |
| function | hàm |
| parameter | tham số |
| argument | đối số |
| return value | giá trị trả về |
| default value | giá trị mặc định |
| syntax | cú pháp |
| keyword | từ khóa |
| operator | toán tử |
| number | số |
| integer | số nguyên |
| floating-point | dấu phẩy động |
| list | danh sách (keep `list` for the type name itself when used as code) |
| string | chuỗi (but keep `str` for the type name) |
| character | ký tự |
| byte | byte (kept English) |
| file | tệp (not "tập tin": the human files use `tệp` 20 times and `tập tin` never) |
| directory, folder | thư mục |
| path | đường dẫn |
| input, output | đầu vào, đầu ra |
| command line | dòng lệnh |
| library | thư viện |
| framework | framework (kept English) |
| implementation | triển khai |
| version | phiên bản |
| release | bản phát hành |
| install, installation | cài đặt |
| import | import (kept, verb form stays English) |
| source code | mã nguồn |
| algorithm | thuật toán |
| data structure | cấu trúc dữ liệu |
| memory | bộ nhớ |
| platform | nền tảng |
| operating system | hệ điều hành |
| developer | lập trình viên |
| user | người dùng |
| environment | môi trường |
| variable (environment) | biến môi trường |
| tutorial | hướng dẫn |
| reference | tham khảo |
| deprecated | không dùng nữa (adjective); có thể dùng "đã bỏ" in past tense |
| built-in | tích hợp sẵn (not "dựng sẵn"; picked for consistency with `introduction.po`) |
| interpreter | trình thông dịch |
| interpreted language | ngôn ngữ thông dịch |
| compile, compilation | biên dịch |
| link, linking | liên kết (in the compile/link sense) |
| indentation | thụt lề |
| prompt | dấu nhắc (the `>>>` and `...` markers in the REPL) |
| comment | chú thích (never "bình luận" in a code context) |
| hash character | ký tự băm (the `#` that starts a Python comment) |
| bug | lỗi |
| patch | bản vá |
| test, testing | kiểm thử |
| test suite | bộ kiểm thử |
| high-level, low-level | bậc cao, bậc thấp |
| throw-away program | chương trình dùng một lần |
| extension language | ngôn ngữ mở rộng |
| bottom-up, top-down | từ dưới lên, từ trên xuống |
| indexing | truy cập theo chỉ số (action) / chỉ số (noun) |
| slicing | cắt lát (when translated); the Python term `slice` stays English |
| identifier | định danh (not "mã định danh") |
| encoding | mã hóa (the verb/noun); keep specific names like UTF-8, ASCII |
| encoding declaration | khai báo mã hóa |
| continuation line | dòng nối tiếp |
| primary prompt, secondary prompt | dấu nhắc chính, dấu nhắc phụ |
| welcome message | thông điệp chào mừng |
| standard input, standard output | stdin, stdout (prefer the short English forms in prose) |
| exit status | mã trạng thái thoát |
| portable code | mã đa nền tảng (not "mã di động") |

### Judgment calls

Where the choice depends on context.

- **"You"**: see Pronoun section above.
- **"Simply", "just"**: usually drop in Vietnamese. It reads
  condescending.
- **"Note that..."**: translate to "Lưu ý:", not "Chú ý rằng..." which
  is more awkward.
- **"See X"**: "Xem X".
- **"Returns X"**: use noun form "Trả về X", not "Hàm trả về X".
- **"Raises X"**: "Gây ra X" or "Ném X" — prefer "Gây ra X".
- **"The X function"**: drop the article, just "Hàm X" or keep X in
  code style without "hàm" at all. `:func:\`X\`` handles the hyperlink
  either way.

### Tricky cases

- `async` / `await`: keep English. `asyncio` too.
- `type hint`, `type annotation`: "chú thích kiểu" reads better than
  "gợi ý kiểu".
- `yield`: keep English. Do not translate to "trả ra" or similar.
- `iterable` vs `iterator`: keep both English. They are different
  protocols and Vietnamese has no concise single-word distinction.
- `raise` (exception): keep as a verb; "Gây ra một exception" reads
  better than "Ném một ngoại lệ".
- `with` statement: "câu lệnh `with`" — keep `with` in code style.
- `__init__`, `__call__`, dunders: never translate; wrap in backticks.
- `:term:` references: leave the target name (e.g. `:term:`immutable``)
  untouched. The Sphinx glossary handles the link text. Do not try to
  pre-translate the anchor.
- `:ref:` link text: translate the visible link label when it is a
  Vietnamese word (e.g. `:ref:`đóng góp <contributing-to-python>``),
  but never alter the anchor inside `<...>`.
- English emphasis inside Vietnamese prose: when the `msgid` italicizes
  a term (e.g. `*body*`, `*indented*`, `*existing list*`) and we have a
  Vietnamese equivalent, italicize the Vietnamese instead of keeping
  the English word in italic. Keeping both looks like half-translated
  MT output.
- Gerund/verbal-noun headings ("Whetting Your Appetite", "Dealing with
  Bugs", "An Informal Introduction to Python"): rewrite as a Vietnamese
  noun phrase, not a direct gerund. "Khơi gợi hứng thú", "Xử lý lỗi",
  "Giới thiệu không chính thức về Python".

## Common MT artifacts to fix during review

These are patterns the Google MT output in PR #1 kept producing. Watch
for them and fix during unfuzzy review.

1. **Over-literal `bạn`.** Google uses it in every sentence. Most can be
   dropped. Keep only where the text is actually addressing the reader.
2. **"Các" noise.** Google inserts `các` before every plural noun. In
   Vietnamese, `các` is often unnecessary and can be dropped ("các
   hàm" → "hàm" when context is clear).
3. **"Việc X"**: Google frequently wraps verbs in `việc X`. Often
   cleaner to use the verb directly: "Việc sử dụng X" → "Sử dụng X".
4. **Literal "rằng".** Google translates "that" as "rằng" even when
   Vietnamese would omit the complementizer. "cho rằng" → "cho là" or
   drop entirely.
5. **Inverted adjective-noun order.** "Python function" → Google gives
   "hàm Python" (correct). But "built-in function" sometimes becomes
   "built-in hàm" which is wrong. Should be "hàm dựng sẵn" or "hàm
   built-in".
6. **Code tokens in awkward positions.** Because placeholders kept
   `:func:\`x\`` intact, Vietnamese word order sometimes leaves the
   token dangling. Rewrite for fluency.
7. **Wrong-register calques.** MT picks the dictionary's first hit
   regardless of domain. Examples seen in PR #1:
   - *straightforward* → "thẳng thắn" (applies to people, not syntax).
     Use "rõ ràng" or "đơn giản".
   - *whetting your appetite* → "kích thích sự thèm ăn" (literal food
     sense). Use "khơi gợi hứng thú".
   - *good practices* → "thực hành tốt" (literal). Use "thông lệ tốt".
   - *throw-away programs* → "các chương trình cũ" (means *old*
     programs). Use "chương trình dùng một lần".
   - *socket* → "ổ cắm" (electrical outlet). Keep English.
   - *dictionary* (Python dict) → "từ điển". Keep `dict` in English.
   - *batch file* → "tệp bó". Keep `batch file` in English.
8. **Passive-voice calques.** "X được Y" is legitimate Vietnamese, but
   MT overuses it. Prefer active voice when the agent is clear:
   - *This variable should be treated as read-only by the user* →
     "Người dùng nên xem biến này là chỉ đọc"
     (not "Biến này nên được người dùng xem là chỉ đọc").
9. **"Việc" wrappers.** "Việc X" is correct but frequently unnecessary.
   "Việc sử dụng X" → "Sử dụng X"; "việc có hay không có Y" →
   "sự xuất hiện của Y".

## How to update this file

Open a PR that changes `GLOSSARY.md` in the same commit as whatever
`.po` changes motivated the update. State the motivating file and a
one-line reason. Sweep any other files that the old rule applied to
in the same PR if it is small, or open a follow-up if it is large.

No vote is required for uncontroversial additions (new Python 3.x
keywords, clearly-settled translations). Changes to settled rules in
this file need at least one reviewer from the team.
