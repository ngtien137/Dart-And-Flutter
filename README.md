# Dart And Flutter
## Khai báo biến
* Khai báo biến với kiểu dữ liệu:
```java
  int lineCount1 = 5;
  int lineCount2; // Giá trị mặc định là null
```
* Khai báo biến không cần xác định kiểu dữ liệu:
```kotlin
  var name = 'Bob';
```
* Khai báo biến dynamic: <br>Với loại biến là dynamic, ta có thể coi đây là một loại biến linh động. Khác với var sẽ lấy kiểu dữ liệu ban đầu khi khai báo làm kiểu dữ liệu cho biến, biến dynamic có thể tùy biến kiểu dữ liệu thành các kiểu dữ liệu khác cũng giống với việc ta khai báo 1 dữ liệu là kiểu Object.
```kotlin
  dynamic name = 'Bob';
  name = 5; //Không gây lỗi
  name = 'abc'; //Không gây lỗi
```
* Biến final và const:
<br>Về cơ bản thì chúng đều là hằng số còn cách sử dụng hai biến này vẫn giống với kotlin thôi. Không có gì lạ lẫm hay mới mẻ gì ở đây cả nên sẽ không nói nhiều.
```kotlin
  final name = 'Bob';
  final String name2 = 'Bobby';
  
  const num = 5; 
  const double num2 = 6*num; 
```
## Các kiểu dữ liệu cơ bản
- Number:
<br>Bao gồm 2 kiểu dữ liệu cơ bản là int và double. Ngoài ra giống với kotlin, có thằng cha các kiểu dữ liệu số này là Number thì bên Dart cũng có 1 kiểu dữ liệu cha là num nhưng xịn hơn là num vẫn có thể +,-,/ và * chứ không cùi bắp như Number bên kotlin. Kiểu dữ liệu này có tác dụng gì thì hẳn những người hay viết base sẽ quen hơn còn bình thường cứ dùng thẳng các kiểu dữ liệu con cho rõ ràng.
```
  num count = 0;
  count++;
  num res = count+1;
```
- String:<br>
Giống với kotlin, ta không cần phải cộng chuỗi như java và chèn thêm đô la vào cho nó giàu:
```
  var result = "success";
  var message = "You are $result"; //Hoặc
  var message2 = "You are ${result}"
```
Để tạo ra một string với nhiều dòng, ngoài việc sử dụng "\n", ta có thể sử dụng 3 dấu nháy đơn hoặc 3 dấu nháy đôi chứ không dùng một dấu như ban đầu:
```
  var s1 = '''Line1
    Line2''';
  Hoặc:
  var s2 = """Line1
    Line2""";
```
Khai báo 1 raw string, raw string sẽ không áp dụng những qui luật đặc biệt trong string, ví dụ như nó sẽ bỏ qua "\n" là xuống dòng.
Để khai báo raw string, ta đặt kí tự r ở trước dấu nháy của text:
```
  var s1 = r'Test\nLine2';
  Kết quả:
  'Test\nLine2'
```
- Booleans:

