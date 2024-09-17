# GIT (tiếp theo)
### Xem lại lịch sử commit
    git log

### Thay đổi commit mesage
    git commit --amend
        - Gõ i -> vào chế độ insert
        - Gõ esc để thoát insert
        - Gõ “:wq” -> write and quit

- git commit --amend-m”<message>”: cũng là thay đổi commit message nhưng được phép thay đổi trực tiếp mà không cần phải mở trình soạn thảo VIM

### Đưa từ vùng Staging về Working Directory
    git restore --staged <file>

### Đưa từ vùng repository về Working Directory (uncommit)

    git reset HEAD~1 (undo 1 commit)

## Branch
    Dùng branch để tạo ra một vùng làm việc mới, không ảnh hưởng tới vùng làm việc đã ổn định.

### Tạo branch 
    git branch <ten_branch>
    git checkout <ten_branch>
    git checkout -b <ten_branch> (*) // ưu tiên hơn

- Tips: Luôn tạo branch mới trước khi thực hiện một lệnh copy từ internet

# Javascript Basic (tiếp theo)

## Object
- Khai báo: 
    
        let/const <ten_object> = {
            <thuoc_tinh>: <gia_tri>
            ...
        }
Trong đó:
- <thuoc_tinh>: giống quy tắc đặt tên biến
- <gia tri>: có kiểu giống biến, hoặc là 1 object khác.

## Logical Operator

    && : cả 2 vế của mệnh đề đều đúng
    || : một trong 2 vế đúng
    ! : đảo ngược lại giá trị của mệnh đề

## Array (mảng)
- Khai báo: 

        let/const <ten_mang> = [<gia_tri>];

- Truy xuất mảng: 
    
        Độ dài mảng: length
        Lấy phần tử theo index: [0], [1], [2]

## Function (Hàm)
- Là đoạn code được đặt tên và có thể tái sử dụng nhiều lần.

- Khai Báo: 
    
        function <nameFunction>() {
            // code
        }

## == và !=
== và != : 
- So sánh kiểu “lỏng lẻo”
- Convert giá trị về kiểu
“lớn hơn”

===: so sánh tuyệt đối

## Vòng lặp nâng cao: break and continue

Break : dùng để kết thúc sớm trong quá trình thực thi của 1 vòng lặp

Continue: khi được thực hiện thì nó sẽ bỏ qua câu lệnh bên dưới nó trong vòng lặp và quay trở lại vòng lặp mới