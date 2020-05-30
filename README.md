# Dart And Flutter
## Khai báo biến
* Khai báo biến với kiểu dữ liệu:
```java
  int lineCount1 = 5;
  int lineCount2; // Giá trị mặc định là null
```
* Khai báo biến không cần xác định kiểu dữ liệu:
```java
  var name = 'Bob';
```
* Khai báo biến dynamic:
Với loại biến là dynamic, ta có thể coi đây là một loại biến linh động. Khác với var sẽ lấy kiểu dữ liệu ban đầu khi khai báo làm kiểu dữ liệu cho biến, biến dynamic có thể tùy biến kiểu dữ liệu thành các kiểu dữ liệu khác cũng giống với việc ta khai báo 1 dữ liệu là kiểu Object.
```java
  dynamic name = 'Bob';
  name = 5; //Không gây lỗi
  name = 'abc'; //Không gây lỗi
```
* Khai báo 
