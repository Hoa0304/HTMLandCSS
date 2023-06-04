# CSS in HTML?
> các cách sử dụng CSS trong file HTML
- Internal : sử dụng một cặp thẻ ```<style>``` trong chính file html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1 {
            color: blue;
            font-size: 70px;
        }
    </style>
</head>
<body>
    <h1>Trần Thị Cẩm Hoa</h1>
</body>
</html>
```
- External : tạo file css bên ngoài , link vào file html


- Inline : sử dụng attribute style trong thẻ mở và viết vào 
```html
<h1 style="color: blueviolet;">Trần Thị Cẩm Hoa</h1>
```