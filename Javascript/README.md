# Tuyển tập câu hỏi phỏng vấn Javascript

# Table of Contents

1. [Hỏi về Javascript](#hỏi-về-javascript)
2. [Hỏi về Testing](#hỏi-về-testing)
3. [Hỏi về Performance](#hỏi-về-performance)
4. [Hỏi về Network](#hỏi-về-network)
5. [Hỏi về Coding](#hỏi-về-coding)
6. [Hỏi chơi cho vui](#hỏi-chơi-cho-vui)

## Hỏi về Javascript

* Ý nghĩa của biến `this`.
    * [answer](https://developer.mozilla.org/vi/docs/Web/JavaScript/Reference/Operators/this)
* Sử dụng **AMD** và **CommonJS** có tốt hay không? Tại sao tốt hoặc không tốt?
    * [answer](https://www.codementor.io/michaelaboagye/comparing-commonjs-and-amd-requirejs-4pu4twa4n)
* Nếu viết theo kiểu IIFE (Immediately-Invoked Function Expression), tại sao đoạn mã sau bị lỗi? `function foo(){ }();`
  * Sửa lại : `(function(){ function foo() {} }())`
* Khác nhau giữa `null`, `undefined` hoặc chưa khai báo?
  * Cách kiểm tra từng trường hợp trên.
* Khác nhau giữa **host objects** và **native objects** là gì?
    * [answer](http://lucybain.com/blog/2014/host-vs-native/)
* Javascript closure là gì?
    * [answer](https://kipalog.com/posts/JavaScript-Closures)
* `ES6` Yeild là gì? [giải thích](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/yield)
* `ES6` Function* là gì? [giải thích](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function*)
* callback có phải là một phần của V8 hay không ?
* Khác biệt của arrow function là gì ?
* Phân biệt let,const,var khi nào thì dùng nó ?
* Promise trong JS là gì ? 
* Có nên dùng nhiều callback lồng nhau (callback hell) ?

## Hỏi về Testing 

* Có nên sử dụng các công cụ Lint Style hay không? Tại sao?
* Có nên áp dụng unit test hay không ? 
* Bạn có biết về TDD không ? nêu thử 1 vài framework ?

## Hỏi về Performance

* Bạn hay xài công cụ nào để kiểm tra lỗi về hiệu suất tải trên trình duyệt? 
* Giải thích sự khác nhau giữa layout, painting và compositing.

## Hỏi về Network

* Tại sao lưu resource (js/css/...) trên nhiều domain sẽ tốt hơn? 
* Sự khác nhau giữa Long-Polling, Websockets và Server-Sent?
* Giải thích ý nghĩa của mấy cái HTTP Header sau:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
* HTTP action là gì?
* Phân biệt các method HTTP(khi nào thì dùng nó).

## Hỏi về Coding
**Hỏi:** `foo` có giá trị là bao nhiêu?
```js
var foo = 10 + '20';
```

**Hỏi:** Viết hàm `add` để thực hiện được câu lệnh sau:
```js
add(2, 5); // 7
add(2)(5); // 7
```

**Hỏi:** Kết quả trả về của hàm lệnh sau là gì?
```js
"i'm a developer".split("").reverse().join("");
```

**Hỏi:** Giá trị của `window.foo` là gì?
```js
( window.foo || ( window.foo = "bar" ) );
```

**Hỏi:** Kết quả của 2 lệnh `alert` là gì?
```js
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

**Hỏi:** Giá trị của `foo.length` trong trường hợp sau?
```js
var foo = [];
foo.push(1);
foo.push(2);
```

**Hỏi:** Giá trị của `foo.x` trong trường hợp sau?
```js
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

**Hỏi:** Các lệnh sau sẽ in ra console cái gì?
```js
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

**Hỏi:** Các lệnh sau sẽ in ra console cái gì?
```js
baz = function() {
 return "some thing cool";
}
foo = false;
console.log (foo && baz());
console.log (foo || baz());
```

**Hỏi:** Cho `var string = ['1','3','4','10','2','5','9','7','8','6']` in ra kết quả sau
```js
10 9 8 7
6 5 4 
3 2 
1
```

## Hỏi chơi cho vui 

* Những dự án nào mà bạn cho là thú vị đã từng làm qua?
* Bạn hay sử dụng các công cụ (tools) nào? 
* Bạn thích tính năng nào của Internet Explorer nhất?
* Bạn cho biết cách để đo thời gian chạy của một đoạn code javascript, chính xác tới ms?
* Cho 8 viên bi trong đó có 7 viên cùng khối lượng và 1 viên còn lại nặng hơn ? 
* Cho 1 cái cân -|- (kiểu vậy). Làm sao để tìm viên bi nặng hơn nhanh nhất ?
* Cho 2 sợi dây. Đốt 2 sợi dây đó thì mất 1 tiếng. Hỏi trong 45 phút thì làm sao có thể đốt được 2 sợi dây đó.

# How to Contribute
Trang được xây dựng bởi cộng đồng. Để đóng góp vào danh sách câu hỏi, vui lòng: 

1. Fork repo tại Github: [https://github.com/leecris/vn-interview-dev](https://github.com/leecris/vn-interview-dev)
2. Commit câu hỏi trực tiếp vào file README.md, nhánh master.
3. Tạo Pull Request.