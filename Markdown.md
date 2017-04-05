# **MARKDOWN**

## **1. Tổng quan về Markdown:**

**Markdown** là một ngôn ngữ đánh dấu bằng cú pháp định dạng văn bản thuần. Nó được thiết kế để chuyển đổi qua *HTML* và nhiều định dạng khác sử dụng một công cụ cùng tên. Markdown thường được sử dụng để định dạng file *readme*, viết thông báo cho các diễn dàn trực tuyến và được tạo các siêu văn bản  sử dụng editor văn bản thuần (không biết dịch thế nào đây: plain text editor). ***John Gruber*** đã tạo ra Markdown vào năm 2004 cùng với ***Aaron Swartz***. Với mục tiêu là cho phép mọi người sử dụng một định dạng ở dạng *plain text* dễ đọc, dễ viết và tùy chọn chuyển đổi nó thành XHTML (hoặc HTML) hợp lệ.

Một số phần mềm sử dụng ngôn ngữ Markdown: *Github*, Gitbook, Reddit, Diaspora, Stack Overflow, OpenStreetMap và một số ứng dụng khác.

Phần mở rộng: ```.md```

## **2. Cách sử dụng Markdown:** 

### *a. Header:*

Markdown hỗ trợ 2 kiểu viết tiêu đề: Setext và ATX.

* Với *Setext* : sử dụng kí tự `=` và `-` gạch chân dưới tiêu đề, sử dụng cho 2 thẻ `<h1>` và `<h2>`.
---
```
Header1
=
```
Header1
=
---
```
Header2
-
```
Header2
-
---

* Với *ATX* : sử dụng ký tự `#` đặt trước các tiêu đề. Số ký tự đặt trước tiêu đề biểu diễn lần lượt từ `<h1>` đến `<h6>`
---
```
# Header1
## Header2
### Header3
#### Header4
##### Header5
###### Header6
```
# Header1
## Header2
### Header3
#### Header4
##### Header5
###### Header6
---
### *b. Emphasis:*
* In nghiêng: sử dụng ký tự `*` hoặc `_` đặt trước và sau phần muốn in nghiêng.


`*in nghiêng*` hoặc `_in nghiêng_`

*in nghiêng* hoặc _in nghiêng_

---
* In đậm: sử dụng ký tự `**` hoặc `__` đặt trước và sau phần muốn in đậm.

`**in đậm**` hoặc `__in đậm__`

**in đậm** hoặc __in đậm__

---
* c. Gạch giữa: sử dụng ký tự `~~` đặt trước và sau phần muốn gạch giữa.

`~~Gạch giữa~~`

~~Gạch giữa~~

---
* d. Kết hợp:
```
***Vừa in nghiêng, vừa in đậm***
___Vừa in nghiêng, vừa in đậm___
_**Vừa in nghiêng, vừa in đậm**_
__*Vừa in nghiêng, vừa in đậm*__
***Vừa in nghiêng, vừa in đậm***
___Vừa in nghiêng, vừa in đậm___
_**Vừa in nghiêng, vừa in đậm**_
__*Vừa in nghiêng, vừa in đậm*__
```

***Vừa in nghiêng, vừa in đậm***

___Vừa in nghiêng, vừa in đậm___

_**Vừa in nghiêng, vừa in đậm**_

__*Vừa in nghiêng, vừa in đậm*__

***Vừa in nghiêng, vừa in đậm***

___Vừa in nghiêng, vừa in đậm___

_**Vừa in nghiêng, vừa in đậm**_

__*Vừa in nghiêng, vừa in đậm*__

---
### *c. Lists:*
---
* List sử dụng số thứ tự: 
```
1. Dòng 1:
2. Dòng 2:
3. Dòng 3:
```
1. Dòng 1:
2. Dòng 2:
3. Dòng 3:
---
* List sử dụng ký hiệu:
```
* Dấu sao
+ Dấu cộng
- Dấu trừ
```
* Dấu sao
+ Dấu cộng
- Dấu trừ
---
### *d. Links:*
Có **2** cách để tạo links : ***inline-style*** và ***reference-style***
* *inline-style*
```
[Tên liên kết](link)

Mở rộng: [Tên liên kết](link "Tiêu đề tự chọn cho liên kết")
```

Đoạn văn bản trong dấu `[]` tương đương với giá trị của thuộc tính *title* trong thẻ `<a>` và link đặt trong dấu `()` sẽ tương đương với giá trị thuộc tính *href* trong thẻ `<a>`


```
[Đây là đường dẫn đến Google](https://www.google.com)
[Đây là đường dẫn đến Google](https://www.google.com "Tìm kiếm bằng Google")
```
[Đây là đường dẫn đến Google](https://www.google.com)

[Đây là đường dẫn đến Google](https://www.google.com "Tìm kiếm bằng Google")

---
* *reference-style*
```
[Tên liên kết][Label]
[Label]:link

Mở rộng: 
[Label]:link "Tiêu đề tự chọn cho liên kết"
```

```
Bấm vào [đây][lb] để truy cập Google.

[lb]:https://www.google.com "Truy cập Google"
```

Bấm vào [đây][lb] để truy cập Google.

[lb]:https://www.google.com "Truy cập Google"

Để ngắn gọn, có thể gộp phần [Tên liên kết] với [Label] thành một.

```
Bấm vào [đây] để truy cập Google.

[đây]:https://www.google.com "Truy cập Google"
```
Bấm vào [đây] để truy cập Google.

[đây]:https://www.google.com "Truy cập Google"

---
* Ngoài ra, nếu để URL trong cặp dấu `<` `>`, thì URL sẽ tự động tạo đường dẫn đến nó.

```
<URL>
```
```
<https://www.google.com>
```
<https://www.google.com>

---
### *e. Image:*
Tương tự links, hình ảnh cũng có 2 cách để tạo:
* *inline-style*
```
![Tên hình ảnh](link của hình ảnh "Mô tả tùy chọn")
```

```
![anh-dep]()
```

![anh-dep]()

Đoạn văn bản trong dấu `[]` tương đương với giá trị của thuộc tính *alt* trong thẻ `<img>` và link đặt trong dấu `()` sẽ tương đương với giá trị thuộc tính *src* trong thẻ `<img>`

* *reference-style*
```
![Tên hình ảnh][Label]
[Label]:link của hình ảnh "Mô tả tùy chọn"
```


```
![anh-dep][lb]

[lb]: 
```


### *f. Code and Syntax Highlighting:*
* *Syntax Highlighting*
```
`Syntax`
```

`Syntax`

* *Block Highlighting*

```
Syntax 1
Syntax 2
Syntax 3
...
```


* *Code Highlighting*

````
```language
Code 1
Code 2
Code 3 
```
````



```
```python
s = 'Hello World!'
print s
```
```

```python
s = 'Hello World!'
print s
```

### *g. Tables*
Cấu trúc bảng sẽ như thế này:
```
|col 1|col 2|col 3|
|:----|:---:|----:|
|a|b|c|
```
Hàng đầu tiên, định danh của các cột
Hàng thứ hai, canh lề cho từng cột
`:-----` hoặc `-----` dùng để canh trái.
`:----:` dùng để canh giữa.
`-----:` dùng để canh phải.
Những hàng tiếp theo, chứa nội dung tương ứng với các cột.
|col 1|col 2|col 3|
|:----|:---:|----:|
|a|b|c|

*Lưu ý:* Các dấu `|` ở ngoài cùng có thể lược bỏ.
```
col 1|col 2|col 3
:----|:---:|----:
a|b|c
```

Thôi, cứ coi như cơ bản tại đây! Có gì mới, update thêm! 