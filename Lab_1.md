# Lab 1

## Bài 1 (2 điểm)
- Cho đoạn code:

```
<html>
    <head>
        <style>
            #target {
                width: 60px;
                height: 60px;
                background: #33691E;
            }
        </style>
    </head>
    <body>
        <div id="target"></div>
        <script>
            var target = document.querySelector("#target");
            target.onmouseover = function () {
                // Thực hiện đổi màu sang #BF360C
            };

            target.onmouseout = function () {
                // Thực hiện đổi màu sang #33691E
            };
        </script>
    </body>
</html>
```

- Yêu cầu: Hoàn thiện code cho 2 sự kiện onmouseover & onmouseout trong function tương ứng.

- Gợi ý: hãy sử dụng thuộc tính “style”

## Bài 2 (2 điểm)
- Cho đoạn code như sau:

```
<html>
    <head>
        <style>
            #color {
                width: 200px;
                height: 30px;
                line-height: 30px;
                margin-bottom: 20px;
                display: block;
                background: #33691E;
            }
        </style>
    </head>
    <body>
        <input type="text" id="text-input" value="33691E"/>
        <h3>Input Text</h3>
        <script>
            var h3Tag = document.querySelector("h3");
            var input = document.querySelector("#text-input");
            input.onkeyup = function () {
                /*
                 *   Thay đổi giá trị hiển thị của thẻ h3
                 *      theo giá trị của ô input
                */
            };
        </script>
    </body>
</html>
```

- Yêu cầu: text trong thẻ input thay đổi thì chữ viết trong thẻ h3 cũng đc thay đổi ngay lập tức.
- Gợi ý: sử dụng thuộc tính “value” và “innerText”

## Bài 3 (3 điểm)
- Cho 2 đoạn code **HTML** & **Javascript** như sau:

```
<html>
    <head>
        <!-- Bootstrap CDN -->
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
    </head>
    <body>
        <table class="table">
        <tr>
            <th>Mã SV</th>
            <th>Họ Tên</th>
            <th>Ngày Sinh</th>
            <th>Email</th>
        </tr>
        <tbody id="tbl-body">
        </tbody>
        </table>

        <!-- Jquery CDN -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    </body>
</html>
```

```
const array = [
    {
        'code': 'PH12345',
        'name': 'Nguyen Van A',
        'date_of_birth': (new Date()).toString(),
        'email': 'anguyenvan@gmail.com',
    },
    {
        'code': 'PH12346',
        'name': 'Nguyen Van B',
        'date_of_birth': (new Date()).toString(),
        'email': 'bnguyenvan@gmail.com',
    },
    {
        'code': 'PH12347',
        'name': 'Nguyen Van C',
        'date_of_birth': (new Date()).toString(),
        'email': 'cnguyenvan@gmail.com',
    },
];
```

- Yêu cầu: sử dụng Javascript để hiển thị data trong array ra màn hình.

## Bài 4 (3 điểm)
- Yêu cầu: 
    - Tạo 1 danh sách sinh viên cho phép thêm, xoá sinh viên.
    - Có các tính năng:
        - thêm sinh viên vào đầu danh sách
        - thêm sinh viên vào cuối danh sách
        - xoá sinh viên ở đầu danh sách
        - xoá sinh viên ở cuối danh sách
    - Đối với trường thông tin **Ngày sinh**, cần sử dụng **Date**, không làm bằng *string*.

- Mockup trong thư mục `images/lab1_bai4.png`.

