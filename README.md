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

# Priority?

1. Internal, External ?
> Không có sự ưu tiên , đứa nào gọi sau thì ưu tiên đứa đó (ai viết css mới hơn)
2. Inline - 1000
```html
<h1 style="color: blue;">.....</h1>
```
3. #id - 100
4. .class - 10
5. tag - 1 ``` gọi thẳng cái tên của thẻ (VD: h1)```
- Cách nào nhiều điểm hơn thì được ưu tiên hơn
6. Equal specificity?
giống nhau nhma cái nào mới hơn thì dc ưu tiên hơn
```html
#heading-id {
    color: violet;
}
#heading-id {
    color: blue;
}
```
> Thì ```blue``` được thực hiện
- Tích hợp giữa ```id``` và ```class``` và ```tag``` bỏ qua ```Inline``` vì nó quá mạnh
7. Universal selector and inherited?
- Điểm Universal: 0
- inherited : kế thừa : 0
