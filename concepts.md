- [I. Khái niệm cơ bản về lập trình hướng đối tượng (OOP)](#i-khái-niệm-cơ-bản-về-lập-trình-hướng-đối-tượng-oop)
  - [1. Kế thừa và Ghi đè (Inheritance and Overriding)](#1-kế-thừa-và-ghi-đè-inheritance-and-overriding)
    - [1.1. Phân biệt kế thừa và ghi đè áp dụng với thuộc tính và phương thức `final`, `static`, `private`, `Constructors`:](#11-phân-biệt-kế-thừa-và-ghi-đè-áp-dụng-với-thuộc-tính-và-phương-thức-final-static-private-constructors)
    - [1.2. Kế thừa với `class final`](#12-kế-thừa-với-class-final)
    - [1.3. So sánh giữa quan hệ Is-A và Has-A](#13-so-sánh-giữa-quan-hệ-is-a-và-has-a)
  - [2. Phân biệt đa hình và ghi đè](#2-phân-biệt-đa-hình-và-ghi-đè)
    - [1. Ghi đè (Overriding)](#1-ghi-đè-overriding)
    - [2. Đa hình (Polymorphism)](#2-đa-hình-polymorphism)
    - [Bảng so sánh giữa `ghi đè` và `đa hình`](#bảng-so-sánh-giữa-ghi-đè-và-đa-hình)
  - [3. Mối quan hệ giữa instance và kiểu dữ liệu](#3-mối-quan-hệ-giữa-instance-và-kiểu-dữ-liệu)
    - [3.1. Instance của 1 lớp:](#31-instance-của-1-lớp)
    - [3.2. Kiểu dữ liệu:](#32-kiểu-dữ-liệu)
    - [3.3. Bảng so sánh `Instance của 1 lớp` và `Kiểu dữ liệu`](#33-bảng-so-sánh-instance-của-1-lớp-và-kiểu-dữ-liệu)
  - [4. Java Collection Framework](#4-java-collection-framework)
    - [4.1. Tổng quan về Collection Framework](#41-tổng-quan-về-collection-framework)
    - [4.2. List Interface (ArrayList, LinkedList, Vector)](#42-list-interface-arraylist-linkedlist-vector)
    - [4.2.1. Cách xóa phần tử cuối trong LinkedList](#421-cách-xóa-phần-tử-cuối-trong-linkedlist)
    - [4.3. Set Interface (HashSet, LinkedHashSet, TreeSet)](#43-set-interface-hashset-linkedhashset-treeset)
    - [4.4. Map Interface (HashMap, LinkedHashMap, TreeMap)](#44-map-interface-hashmap-linkedhashmap-treemap)
    - [4.4.1. Cơ chế đồng bộ hóa của Map](#441-cơ-chế-đồng-bộ-hóa-của-map)
    - [4.5. Bảng so sánh `List`, `Set`, `Map`](#45-bảng-so-sánh-list-set-map)
  - [5. Phân biệt `String`, `StringBuilder`, và `StringBuffer`](#5-phân-biệt-string-stringbuilder-và-stringbuffer)
  - [6. Lớp lồng nhau (Nested Class)](#6-lớp-lồng-nhau-nested-class)
    - [1. Static Nested Class](#1-static-nested-class)
    - [2. Inner Class (Non-static Nested Class)](#2-inner-class-non-static-nested-class)
    - [3. Local Class](#3-local-class)
    - [4. Anonymous Class](#4-anonymous-class)
    - [Bảng so sánh các loại lớp lồng nhau](#bảng-so-sánh-các-loại-lớp-lồng-nhau)
- [II. Các tính chất và phạm vi](#ii-các-tính-chất-và-phạm-vi)
  - [7. Phạm vi kiểu dữ liệu trong Java](#7-phạm-vi-kiểu-dữ-liệu-trong-java)
  - [7.1. Phân biệt `Member Variable` và `Local Variable`](#71-phân-biệt-member-variable-và-local-variable)
  - [8. Thuộc tính và phương thức ngầm định trong Interface](#8-thuộc-tính-và-phương-thức-ngầm-định-trong-interface)
    - [8.1. Lý do thuộc tính trong interface là `public static final`](#81-lý-do-thuộc-tính-trong-interface-là-public-static-final)
    - [8.2. Lý do phương thức trong interface là `public abstract`](#82-lý-do-phương-thức-trong-interface-là-public-abstract)
  - [9. Phạm vi truy cập (Access Modifiers)](#9-phạm-vi-truy-cập-access-modifiers)
- [III. Lập trình đa luồng (Multithreading)](#iii-lập-trình-đa-luồng-multithreading)
  - [10. Đồng bộ hóa (Synchronization)](#10-đồng-bộ-hóa-synchronization)
    - [10.1. Mục tiêu và cơ chế của Synchronization](#101-mục-tiêu-và-cơ-chế-của-synchronization)
    - [10.2. Synchronized Method](#102-synchronized-method)
    - [10.3. Synchronized Block](#103-synchronized-block)
    - [10.4. Static Synchronization](#104-static-synchronization)
    - [10.5. Đồng bộ hóa của `Collection` (`Map`, `Set`)](#105-đồng-bộ-hóa-của-collection-map-set)
  - [11. Thread (Luồng)](#11-thread-luồng)
    - [11.1. Các trạng thái của `Thread`](#111-các-trạng-thái-của-thread)
    - [11.2. Phân biệt `Concurrency` và `Multithreading`](#112-phân-biệt-concurrency-và-multithreading)
- [IV. File và I/O trong Java](#iv-file-và-io-trong-java)
  - [12. File và I/O](#12-file-và-io)
    - [12.1. Cơ bản về `File`, `InputStream`, `Reader`](#121-cơ-bản-về-file-inputstream-reader)
    - [12.2. Sử dụng `Files.walk`](#122-sử-dụng-fileswalk)
- [V. Quản lý Exception (Ngoại lệ) trong Java](#v-quản-lý-exception-ngoại-lệ-trong-java)
  - [13. Xử lý Exception](#13-xử-lý-exception)
    - [13.1. Tổng quan về Exception và cơ chế xử lý](#131-tổng-quan-về-exception-và-cơ-chế-xử-lý)
    - [13.2. Xử lý Exception trong trường hợp kế thừa (`extends`)](#132-xử-lý-exception-trong-trường-hợp-kế-thừa-extends)
- [VI. Các khái niệm nâng cao trong Java](#vi-các-khái-niệm-nâng-cao-trong-java)
  - [14. Hibernate Annotations](#14-hibernate-annotations)
    - [14.1. Các loại annotation trong Hibernate](#141-các-loại-annotation-trong-hibernate)
  - [15. Date and Time API](#15-date-and-time-api)
  - [16. Stream API và Java Reflection](#16-stream-api-và-java-reflection)
    - [16.1. Tổng quan về `Stream API`](#161-tổng-quan-về-stream-api)
    - [16.2. Java Reflection](#162-java-reflection)
  - [17. Regular Expressions (Biểu thức chính quy)](#17-regular-expressions-biểu-thức-chính-quy)


## I. Khái niệm cơ bản về lập trình hướng đối tượng (OOP)

### 1. Kế thừa và Ghi đè (Inheritance and Overriding)

#### 1.1. Phân biệt kế thừa và ghi đè áp dụng với thuộc tính và phương thức `final`, `static`, `private`, `Constructors`:

| Loại | Kế thừa (Inheritance) | Ghi đè (Overriding) |
| --- | --- | --- |
| Constructors | - Không được kế thừa.<br>- Gọi constructor của lớp cha bằng `super()`. | - Không thể ghi đè.<br>- Constructor của lớp con tách biệt với lớp cha. |
| Static methods | - Được kế thừa (nếu không `private`).<br>- Thuộc về lớp, không phải đối tượng. | - Không thể ghi đè.<br>- Che giấu (hides) phương thức static của lớp cha. |
| Final methods | - Được kế thừa (nếu không `private`).<br>- Có thể sử dụng mà không cần định nghĩa lại. | - Không thể ghi đè.<br>- `final` ngăn chặn việc ghi đè. |
| Private methods | - Không được kế thừa.<br>- Chỉ truy cập trong lớp định nghĩa. | - Không thể ghi đè.<br>- Không thể truy cập từ lớp con. |

(*) Tóm lại:
- Final: Chỉ kế thừa, không ghi đè
- Static: Chỉ kế thừa, không ghi đè nhưng che giấu static lớp cha nếu định nghĩa lại ở lớp con
- Private: Không kế thừa, không ghi đè
- Constructors: Không kế thừa, không ghi đè, nhưng lớp con có thể gọi constructor của lớp cha thông qua `super()`

Tương đương với:
- Chỉ kế thừa với `static` và `final`, còn lại thì không kế thừa với `private`, `Constructors`
- Không ghi đè với tất cả `final`, `static`, `private`, `Constructors`. Ngay kể cả đối với `static` thì nếu có thuộc tính/phương thức ở `static` ở lớp con đặt giống với lớp cha thì là vẫn thuộc của lớp con và che giấu static của lớp cha. Tức là nếu lớp con kế thừa static thuộc tính và phương thức của lớp cha thì sẽ lấy của lớp cha, còn nếu viết lại thuộc tính và phương thức đó ở lớp con thì thuộc tính và phương thức của lớp cha sẽ bị `che giấu/ẩn đi` chứ đang không phải là đang ghi đè. Tóm lại là Ghi đè không bao giờ áp dụng cho các trường hợp là static

```java
class Parent {
    public void instanceMethod() {
        System.out.println("Phương thức instance của lớp cha.");
    }
}

class Child extends Parent {
    public void instanceMethod() {
        System.out.println("Phương thức instance của lớp con.");
    }
}

public class Main {
    public static void main(String[] args) {
        Parent parent = new Parent();
        Parent child = new Child();

        parent.instanceMethod(); // Gọi phương thức instance của lớp cha
        child.instanceMethod();  // Gọi phương thức instance của lớp con (ghi đè)
    }
}
```

`@Override` chỉ là một cách thông báo cho trình biên dịch rằng bạn đang cố tình ghi đè phương thức, và giúp phát hiện lỗi nếu phương thức của lớp con không thực sự ghi đè phương thức của lớp cha nên ngay cả khi không sử dụng `@Override`, Java vẫn hiểu rằng phương thức trong lớp con là một ghi đè phương thức trong lớp cha nếu nó có cùng tên

`@Override` không áp dụng cho static là vì phương thức và thuộc tính static trong Java không bị ghi đè, mà chỉ bị che giấu (hiding). Do đó, từ khóa @Override không thể được sử dụng cho các phương thức hoặc thuộc tính static. `@Override` chỉ có ý nghĩa đối với phương thức instance (non-static), nơi mà hành vi ghi đè có thể xảy ra.

```java
class Parent {
    // Static thuộc tính
    public static int staticVar = 10;

    // Static phương thức
    public static void staticMethod() {
        System.out.println("Phương thức static của lớp cha.");
    }

    // Final phương thức
    public final void finalMethod() {
        System.out.println("Phương thức final của lớp cha.");
    }

    // Private phương thức
    private void privateMethod() {
        System.out.println("Phương thức private của lớp cha.");
    }

    // Constructor
    public Parent() {
        System.out.println("Constructor của lớp cha được gọi.");
    }
}

class Child extends Parent {
    // Static thuộc tính giúp che giấu thuộc tính static của lớp cha
    public static int staticVar = 20;

    // Static phương thức giúp che giấu phương thức static của lớp cha
    public static void staticMethod() {
        System.out.println("Phương thức static của lớp con.");
    }

    // Không thể ghi đè final method
    // public void finalMethod() { ... } // Lỗi biên dịch

    // Constructor
    public Child() {
        super(); // Gọi constructor của lớp cha
        System.out.println("Constructor của lớp con được gọi.");
    }
}

public class Main {
    public static void main(String[] args) {
        // Truy cập phương thức và thuộc tính static thông qua lớp
        System.out.println("Parent.staticVar = " + Parent.staticVar); // Kết quả: 10
        System.out.println("Child.staticVar = " + Child.staticVar);   // Kết quả: 20
        
        Parent.staticMethod(); // Kết quả: Phương thức static của lớp cha.
        Child.staticMethod();  // Kết quả: Phương thức static của lớp con.

        // Khởi tạo đối tượng
        Child child = new Child(); // Gọi cả constructor của lớp cha và con

        // Gọi phương thức final (được kế thừa nhưng không ghi đè được)
        child.finalMethod(); // Kết quả: Phương thức final của lớp cha.
    }
}
```

#### 1.2. Kế thừa với `class final`

`Class final` không thể bị kế thừa (có thể bị nhầm lẫn sang thuộc tính/phương thức `final` có thể kế thừa)

```java
final class FinalClass {}

class SubClass extends FinalClass {
    // Lỗi: không thể kế thừa từ lớp final
}
```

#### 1.3. So sánh giữa quan hệ Is-A và Has-A

| Loại quan hệ | Định nghĩa | Ví dụ | Mục đích |
| --- | --- | --- | --- |
| Is-A | Thể hiện sự kế thừa giữa các lớp. Một lớp con kế thừa từ một lớp cha. | `class Dog extends Animal {}` | Sử dụng để thể hiện mối quan hệ kế thừa, nơi lớp con thừa hưởng các thuộc tính và phương thức của lớp cha. |
| Has-A | Thể hiện quan hệ thành phần giữa các lớp. Một lớp chứa một đối tượng của lớp khác. | `class Car { private Engine engine; }` | Sử dụng để thể hiện mối quan hệ thành phần, nơi một lớp có một hoặc nhiều đối tượng của lớp khác như là thành phần của nó. |

### 2. Phân biệt đa hình và ghi đè

#### 1. Ghi đè (Overriding)
Ghi đè xảy ra khi một lớp con cung cấp cách triển khai lại cho một phương thức đã được định nghĩa trong lớp cha. Khi một phương thức trong lớp con có cùng tên, kiểu trả về và danh sách tham số giống hệt phương thức trong lớp cha, đó là ghi đè.

Mục đích: Ghi đè được dùng để thay thế hoặc mở rộng chức năng của phương thức trong lớp cha.

Điều kiện:
- Phải có quan hệ kế thừa giữa lớp cha và lớp con.
- Phương thức ghi đè phải có cùng tên, cùng kiểu trả về, và cùng tham số.

Kết quả: Khi phương thức được gọi trên đối tượng lớp con, phương thức của lớp con (đã ghi đè) sẽ được thực thi, thay vì phương thức của lớp cha.

#### 2. Đa hình (Polymorphism)
Đa hình là khả năng mà một phương thức có thể thực thi các hành vi khác nhau dựa trên đối tượng gọi phương thức. Đa hình giúp viết mã linh hoạt và có thể thực hiện trên các đối tượng có cùng kiểu nhưng có cách hành xử khác nhau.

Mục đích: Đa hình cho phép gọi cùng một phương thức trên các đối tượng khác nhau nhưng nhận được cách thực hiện khác nhau, tùy thuộc vào kiểu của đối tượng.

Có hai loại đa hình chính:
- Đa hình lúc biên dịch (compile-time polymorphism): Còn gọi là nạp chồng phương thức (method overloading), cho phép gọi nhiều phương thức cùng tên nhưng khác tham số.
- Đa hình lúc chạy (runtime polymorphism): Xảy ra khi ghi đè phương thức, tức là lớp con có thể thay đổi cách triển khai phương thức của lớp cha.

Đa hình lúc chạy chính là khi phương thức ghi đè được gọi trên đối tượng của các lớp khác nhau, với cùng tên phương thức nhưng kết quả khác nhau.

#### Bảng so sánh giữa `ghi đè` và `đa hình`

| Tiêu chí | Ghi đè (Overriding) | Đa hình (Polymorphism) |
| --- | --- | --- |
| Khái niệm | Lớp con thay đổi cách triển khai phương thức của lớp cha. | Một phương thức có thể có nhiều cách thực thi khác nhau dựa trên đối tượng. |
| Phạm vi | Chỉ áp dụng trong quan hệ kế thừa giữa lớp cha và lớp con. | Áp dụng rộng hơn, cả trong kế thừa và thông qua giao diện (interface). |
| Tên và tham số phương thức | Phương thức ghi đè phải có cùng tên và tham số giống hệt với phương thức trong lớp cha. | Cùng tên phương thức, nhưng có thể có các cách triển khai khác nhau ở các lớp khác nhau. |
| Điều kiện thực hiện | Phải có mối quan hệ kế thừa giữa lớp cha và lớp con. | Có thể có quan hệ kế thừa hoặc thông qua giao diện (interface). |
| Mục đích | Thay đổi, mở rộng hoặc bổ sung hành vi của phương thức lớp cha. | Cung cấp nhiều hành vi khác nhau cho cùng một phương thức khi thực hiện trên các đối tượng khác nhau. |
| Cách thực hiện | Lớp con viết lại (ghi đè) phương thức của lớp cha. | Thực hiện cùng một phương thức trên các đối tượng khác nhau, với hành vi cụ thể của từng đối tượng. |
| Loại đa hình | Một hình thức của đa hình lúc chạy (runtime polymorphism). | Gồm cả đa hình lúc biên dịch (compile-time) và lúc chạy (runtime). |
| Ví dụ | Lớp con `Dog` ghi đè phương thức `sound()` của lớp cha `Animal`. | Một mảng đối tượng kiểu `Animal` có cả `Dog` và `Cat`, gọi `sound()` sẽ nhận được hành vi khác nhau tùy đối tượng. |
| Kiểu trả về | Phải giống với kiểu trả về của phương thức trong lớp cha. | Kiểu trả về có thể khác nhau tùy cách triển khai phương thức ở mỗi lớp. |

Tóm lại:
- Ghi đè là một hình thức cụ thể của đa hình trong quan hệ kế thừa, nơi lớp con cung cấp triển khai cụ thể cho phương thức của lớp cha.
- Đa hình là khái niệm rộng hơn, bao gồm cả ghi đè và việc nhiều lớp có thể có các phương thức giống tên nhưng triển khai khác nhau, ví dụ thông qua giao diện (interface).

**Ghi đè:**
```java
class Animal {
    void sound() {
        System.out.println("Some generic animal sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    @Override
    void sound() {
        System.out.println("Meow");
    }
}

// Ghi đè: Dog và Cat ghi đè phương thức sound() từ lớp Animal.
```

**Đa hình:**
```java
Animal animal1 = new Dog();
Animal animal2 = new Cat();

animal1.sound();  // Output: "Bark"
animal2.sound();  // Output: "Meow"

// Đa hình: Cùng gọi phương thức sound() nhưng kết quả khác nhau, dựa trên kiểu đối tượng cụ thể.
```

**Tổng kết:**
- Ghi đè là một trường hợp cụ thể của đa hình, xảy ra trong quan hệ kế thừa. Khi lớp con ghi đè phương thức của lớp cha, đó là đa hình lúc chạy (runtime polymorphism).
- Đa hình là khái niệm tổng quát hơn, bao gồm cả đa hình lúc biên dịch (compile-time, như nạp chồng phương thức) và đa hình lúc chạy (runtime, như ghi đè phương thức).

### 3. Mối quan hệ giữa instance và kiểu dữ liệu

#### 3.1. Instance của 1 lớp:
Instance của một lớp là một đối tượng được tạo ra từ một lớp cụ thể và nó thuộc về lớp mà nó được khởi tạo, bất kể kiểu dữ liệu mà nó đang được tham chiếu.

Khi nói đến instance của một lớp là đang nói về đối tượng thực tế trong bộ nhớ và đối tượng đó luôn giữ các thuộc tính và hành vi của lớp mà nó được khởi tạo từ.

Instance của lớp quyết định đối tượng thực tế trong bộ nhớ và những phương thức hoặc thuộc tính mà đối tượng có thể thực thi (dù thông qua kiểu lớp cha).

Có thể sử dụng instanceof để kiểm tra instance của một lớp

Nếu một đối tượng là instance của một lớp con, nó cũng được coi là instance của tất cả các lớp cha của nó.

```java
class Animal {}

class Dog extends Animal {}

public class Main {
    public static void main(String[] args) {
        Animal animal = new Dog();  // Đối tượng của Dog
        
        if (animal instanceof Dog) { // true
            System.out.println("animal is an instance of Dog");
        }
        
        if (animal instanceof Animal) { // true
            System.out.println("animal is an instance of Animal");
        }
    }
}
```

#### 3.2. Kiểu dữ liệu:
Kiểu dữ liệu là cách mà bạn khai báo một biến để tham chiếu tới đối tượng đó. Kiểu dữ liệu xác định những gì bạn có thể truy cập và cách bạn có thể sử dụng đối tượng trong chương trình.

Trong Java, kiểu dữ liệu có thể là của lớp cha hoặc lớp con, nhưng kiểu dữ liệu này ảnh hưởng đến các thành phần (method, thuộc tính) nào bạn có thể truy cập mà không cần ép kiểu.

```java
class Animal {
    public void eat() {
        System.out.println("Animal is eating");
    }
}

class Dog extends Animal {
    public void bark() {
        System.out.println("Woof");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal dog = new Dog(); // dog là một instance của lớp Dog, nhưng có kiểu dữ liệu là Animal

        dog.eat(); // Hợp lệ: eat() được khai báo trong lớp Animal
        // dog.bark(); // Lỗi biên dịch: bark() không được khai báo trong Animal

        Dog realDog = (Dog) dog; // Đúng vì bản chất thì dog là một instance của lớp Dog nên hoàn toàn ép kiểu được
        realDog.bark(); // Hợp lệ: realDog có kiểu Dog
    }
}
```

#### 3.3. Bảng so sánh `Instance của 1 lớp` và `Kiểu dữ liệu`

| Đặc điểm | Instance của một lớp | Kiểu dữ liệu |
| --- | --- | --- |
| Định nghĩa | Đối tượng cụ thể được tạo ra từ một lớp và tồn tại trong bộ nhớ. | Cách khai báo biến để tham chiếu đến một đối tượng. |
| Mối quan hệ với lớp | Luôn thuộc về lớp mà nó được khởi tạo, bất kể kiểu dữ liệu khai báo. | Có thể là của lớp cha hoặc lớp con, ảnh hưởng đến khả năng truy cập các thành phần. |
| Quyết định | Quyết định đối tượng thực tế trong bộ nhớ và các phương thức/thuộc tính đối tượng có thể thực thi. | Xác định những gì bạn có thể truy cập và cách bạn có thể sử dụng đối tượng. |
| Kiểm tra | Có thể kiểm tra bằng toán tử `instanceof`. | Không có toán tử kiểm tra trực tiếp. |
| Thừa kế | Nếu là instance của lớp con, cũng được coi là instance của tất cả các lớp cha. | Không có tính thừa kế trực tiếp. |
| Ví dụ 1 | `Person person = new Person();` (Ở đây, `person` là một instance của lớp `Person`) | `Person person;` (Ở đây, `Person` là kiểu dữ liệu của biến `person`) |
| Ví dụ 2 | `Animal animal = new Dog();` (Ở đây, `animal` là 1 instance của lớp `Dog` và cũng là 1 instance của lớp `Animal`) | `Animal animal;` (Ở đây, `Animal` là kiểu dữ liệu của biến `animal`) |

**Tóm tắt:**
- Instance là một đối tượng cụ thể, thực tế tồn tại trong bộ nhớ, mang các đặc điểm của lớp mà nó được tạo ra.
- Kiểu dữ liệu là một cách khai báo biến để tham chiếu đến một đối tượng, quyết định cách bạn có thể tương tác với đối tượng đó trong chương trình.

**Lưu ý quan trọng:** Mặc dù một instance luôn thuộc về lớp mà nó được khởi tạo, bạn có thể khai báo một biến với kiểu dữ liệu là lớp cha để tham chiếu đến instance của lớp con (đây là tính đa hình trong Java). Tuy nhiên, điều này sẽ giới hạn khả năng truy cập các thành phần của instance đó chỉ còn các thành phần được định nghĩa trong lớp cha, trừ khi bạn thực hiện ép kiểu.

```java
class Building {
    public void show() {
        System.out.println("This is a building.");
    }
}

class Barn extends Building {
    public void show() {
        System.out.println("This is a barn.");
    }

    public void storeHay() {
        System.out.println("Storing hay in the barn.");
    }
}

public class Main {
    public static void main(String[] args) {
        // build1 là 1 instance của lớp Building
        Building build1 = new Building(); 
        build1.show(); // Kết quả: "This is a building."

        // build2 là 1 instance của lớp Barn
        Building build2 = new Barn(); 
        build2.show(); // Kết quả: "This is a barn." (đa hình - phương thức của Barn được gọi)

        // Barn barn1 = (Barn) build1; / Lỗi ClassCastException sẽ xảy ra tại thời điểm chạy vì build1 là instance của class Building, không phải là 1 instance của lớp Barn
        try {
            Barn barn1 = (Barn) build1; // Lỗi ClassCastException sẽ xảy ra
        } catch (ClassCastException e) {
             System.out.println("Exception: build1 không thể ép kiểu thành Barn vì build1 là instance của Building.");
        }

        // Barn barn2 = (Barn) build2; // Đúng vì build2 là 1 instance của lớp Barn
        Barn barn2 = (Barn) build2;
        barn2.show(); // Kết quả: "This is a barn."
        barn2.storeHay(); // Kết quả: "Storing hay in the barn."

        // Barn barn3 = new Barn();
        Barn barn3 = new Barn(); // Tạo một instance của Barn

        // Building build3 = (Building) barn3; // Đúng vì ép từ kiểu con sang kiểu cha không cần ép kiểu tường minh
        Building build3 = barn3;
        build3.show(); // Kết quả: "This is a barn." (vì build3 thực sự là instance của Barn)

        // Object obj1 = (Object) build1;
        Object obj1 = build1; // Tất cả các đối tượng đều có thể được ép kiểu sang Object mà không cần ép kiểu tường minh
        System.out.println("obj1 is instance of Object: " + (obj1 instanceof Object)); // Kết quả: true
    }
}
```

### 4. Java Collection Framework

#### 4.1. Tổng quan về Collection Framework

```
Java Collection Framework
├── Iterable
│   └── Collection
│       ├── List (Interface)
│       │   ├── ArrayList
│       │   ├── LinkedList
│       │   └── Vector
│       │       └── Stack
│       ├── Set (Interface)
│       │   ├── HashSet
│       │   ├── LinkedHashSet
│       │   └── TreeSet
│       ├── Queue (Interface)
│       │   ├── PriorityQueue
│       │   └── LinkedList (also implements Queue)
│       └── Deque (Interface)
│           ├── ArrayDeque
│           └── LinkedList (also implements Deque)
└── Map (Interface) (doesn't extend Collection)
    ├── HashMap
    ├── LinkedHashMap
    ├── TreeMap
    └── Hashtable
        └── Properties
```

#### 4.2. List Interface (ArrayList, LinkedList, Vector)

**List (Interface)** // Các implement từ List Interface (ArrayList, LinkedList, Vector) đều có chung các phương thức này:
- `add()`          // Thêm phần tử vào cuối danh sách
- `get()`          // Lấy phần tử theo chỉ số
- `set()`          // Cập nhật phần tử tại chỉ số cụ thể
- `remove()`       // Xóa phần tử theo chỉ số hoặc đối tượng
- `size()`         // Trả về số lượng phần tử trong danh sách
- `contains()`     // Kiểm tra xem danh sách có chứa phần tử chỉ định
- `indexOf()`      // Tìm vị trí của phần tử đầu tiên xuất hiện trong danh sách
- `clear()`        // Xóa tất cả các phần tử trong danh sách
- `isEmpty()`      // Kiểm tra xem danh sách có rỗng không
- `subList()`      // Trả về danh sách con từ vị trí chỉ định

| Đặc điểm | ArrayList | LinkedList | Vector |
| --- | --- | --- | --- |
| Cấu trúc dữ liệu | Mảng động | Danh sách liên kết | Mảng động |
| Truy cập phần tử | Nhanh (O(1)) | Chậm (O(n)) | Nhanh (O(1)) |
| Thêm/xóa phần tử ở giữa | Chậm (O(n)) | Nhanh (O(1)) | Chậm (O(n)) |
| Sử dụng bộ nhớ | Ít hơn | Nhiều hơn | Ít hơn |
| Đồng bộ (Synchronized) | Không | Không | Có |
| Thread-safe | Không | Không | Có |
| Thích hợp cho | Truy cập ngẫu nhiên | Thêm/xóa phần tử thường xuyên | Ứng dụng đa luồng cần thread-safe |

#### 4.2.1. Cách xóa phần tử cuối trong LinkedList

Để xóa phần tử cuối trong LinkedList, có hai cách chính:

1. Sử dụng phương thức `removeLast()`:
```java
LinkedList<String> list = new LinkedList<>();
list.add("A");
list.add("B");
list.add("C");
list.removeLast(); // Xóa phần tử cuối cùng ("C")
```

2. Sử dụng phương thức `remove()` với chỉ số:
```java
LinkedList<String> list = new LinkedList<>();
list.add("A");
list.add("B");
list.add("C");
if (!list.isEmpty()) {
    list.remove(list.size() - 1); // Xóa phần tử cuối cùng
}
```

Cách 1 (`removeLast()`) hiệu quả hơn vì LinkedList được triển khai dưới dạng danh sách liên kết đôi, nên việc truy cập vào phần tử cuối là O(1). Trong khi đó, cách 2 cần phải duyệt đến phần tử cuối cùng nên có độ phức tạp O(n).

#### 4.3. Set Interface (HashSet, LinkedHashSet, TreeSet)

**Set (Interface)** // Các implement từ Set Interface (HashSet, LinkedHashSet, TreeSet) đều có chung các phương thức này:
- `add()`            // Thêm phần tử vào Set (không thêm nếu đã tồn tại)
- `remove()`         // Xóa phần tử khỏi Set
- `contains()`       // Kiểm tra xem phần tử có tồn tại trong Set không
- `size()`           // Trả về số lượng phần tử trong Set
- `isEmpty()`        // Kiểm tra xem Set có rỗng không
- `clear()`          // Xóa tất cả các phần tử trong Set
- `addAll()`         // Thêm tất cả phần tử từ Collection khác vào Set
- `removeAll()`      // Xóa các phần tử trong Set có trong Collection khác
- `retainAll()`      // Giữ lại các phần tử có trong cả Set và Collection khác
- `toArray()`        // Chuyển Set thành mảng

| Đặc điểm | HashSet | LinkedHashSet | TreeSet |
| --- | --- | --- | --- |
| Cấu trúc dữ liệu | Bảng băm (Hash Table) | Bảng băm + Danh sách liên kết doubly | Cây đỏ-đen (Red-Black Tree) |
| Thứ tự phần tử | Không đảm bảo thứ tự | Duy trì thứ tự thêm phần tử | Duy trì thứ tự tăng dần của phần tử |
| Độ phức tạp thêm/xóa/kiểm tra phần tử | O(1) (trung bình) | O(1) (trung bình) | O(log n) |
| Độ phức tạp duyệt (iteration) | O(n) | O(n) | O(n) |
| Sử dụng bộ nhớ | Ít hơn | Nhiều hơn (do lưu thêm thông tin về thứ tự) | Nhiều hơn (do cấu trúc cây phức tạp) |
| Thích hợp cho | Ứng dụng cần lưu trữ phần tử duy nhất, không quan tâm thứ tự | Ứng dụng cần duy trì thứ tự thêm phần tử | Ứng dụng cần duy trì thứ tự của phần tử |

```java
import java.util.HashSet;
import java.util.LinkedHashSet;
import java.util.TreeSet;

public class Main {
    public static void main(String[] args) {
        HashSet<String> hashSet = new HashSet<>();
        hashSet.add("B");
        hashSet.add("A");
        hashSet.add("C");
        System.out.println("HashSet: " + hashSet); // HashSet: [A, B, C] -> Thứ tự không được đảm bảo

        LinkedHashSet<String> linkedHashSet = new LinkedHashSet<>();
        linkedHashSet.add("B");
        linkedHashSet.add("A");
        linkedHashSet.add("C");
        System.out.println("LinkedHashSet: " + linkedHashSet); // LinkedHashSet: [B, A, C] -> Duy trì thứ tự thêm vào

        TreeSet<String> treeSet = new TreeSet<>();
        treeSet.add("B");
        treeSet.add("A");
        treeSet.add("C");
        System.out.println("TreeSet: " + treeSet); // TreeSet: [A, B, C] -> Duy trì thứ tự tự nhiên (alphabet)
    }
}
```

**Giải thích:**
- Tương tự như Map, Set cũng có ba lớp con phổ biến là `HashSet`, `LinkedHashSet`, và `TreeSet`.
- `HashSet` sử dụng `HashMap` để lưu trữ dữ liệu, do đó nó cũng cung cấp hiệu năng cao nhưng không đảm bảo thứ tự phần tử.
- `LinkedHashSet` kế thừa từ `HashSet` và sử dụng doubly-linked list để duy trì thứ tự thêm vào.
- `TreeSet` dựa trên `TreeMap` và lưu trữ các phần tử theo thứ tự được sắp xếp.

**Lựa chọn lớp con phù hợp:**
- Nếu bạn cần hiệu năng cao và không quan tâm đến thứ tự phần tử, hãy sử dụng `HashSet`.
- Nếu bạn cần duy trì thứ tự thêm vào, hãy sử dụng `LinkedHashSet`.
- Nếu bạn cần duy trì thứ tự được sắp xếp, hãy sử dụng `TreeSet`.

#### 4.4. Map Interface (HashMap, LinkedHashMap, TreeMap)

**Map (Interface)** // Các implement từ Map Interface (HashMap, LinkedHashMap, TreeMap) đều có chung các phương thức này:
- `put()`            // Thêm hoặc cập nhật cặp key-value
- `get()`            // Lấy giá trị dựa trên khóa
- `remove()`         // Xóa cặp key-value dựa trên khóa
- `containsKey()`    // Kiểm tra xem có khóa cụ thể trong map không
- `containsValue()`  // Kiểm tra xem có giá trị cụ thể trong map không
- `size()`           // Trả về số lượng cặp key-value trong map
- `isEmpty()`        // Kiểm tra xem map có rỗng không
- `clear()`          // Xóa tất cả các cặp key-value trong map
- `keySet()`         // Trả về tập hợp các khóa có trong map
- `values()`         // Trả về tập hợp các giá trị có trong map
- `entrySet()`       // Trả về tập hợp các cặp key-value dưới dạng Set

| Đặc điểm | HashMap | LinkedHashMap | TreeMap |
| --- | --- | --- | --- |
| Cấu trúc dữ liệu | Bảng băm (Hash Table) | Bảng băm + Danh sách liên kết doubly | Cây đỏ-đen (Red-Black Tree) |
| Thứ tự phần tử | Không đảm bảo thứ tự | Duy trì thứ tự thêm phần tử | Duy trì thứ tự tăng dần của key |
| Độ phức tạp truy cập (get/put) | O(1) (trung bình) | O(1) (trung bình) | O(log n) |
| Độ phức tạp duyệt (iteration) | O(n) | O(n) | O(n) |
| Sử dụng bộ nhớ | Ít hơn | Nhiều hơn (do lưu thêm thông tin về thứ tự) | Nhiều hơn (do cấu trúc cây phức tạp) |
| Thích hợp cho | Ứng dụng cần truy cập nhanh, không quan tâm thứ tự | Ứng dụng cần duy trì thứ tự thêm phần tử | Ứng dụng cần duy trì thứ tự của key |

```java
import java.util.HashMap;
import java.util.LinkedHashMap;
import java.util.TreeMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, Integer> hashMap = new HashMap<>();
        hashMap.put("B", 2);
        hashMap.put("A", 1);
        hashMap.put("C", 3);
        System.out.println("HashMap: " + hashMap); // HashMap: {A=1, B=2, C=3} -> Thứ tự không được đảm bảo

        LinkedHashMap<String, Integer> linkedHashMap = new LinkedHashMap<>();
        linkedHashMap.put("B", 2);
        linkedHashMap.put("A", 1);
        linkedHashMap.put("C", 3);
        System.out.println("LinkedHashMap: " + linkedHashMap); // LinkedHashMap: {B=2, A=1, C=3} -> Duy trì thứ tự thêm vào

        TreeMap<String, Integer> treeMap = new TreeMap<>();
        treeMap.put("B", 2);
        treeMap.put("A", 1);
        treeMap.put("C", 3);
        System.out.println("TreeMap: " + treeMap); // TreeMap: {A=1, B=2, C=3} -> Duy trì thứ tự tự nhiên (alphabet)
    }
}
```

#### 4.4.1. Cơ chế đồng bộ hóa của Map

Trong Java, có nhiều cách để tạo Map đồng bộ (thread-safe):

1. **Hashtable**: Lớp cũ, tất cả các phương thức đều được đồng bộ hóa.
   ```java
   Map<String, Integer> hashtable = new Hashtable<>();
   ```
   - Ưu điểm: Đơn giản, thread-safe
   - Nhược điểm: Hiệu suất thấp vì đồng bộ hóa toàn bộ map, không cho phép giá trị null

2. **Collections.synchronizedMap()**: Chuyển đổi một Map không đồng bộ thành Map đồng bộ.
   ```java
   Map<String, Integer> synchronizedMap = Collections.synchronizedMap(new HashMap<>());
   ```
   - Ưu điểm: Linh hoạt, có thể sử dụng với bất kỳ Map nào
   - Nhược điểm: Vẫn đồng bộ hóa toàn bộ map, hiệu suất không cao

3. **ConcurrentHashMap**: Được thiết kế đặc biệt cho môi trường đa luồng.
   ```java
   ConcurrentHashMap<String, Integer> concurrentHashMap = new ConcurrentHashMap<>();
   ```
   - Ưu điểm: Hiệu suất cao, chia nhỏ lock thành nhiều segment, không khóa toàn bộ map
   - Nhược điểm: Triển khai phức tạp hơn

**So sánh hiệu suất:**
- ConcurrentHashMap > Hashtable > SynchronizedMap
- ConcurrentHashMap cho phép nhiều luồng đọc đồng thời và số lượng luồng ghi được giới hạn bởi số lượng segment (mặc định là 16)

**Ví dụ sử dụng ConcurrentHashMap:**
```java
import java.util.concurrent.ConcurrentHashMap;

public class ConcurrentMapExample {
    public static void main(String[] args) {
        ConcurrentHashMap<String, Integer> map = new ConcurrentHashMap<>();
        
        // Các thao tác an toàn với đa luồng
        map.put("A", 1);
        map.put("B", 2);
        
        // Đọc an toàn
        System.out.println(map.get("A"));
        
        // Cập nhật an toàn
        map.compute("A", (key, value) -> value != null ? value + 1 : 1);
    }
}
```

**Lưu ý quan trọng:**
- Khi sử dụng các phương thức duyệt (như keySet(), values(), entrySet()), cần sử dụng synchronized block nếu cần đảm bảo tính toàn vẹn:
  ```java
  synchronized (map) {
      for (Map.Entry<String, Integer> entry : map.entrySet()) {
          // Xử lý
      }
  }
  ```
- ConcurrentHashMap cung cấp các phương thức nguyên tử như `putIfAbsent()`, `compute()`, `merge()` giúp xử lý an toàn trong môi trường đa luồng.

#### 4.5. Bảng so sánh `List`, `Set`, `Map`

Dưới đây là bảng so sánh với dấu `x` cho những phương thức không được hỗ trợ

| Phương thức | List | Map | Set |
| --- | --- | --- | --- |
| Thêm | `add(E element)` | `put(K key, V value)` | `add(E element)` |
| Sửa | `set(int index, E element)` | `put(K key, V value)` | x |
| Xóa | `remove(int index)` | `remove(Object key)` | `remove(Object o)` |
| Truy cập | `get(int index)` | `get(Object key)` | x |
| Kiểm tra phần tử | `contains(Object o)` | `containsKey(Object key)`, `containsValue(Object value)` | `contains(Object o)` |
| Kích thước | `size()` | `size()` | `size()` |
| Kiểm tra rỗng | `isEmpty()` | `isEmpty()` | `isEmpty()` |
| Xóa tất cả | `clear()` | `clear()` | `clear()` |
| Trả về tập hợp con | `subList(int fromIndex, int toIndex)` | `entrySet()`, `keySet()`, `values()` | `toArray()` |
| Chỉ số hoặc khóa | `indexOf(Object o)` | `keySet()` | x |
| Tập hợp các phần tử | x | `entrySet()`, `keySet()`, `values()` | x |
| Thêm tập hợp | x | x | `addAll(Collection<? extends E> c)` |
| Xóa tập hợp | x | x | `removeAll(Collection<?> c)` |
| Giữ lại phần tử | x | x | `retainAll(Collection<?> c)` |

**Giải thích chi tiết:**
- **List**: Cho phép thêm, sửa, xóa và truy cập các phần tử theo chỉ số. Không hỗ trợ các thao tác tập hợp (addAll, removeAll, retainAll) và không có khái niệm về khóa.
- **Map**: Quản lý các cặp key-value và hỗ trợ các phương thức liên quan đến khóa và giá trị. Không hỗ trợ truy cập theo chỉ số và các thao tác tập hợp.
- **Set**: Cho phép thêm, xóa và kiểm tra phần tử duy nhất, không hỗ trợ truy cập trực tiếp qua chỉ số hay khóa. Hỗ trợ các thao tác tập hợp như `addAll`, `removeAll`, `retainAll`.

### 5. Phân biệt `String`, `StringBuilder`, và `StringBuffer`

| Đặc điểm | String | StringBuffer | StringBuilder |
| --- | --- | --- | --- |
| Tính chất | Immutable (không thay đổi được) | Mutable (thay đổi được) | Mutable (thay đổi được) |
| Thread safety | Thread-safe (vì immutable) | Thread-safe (sử dụng synchronized) | Không thread-safe |
| Hiệu suất | Thấp khi thực hiện nhiều thao tác nối chuỗi | Trung bình | Cao nhất |
| Sử dụng bộ nhớ | Tốn nhiều bộ nhớ khi thực hiện nhiều thao tác nối chuỗi | Tiết kiệm bộ nhớ hơn String | Tiết kiệm bộ nhớ nhất |
| Kế thừa | Không kế thừa từ bất kỳ lớp nào | Kế thừa từ Object | Kế thừa từ Object |
| Triển khai | Không triển khai interface nào đặc biệt | Triển khai CharSequence, Appendable | Triển khai CharSequence, Appendable |
| Phiên bản giới thiệu | Java 1.0 | Java 1.0 | Java 1.5 |

**Giải thích chi tiết:**

- **String**: 
  - Là lớp final, không thể kế thừa
  - Một khi được tạo, giá trị không thể thay đổi (immutable)
  - Khi thực hiện các phép nối chuỗi, một đối tượng String mới sẽ được tạo ra
  - Tốt cho các chuỗi không thay đổi nhiều
  - Ví dụ: `String str = "Hello" + " World";` tạo ra 3 đối tượng String

- **StringBuffer**:
  - Có thể thay đổi giá trị (mutable)
  - Tất cả các phương thức thay đổi nội dung đều được đồng bộ hóa (synchronized)
  - An toàn khi sử dụng trong môi trường đa luồng
  - Hiệu suất thấp hơn StringBuilder do phải xử lý đồng bộ hóa
  - Ví dụ: 
    ```java
    StringBuffer sb = new StringBuffer("Hello");
    sb.append(" World"); // Không tạo đối tượng mới
    ```

- **StringBuilder**:
  - Có thể thay đổi giá trị (mutable)
  - Không được đồng bộ hóa, không an toàn trong môi trường đa luồng
  - Hiệu suất cao hơn StringBuffer
  - Nên sử dụng khi không làm việc với đa luồng
  - Ví dụ:
    ```java
    StringBuilder sb = new StringBuilder("Hello");
    sb.append(" World"); // Không tạo đối tượng mới
    ```

**Khi nào nên sử dụng cái nào?**
- Sử dụng **String** khi:
  - Chuỗi không thay đổi
  - Không thực hiện nhiều thao tác nối chuỗi
  - Cần sử dụng như khóa trong Map

- Sử dụng **StringBuffer** khi:
  - Cần thay đổi chuỗi
  - Làm việc trong môi trường đa luồng
  - Cần đảm bảo thread safety

- Sử dụng **StringBuilder** khi:
  - Cần thay đổi chuỗi
  - Không làm việc trong môi trường đa luồng
  - Cần hiệu suất cao nhất

**Ví dụ so sánh hiệu suất:**
```java
public class StringPerformanceTest {
    public static void main(String[] args) {
        long startTime = System.currentTimeMillis();
        
        // Sử dụng String
        String str = "";
        for (int i = 0; i < 10000; i++) {
            str += "a";
        }
        System.out.println("String: " + (System.currentTimeMillis() - startTime) + "ms");
        
        // Sử dụng StringBuffer
        startTime = System.currentTimeMillis();
        StringBuffer sb = new StringBuffer();
        for (int i = 0; i < 10000; i++) {
            sb.append("a");
        }
        System.out.println("StringBuffer: " + (System.currentTimeMillis() - startTime) + "ms");
        
        // Sử dụng StringBuilder
        startTime = System.currentTimeMillis();
        StringBuilder sbl = new StringBuilder();
        for (int i = 0; i < 10000; i++) {
            sbl.append("a");
        }
        System.out.println("StringBuilder: " + (System.currentTimeMillis() - startTime) + "ms");
    }
}
```
Kết quả thường cho thấy StringBuilder nhanh nhất, tiếp theo là StringBuffer, và String chậm nhất khi thực hiện nhiều thao tác nối chuỗi.

### 6. Lớp lồng nhau (Nested Class)

Trong Java, có 4 loại lớp lồng nhau:

#### 1. Static Nested Class
- Được khai báo với từ khóa `static`
- Không có tham chiếu ẩn đến instance của lớp bên ngoài
- Có thể được khởi tạo mà không cần instance của lớp bên ngoài
- Chỉ có thể truy cập các thành phần static của lớp bên ngoài

```java
public class OuterClass {
    private static String staticMessage = "Static Message";
    
    public static class StaticNestedClass {
        void display() {
            System.out.println(staticMessage);
            // Không thể truy cập non-static members của OuterClass
        }
    }
    
    public static void main(String[] args) {
        OuterClass.StaticNestedClass nested = new OuterClass.StaticNestedClass();
        nested.display();
    }
}
```

#### 2. Inner Class (Non-static Nested Class)
- Không có từ khóa `static`
- Có tham chiếu ẩn đến instance của lớp bên ngoài
- Phải được khởi tạo thông qua instance của lớp bên ngoài
- Có thể truy cập tất cả các thành phần của lớp bên ngoài

```java
public class OuterClass {
    private String message = "Hello from OuterClass";
    
    public class InnerClass {
        void display() {
            System.out.println(message); // Có thể truy cập thành phần private của OuterClass
        }
    }
    
    public static void main(String[] args) {
        OuterClass outer = new OuterClass();
        OuterClass.InnerClass inner = outer.new InnerClass();
        inner.display();
    }
}
```

#### 3. Local Class
- Được khai báo bên trong một phương thức
- Chỉ có thể truy cập các biến final hoặc effectively final của phương thức chứa nó
- Không có access modifier (public, private, v.v.)

```java
public class OuterClass {
    public void createLocalClass() {
        final String message = "Hello from LocalClass";
        
        class LocalClass {
            void display() {
                System.out.println(message);
            }
        }
        
        LocalClass local = new LocalClass();
        local.display();
    }
    
    public static void main(String[] args) {
        new OuterClass().createLocalClass();
    }
}
```

#### 4. Anonymous Class
- Lớp không tên, được khai báo và khởi tạo cùng một lúc
- Thường được sử dụng để ghi đè phương thức của lớp cha hoặc interface
- Chỉ có thể truy cập các biến final hoặc effectively final

```java
public class OuterClass {
    public void createAnonymousClass() {
        final String message = "Hello from AnonymousClass";
        
        // Anonymous class implementing Runnable
        Runnable runnable = new Runnable() {
            @Override
            public void run() {
                System.out.println(message);
            }
        };
        
        new Thread(runnable).start();
    }
    
    public static void main(String[] args) {
        new OuterClass().createAnonymousClass();
    }
}
```

#### Bảng so sánh các loại lớp lồng nhau

| Đặc điểm | Static Nested Class | Inner Class | Local Class | Anonymous Class |
| --- | --- | --- | --- | --- |
| Từ khóa static | Có | Không | Không áp dụng | Không áp dụng |
| Truy cập thành phần non-static của lớp bên ngoài | Không | Có | Có | Có |
| Khởi tạo mà không cần instance lớp bên ngoài | Có | Không | Không | Không |
| Được khai báo bên trong phương thức | Không | Không | Có | Có |
| Có tên | Có | Có | Có | Không |
| Mục đích chính | Tổ chức code, nhóm các lớp liên quan | Truy cập trực tiếp vào instance của lớp bên ngoài | Định nghĩa lớp cục bộ cho một phương thức | Triển khai nhanh interface hoặc lớp trừu tượng |

**Lưu ý quan trọng:**
- Inner class giữ một tham chiếu ẩn đến instance của lớp bên ngoài, có thể gây rò rỉ bộ nhớ nếu không cẩn thận
- Static nested class không giữ tham chiếu đến instance của lớp bên ngoài, thường được ưa chuộng hơn để tránh vấn đề rò rỉ bộ nhớ
- Local class và anonymous class thường được sử dụng cho các trường hợp đơn giản, ngắn gọn

---

## II. Các tính chất và phạm vi

### 7. Phạm vi kiểu dữ liệu trong Java

| Kiểu dữ liệu | Kích thước | Giá trị nhỏ nhất | Giá trị lớn nhất | Giá trị mặc định |
| --- | --- | --- | --- | --- |
| boolean | 1-bit | false | true | false |
| byte | 8-bit | -128 | 127 | 0 |
| short | 16-bit | -32,768 | 32,767 | 0 |
| char | 16-bit | 0 | 65,535 (biểu diễn Unicode) | \u0000 (null) |
| int | 32-bit | -2^31 (-2,147,483,648) | 2^31 - 1 (2,147,483,647) | 0 |
| float | 32-bit | ~1.4E-45 | ~3.4E+38 | 0.0F |
| long | 64-bit | -2^63 (-9,223,372,036,854,775,808) | 2^63 - 1 (9,223,372,036,854,775,807) | 0L |
| double | 64-bit | ~4.9E-324 | ~1.7E+308 | 0.0D |

```java
public class MyClass {
    boolean data; // Giá trị mặc định là false
    byte data; // Giá trị mặc định là 0
    short data; // Giá trị mặc định là 0
    char data; // Giá trị mặc định là \u0000 hoặc '\0'
    int data; // Giá trị mặc định là 0
    float data; // Giá trị mặc định là 0.0F
    long data; // Giá trị mặc định là 0L
    double data; // Giá trị mặc định là 0.0D
}
```

### 7.1. Phân biệt `Member Variable` và `Local Variable`

| Đặc điểm | Member Variable | Local Variable |
| --- | --- | --- |
| Vị trí khai báo | Trong lớp nhưng ngoài phương thức | Trong phương thức, constructor hoặc khối lệnh |
| Thời điểm khởi tạo | Khi đối tượng được tạo | Khi phương thức được gọi |
| Phạm vi | Toàn bộ lớp | Chỉ trong khối lệnh khai báo |
| Giá trị mặc định | Có giá trị mặc định (0, false, null) | Không có giá trị mặc định |
| Khởi tạo bắt buộc | Không cần khởi tạo trước khi sử dụng | Phải khởi tạo trước khi sử dụng |
| Bộ nhớ | Được lưu trong heap | Được lưu trong stack |
| Ví dụ | `private int age;` | `int count = 0;` |

**Giải thích chi tiết:**

**Biến thành viên (Member Variables):**
- Được khai báo trong lớp nhưng bên ngoài bất kỳ phương thức, constructor hoặc khối lệnh nào
- Có giá trị mặc định nếu không được khởi tạo:
  - Kiểu số nguyên (byte, short, int, long): Giá trị mặc định là 0
  - Kiểu số thực (float, double): Giá trị mặc định là 0.0
  - Kiểu ký tự (char): Giá trị mặc định là ký tự '\u0000' (null character)
  - Kiểu boolean: Giá trị mặc định là false
  - Kiểu tham chiếu (như String, Object): Giá trị mặc định là null

```java
public class Person {
    private int age;          // giá trị mặc định là 0
    private boolean isStudent;   // giá trị mặc định là false
    private String name;     // giá trị mặc định là null
    
    public void printDetails() {
        System.out.println("Age: " + age);
        System.out.println("Is Student: " + isStudent);
        System.out.println("Name: " + name);
    }
}
```

**Biến cục bộ (Local Variables):**
- Được khai báo bên trong phương thức, constructor hoặc khối lệnh
- Không có giá trị mặc định, phải được khởi tạo trước khi sử dụng
- Nếu cố gắng sử dụng mà chưa khởi tạo sẽ gây lỗi biên dịch

```java
public class Calculator {
    public int add(int a, int b) {
        int result = a + b; // Biến cục bộ, phải được khởi tạo
        return result;
    }
    
    public void print() {
        int value; // Khai báo biến cục bộ
        // System.out.println(value); // Lỗi biên dịch: variable might not have been initialized
        value = 10; // Khởi tạo trước khi sử dụng
        System.out.println(value); // Hợp lệ
    }
}
```

**Biến tĩnh (Static Variables):**
- Được khai báo với từ khóa `static`
- Thuộc về lớp, không thuộc về instance
- Có giá trị mặc định tương tự như member variables

```java
public class Counter {
    private static int totalCount = 0; // Biến tĩnh
    
    public Counter() {
        totalCount++;
    }
    
    public static int getTotalCount() {
        return totalCount;
    }
}
```

**Lưu ý quan trọng:**
- Biến cục bộ chỉ tồn tại trong thời gian thực thi phương thức/bloch lệnh
- Biến thành viên tồn tại suốt đời của đối tượng
- Biến tĩnh tồn tại suốt đời của chương trình
- Tên biến cục bộ có thể giống với tên biến thành viên, khi đó cần dùng `this` để truy cập biến thành viên

### 8. Thuộc tính và phương thức ngầm định trong Interface

#### 8.1. Lý do thuộc tính trong interface là `public static final`

Các thuộc tính trong interface được mặc định là `public static final` vì:

- `public`: Các hằng số trong interface cần được truy cập từ bất kỳ lớp nào implement interface đó, cũng như từ các lớp khác.
- `static`: Các hằng số này thuộc về interface, chứ không thuộc về các instance của interface (interface không thể được khởi tạo).
- `final`: Các hằng số không được phép thay đổi giá trị sau khi được gán. Việc này đảm bảo tính nhất quán và tránh lỗi.

**Mệnh đề:** "Tất cả các biến là `static` và phương thức là `public` nếu interface được định nghĩa là `public`"
→ Đây là một mệnh đề sai.

**Giải thích:**
Trong Java, các thuộc tính (biến) trong `interface` luôn có các đặc tính:
- `public static final` (công khai, tĩnh, hằng số).

Các phương thức trong `interface` luôn có các đặc tính:
- `public abstract` (công khai và trừu tượng).

Điều này đúng bất kể `interface` được khai báo là `public` hay `private`. Ngay cả khi `interface` là `private`, các thuộc tính và phương thức trong đó vẫn tuân theo quy tắc này.

**Các cách viết sau là tương đương:**
```java
public interface MyInterface {
    // Thuộc tính 
    int MAX_VALUE = 100;
    public int MAX_VALUE = 100;
    final int MAX_VALUE = 100;
    static int MAX_VALUE = 100;
    public static final int MAX_VALUE = 100;
    public final static int MAX_VALUE = 100;
    static final int MAX_VALUE = 100;
    final static int MAX_VALUE = 100;
    
    // Phương thức
    void doSomething();
    public abstract void doSomething();
    public void doSomething();
    abstract void doSomething();
}
```

#### 8.2. Lý do phương thức trong interface là `public abstract`

Các phương thức trong interface được mặc định là `public abstract` vì việc này buộc các lớp implement interface phải cung cấp triển khai cụ thể cho các phương thức đó.

### 9. Phạm vi truy cập (Access Modifiers)

| Modifier | Truy cập trong cùng lớp | Truy cập trong cùng package | Truy cập từ lớp con (khác package) | Truy cập từ mọi nơi |
| --- | --- | --- | --- | --- |
| public | ✔ | ✔ | ✔ | ✔ |
| protected | ✔ | ✔ | ✔ | ✘ |
| (default) | ✔ | ✔ | ✘ | ✘ |
| private | ✔ | ✘ | ✘ | ✘ |

```java
public class MyClass {
    public int publicData = 1; // Truy cập từ mọi nơi
    protected int protectedData = 2; // Truy cập trong cùng package và lớp con
    int defaultData = 3; // Truy cập trong cùng package
    private int privateData = 4; // Truy cập chỉ trong lớp MyClass

    public void publicMethod() {} // Truy cập từ mọi nơi
    protected void protectedMethod() {} // Truy cập trong cùng package và lớp con
    void defaultMethod() {} // Truy cập trong cùng package
    private void privateMethod() {} // Truy cập chỉ trong lớp MyClass
}

class AnotherClass {
    // Trong cùng package
    public void accessData(MyClass obj) {
        System.out.println(obj.publicData); 
        System.out.println(obj.protectedData); 
        System.out.println(obj.defaultData); 
        // System.out.println(obj.privateData); // Lỗi: không truy cập được
    }
}

class SubClass extends MyClass {
    // Lớp con (khác package)
    public void accessData() {
        System.out.println(publicData);
        System.out.println(protectedData); 
        // System.out.println(defaultData); // Lỗi: không truy cập được
        // System.out.println(privateData); // Lỗi: không truy cập được
    }
}
```

---

## III. Lập trình đa luồng (Multithreading)

### 10. Đồng bộ hóa (Synchronization)

#### 10.1. Mục tiêu và cơ chế của Synchronization

**Mục tiêu:** Đảm bảo rằng chỉ có một luồng (thread) có thể thực thi một phương thức hoặc khối mã cụ thể tại một thời điểm trên một đối tượng hoặc lớp nhất định.

**Cơ chế:**
- Khi một luồng đang thực thi một đoạn mã được đồng bộ hóa (bằng `synchronized`), các luồng khác phải đợi cho đến khi luồng đó hoàn tất trước khi có thể vào đoạn mã này.
- `Synchronized` sử dụng khái niệm khóa (lock) để kiểm soát truy cập. Mỗi đối tượng và lớp trong Java đều có một khóa liên quan.

**Phân loại:** Có 3 loại đồng bộ hóa:

| Loại đồng bộ hóa | Code ví dụ | Phạm vi khóa | Giải thích |
| --- | --- | --- | --- |
| Synchronized Method | `synchronized void m1() { ... }` | Đối tượng hiện tại (`this`) | Toàn bộ phương thức `m1()` được đồng bộ hóa. Chỉ một luồng có thể thực thi `m1()` trên một đối tượng cụ thể tại một thời điểm. Các luồng khác muốn truy cập `m1()` trên cùng đối tượng đó sẽ phải đợi. |
| Synchronized Block | `void m1() { synchronized (this) { ... } }` | Đối tượng cụ thể được chỉ định (ví dụ: `this`) | Chỉ khối mã bên trong `synchronized` được đồng bộ hóa. Các luồng khác vẫn có thể truy cập các phần khác của phương thức `m1()` đồng thời. |
| Static Synchronization | `synchronized static void m1() { ... }` | Lớp (`Class`) | Toàn bộ phương thức `static` `m1()` được đồng bộ hóa trên toàn bộ lớp. Chỉ một luồng có thể thực thi `m1()` trên lớp đó tại một thời điểm, bất kể có bao nhiêu đối tượng của lớp tồn tại. |

#### 10.2. Synchronized Method

```java
class A {
    // Phương thức synchronized: chỉ một luồng có thể truy cập cùng lúc
    synchronized void m1() {
        System.out.println(Thread.currentThread().getName() + " đang thực thi m1.");

        // Giả lập việc phương thức chạy lâu
        try { Thread.sleep(1000); } catch (InterruptedException e) { e.printStackTrace(); } 

        System.out.println(Thread.currentThread().getName() + " hoàn thành m1.");
    }

    // Phương thức không synchronized: nhiều luồng có thể truy cập cùng lúc
    void m2() { 
        System.out.println(Thread.currentThread().getName() + " đang thực thi m2."); 
    } 
}

// Lớp ThreadWorker đại diện cho các luồng thực thi, kế thừa từ Thread
class ThreadWorker extends Thread {
    A obj; // Đối tượng mà các luồng sẽ thao tác
    String method; // Phương thức mà luồng sẽ gọi ("m1" hoặc "m2")

    ThreadWorker(A obj, String method) {
        this.obj = obj;
        this.method = method;
    }

    public void run() { 
        if (method.equals("m1")) { 
            obj.m1(); // Gọi m1() - chỉ một luồng có thể truy cập tại một thời điểm
        } else if (method.equals("m2")) {
            obj.m2(); // Gọi m2() - nhiều luồng có thể truy cập đồng thời
        }
    }
}

public class Main {
    public static void main(String[] args) {
        A obj = new A(); 

        ThreadWorker t0 = new ThreadWorker(obj, "m1");
        ThreadWorker t1 = new ThreadWorker(obj, "m1");
        ThreadWorker t2 = new ThreadWorker(obj, "m2");
        ThreadWorker t3 = new ThreadWorker(obj, "m2");

        t0.start();
        t1.start();
        t2.start();
        t3.start();
    }
}
```

**Kết quả dự kiến**

| Trường hợp | Thứ tự thực thi | Kết luận |
| --- | --- | --- |
| Trường hợp 1 | - Thread-0 thực thi m1()<br>- Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 hoàn thành m1()<br>- Thread-1 bắt đầu thực thi m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành m1() | Thứ tự này phản ánh chính xác việc đồng bộ hóa của m1(), trong khi các luồng gọi m2() thực thi đồng thời. |
| Trường hợp 2 | - Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 thực thi m1()<br>- Thread-0 hoàn thành m1()<br>- Thread-1 bắt đầu thực thi m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành m1() | Thứ tự khác nhưng vẫn đảm bảo việc đồng bộ hóa cho m1(). Kết quả này cũng hợp lệ trong lập trình đa luồng. |

#### 10.3. Synchronized Block

```java
class A {
    void m1() {
        // Khối synchronized: chỉ một luồng có thể truy cập cùng lúc
        synchronized (this) {
            System.out.println(Thread.currentThread().getName() + " đang thực thi khối synchronized trong m1.");

            try { Thread.sleep(1000); } catch (InterruptedException e) { e.printStackTrace(); }

            System.out.println(Thread.currentThread().getName() + " hoàn thành khối synchronized trong m1.");
        }
    }

    void m2() { 
        System.out.println(Thread.currentThread().getName() + " đang thực thi m2."); 
    } 
}

// ... (Lớp ThreadWorker và Main tương tự như phần 10.2)
```

**Kết quả dự kiến**

| Trường hợp | Thứ tự thực thi | Kết luận |
| --- | --- | --- |
| Trường hợp 1 | - Thread-0 thực thi khối synchronized trong m1()<br>- Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 hoàn thành khối synchronized trong m1()<br>- Thread-1 bắt đầu thực thi khối synchronized trong m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành khối synchronized trong m1() | Thứ tự này phản ánh việc đồng bộ hóa của khối code trong m1(), trong khi các luồng gọi m2() thực thi đồng thời. Chỉ một luồng có thể truy cập khối synchronized tại một thời điểm. |
| Trường hợp 2 | - Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 thực thi khối synchronized trong m1()<br>- Thread-0 hoàn thành khối synchronized trong m1()<br>- Thread-1 bắt đầu thực thi khối synchronized trong m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành khối synchronized trong m1() | Tương tự trường hợp 1, thứ tự thực thi có thể khác nhau, nhưng nguyên tắc đồng bộ hóa vẫn được đảm bảo. Chỉ một luồng được phép truy cập vào khối synchronized tại một thời điểm. |

#### 10.4. Static Synchronization

```java
class A {
    // Phương thức static synchronized: chỉ một luồng có thể truy cập cùng lúc trên toàn bộ lớp
    synchronized static void m1() {
        System.out.println(Thread.currentThread().getName() + " đang thực thi phương thức static synchronized m1.");

        try { Thread.sleep(1000); } catch (InterruptedException e) { e.printStackTrace(); }

        System.out.println(Thread.currentThread().getName() + " hoàn thành phương thức static synchronized m1.");
    }

    void m2() { 
        System.out.println(Thread.currentThread().getName() + " đang thực thi m2."); 
    }
}

// Lớp ThreadWorker đại diện cho các luồng thực thi, kế thừa từ Thread
class ThreadWorker extends Thread {
    A obj; // Đối tượng mà các luồng sẽ thao tác (không cần thiết cho phương thức static)
    String method; // Phương thức mà luồng sẽ gọi ("m1" hoặc "m2")

    ThreadWorker(A obj, String method) {
        this.obj = obj;
        this.method = method;
    }

    public void run() {
        if (method.equals("m1")) {
            A.m1(); // Gọi phương thức static m1() trực tiếp thông qua tên lớp
        } else if (method.equals("m2")) {
            obj.m2();
        }
    }
}

// ... (Lớp Main tương tự như phần 10.2)
```

**Kết quả dự kiến**

| Trường hợp | Thứ tự thực thi | Kết luận |
| --- | --- | --- |
| Trường hợp 1 | - Thread-0 thực thi m1()<br>- Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 hoàn thành m1()<br>- Thread-1 bắt đầu thực thi m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành m1() | Thứ tự này phản ánh chính xác việc đồng bộ hóa của phương thức static m1(). Chỉ một luồng có thể truy cập m1() tại một thời điểm, bất kể nó được gọi từ đối tượng nào của lớp A. |
| Trường hợp 2 | - Thread-2 và Thread-3 thực thi m2() cùng lúc<br>- Thread-0 thực thi m1()<br>- Thread-0 hoàn thành m1()<br>- Thread-1 bắt đầu thực thi m1() sau khi Thread-0 hoàn thành<br>- Thread-1 hoàn thành m1() | Tương tự trường hợp 1, thứ tự thực thi có thể khác nhau, nhưng nguyên tắc đồng bộ hóa vẫn được đảm bảo cho phương thức static m1(). Việc nhiều luồng gọi m2() không ảnh hưởng đến việc đồng bộ hóa của m1(). |

#### 10.5. Đồng bộ hóa của `Collection` (`Map`, `Set`)

**1. Đồng bộ hóa Collection**

Java cung cấp hai cách chính để đồng bộ hóa Collection:

**a. Sử dụng Collections.synchronizedList/Set/Map:**
```java
List<String> syncList = Collections.synchronizedList(new ArrayList<>());
Set<String> syncSet = Collections.synchronizedSet(new HashSet<>());
Map<String, String> syncMap = Collections.synchronizedMap(new HashMap<>());
```

- Các phương thức của collection được bọc trong synchronized block
- Cần sử dụng synchronized block khi duyệt qua collection:
```java
synchronized (syncList) {
    Iterator<String> i = syncList.iterator();
    while (i.hasNext())
        foo(i.next());
}
```

**b. Sử dụng các lớp đồng bộ hóa có sẵn:**
- `Vector` và `Hashtable` (các lớp cũ, đã được thay thế bởi ArrayList và HashMap)
- `ConcurrentHashMap`, `CopyOnWriteArrayList`, `CopyOnWriteArraySet` (từ package java.util.concurrent)

**2. So sánh các cách đồng bộ hóa Collection**

| Loại Collection | Đồng bộ hóa truyền thống | Đồng bộ hóa hiệu suất cao |
| --- | --- | --- |
| List | `Collections.synchronizedList(new ArrayList<>)` | `CopyOnWriteArrayList` |
| Set | `Collections.synchronizedSet(new HashSet<>)` | `ConcurrentSkipListSet`, `CopyOnWriteArraySet` |
| Map | `Collections.synchronizedMap(new HashMap<>)`, `Hashtable` | `ConcurrentHashMap` |

**3. ConcurrentHashMap - Giải pháp đồng bộ hóa hiệu suất cao**

```java
ConcurrentHashMap<String, Integer> concurrentMap = new ConcurrentHashMap<>();

// Các phương thức an toàn với đa luồng
concurrentMap.put("key1", 1);
concurrentMap.get("key1");
concurrentMap.putIfAbsent("key2", 2);
concurrentMap.compute("key1", (k, v) -> v != null ? v + 1 : 1);
```

**Ưu điểm của ConcurrentHashMap:**
- Chia không gian khóa thành nhiều segment (mặc định 16)
- Mỗi segment có khóa riêng, cho phép nhiều luồng truy cập đồng thời
- Hiệu suất cao hơn Collections.synchronizedMap
- Cung cấp các phương thức nguyên tử như putIfAbsent, compute, merge

**4. CopyOnWriteArrayList - Giải pháp cho trường hợp đọc nhiều, ghi ít**

```java
CopyOnWriteArrayList<String> copyOnWriteList = new CopyOnWriteArrayList<>();
copyOnWriteList.add("A");
copyOnWriteList.add("B");

// Duyệt an toàn mà không cần synchronized
for (String s : copyOnWriteList) {
    System.out.println(s);
}
```

**Đặc điểm:**
- Khi sửa đổi, tạo một bản sao của mảng cơ sở
- Đọc không cần khóa, rất nhanh
- Viết chậm do phải sao chép mảng
- Thích hợp cho trường hợp đọc nhiều, ghi ít

**5. Ví dụ so sánh hiệu suất**

```java
import java.util.*;
import java.util.concurrent.*;
import java.util.stream.IntStream;

public class ConcurrentCollectionPerformance {
    public static void main(String[] args) {
        int iterations = 100000;
        int threads = 10;
        
        // So sánh HashMap và ConcurrentHashMap
        testMapPerformance(new HashMap<>(), "HashMap", iterations, threads);
        testMapPerformance(new ConcurrentHashMap<>(), "ConcurrentHashMap", iterations, threads);
        
        // So sánh ArrayList và CopyOnWriteArrayList
        testListPerformance(new ArrayList<>(), "ArrayList", iterations, threads);
        testListPerformance(new CopyOnWriteArrayList<>(), "CopyOnWriteArrayList", iterations, threads);
    }
    
    private static void testMapPerformance(Map<String, Integer> map, String name, int iterations, int threads) {
        long startTime = System.currentTimeMillis();
        
        // Khởi tạo dữ liệu
        for (int i = 0; i < 1000; i++) {
            map.put("key" + i, i);
        }
        
        // Tạo và chạy các luồng
        List<Thread> threadList = new ArrayList<>();
        for (int t = 0; t < threads; t++) {
            Thread thread = new Thread(() -> {
                for (int i = 0; i < iterations; i++) {
                    String key = "key" + (i % 1000);
                    map.get(key);
                    map.put(key, i);
                }
            });
            threadList.add(thread);
            thread.start();
        }
        
        // Chờ tất cả luồng hoàn thành
        for (Thread thread : threadList) {
            try {
                thread.join();
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        long duration = System.currentTimeMillis() - startTime;
        System.out.println(name + " took: " + duration + "ms");
    }
    
    private static void testListPerformance(List<String> list, String name, int iterations, int threads) {
        long startTime = System.currentTimeMillis();
        
        // Khởi tạo dữ liệu
        for (int i = 0; i < 1000; i++) {
            list.add("item" + i);
        }
        
        // Tạo và chạy các luồng
        List<Thread> threadList = new ArrayList<>();
        for (int t = 0; t < threads; t++) {
            Thread thread = new Thread(() -> {
                for (int i = 0; i < iterations; i++) {
                    int index = i % 1000;
                    list.get(index);
                    if (i % 100 == 0) {
                        list.set(index, "updated");
                    }
                }
            });
            threadList.add(thread);
            thread.start();
        }
        
        // Chờ tất cả luồng hoàn thành
        for (Thread thread : threadList) {
            try {
                thread.join();
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        long duration = System.currentTimeMillis() - startTime;
        System.out.println(name + " took: " + duration + "ms");
    }
}
```

**Kết luận khi chọn Collection đồng bộ:**
- Sử dụng `ConcurrentHashMap` thay vì `synchronizedMap` cho hiệu suất tốt hơn
- Sử dụng `CopyOnWriteArrayList` khi có nhiều thao tác đọc và ít thao tác ghi
- Luôn sử dụng synchronized block khi duyệt qua các collection được đồng bộ hóa bằng Collections.synchronizedX
- Tránh sử dụng Vector và Hashtable trong code mới

### 11. Thread (Luồng)

#### 11.1. Các trạng thái của `Thread`

Một luồng trong Java có thể ở một trong sáu trạng thái sau:

1. **NEW**: Luồng đã được tạo nhưng chưa bắt đầu chạy (chưa gọi phương thức `start()`)

2. **RUNNABLE**: Luồng đang chạy hoặc sẵn sàng chạy (đang chờ CPU)
   - Đang thực thi mã
   - Đang chờ được cấp CPU time

3. **BLOCKED**: Luồng đang chờ khóa monitor để vào một khối synchronized hoặc phương thức synchronized
   - Đang chờ giải phóng khóa để vào synchronized block/method
   - Không thể tiếp tục cho đến khi có được khóa

4. **WAITING**: Luồng đang chờ không xác định thời gian cho một hành động cụ thể
   - Chờ khi gọi `Object.wait()`
   - Chờ khi gọi `Thread.join()`
   - Chờ khi gọi `LockSupport.park()`

5. **TIMED_WAITING**: Luồng đang chờ trong một khoảng thời gian xác định
   - Chờ khi gọi `Thread.sleep(long millis)`
   - Chờ khi gọi `Object.wait(long timeout)`
   - Chờ khi gọi `Thread.join(long millis)`
   - Chờ khi gọi `LockSupport.parkNanos(long nanos)`

6. **TERMINATED**: Luồng đã kết thúc thực thi
   - Hoàn thành phương thức `run()`
   - Bị dừng do ngoại lệ không được xử lý

**Sơ đồ chuyển trạng thái:**

```
NEW
  │
  ▼
RUNNABLE ←──────────┐
  │                 │
  ├─→ BLOCKED       │
  │      │          │
  │      ▼          │
  │   RUNNABLE      │
  │                 │
  ├─→ WAITING       │
  │      │          │
  │      ▼          │
  │   RUNNABLE ─────┘
  │
  ▼
TERMINATED
```

**Ví dụ minh họa các trạng thái:**

```java
public class ThreadStatesExample {
    public static void main(String[] args) throws InterruptedException {
        Object lock = new Object();
        
        Thread t1 = new Thread(() -> {
            synchronized (lock) {
                try {
                    System.out.println("Thread t1: RUNNABLE (sau khi start)");
                    Thread.sleep(1000);
                    System.out.println("Thread t1: TIMED_WAITING (sau khi sleep)");
                    lock.wait();
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        });
        
        Thread t2 = new Thread(() -> {
            synchronized (lock) {
                System.out.println("Thread t2: RUNNABLE");
                try {
                    Thread.sleep(5000);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        });
        
        System.out.println("Thread t1 state: " + t1.getState()); // NEW
        t1.start();
        Thread.sleep(100);
        System.out.println("Thread t1 state: " + t1.getState()); // RUNNABLE
        
        t2.start();
        Thread.sleep(100);
        System.out.println("Thread t1 state: " + t1.getState()); // WAITING
        System.out.println("Thread t2 state: " + t2.getState()); // BLOCKED
        
        Thread.sleep(2000);
        System.out.println("Thread t1 state: " + t1.getState()); // WAITING
        System.out.println("Thread t2 state: " + t2.getState()); // RUNNABLE
        
        synchronized (lock) {
            lock.notify();
        }
        
        t1.join();
        t2.join();
        System.out.println("Thread t1 state: " + t1.getState()); // TERMINATED
        System.out.println("Thread t2 state: " + t2.getState()); // TERMINATED
    }
}
```

**Lưu ý quan trọng:**
- Trạng thái RUNNABLE bao gồm cả khi luồng đang chạy và khi đang sẵn sàng chạy (chờ CPU)
- Trạng thái BLOCKED chỉ xảy ra khi chờ khóa monitor
- Trạng thái WAITING và TIMED_WAITING xảy ra khi luồng đang chờ một sự kiện cụ thể
- Không thể chuyển trực tiếp từ BLOCKED sang WAITING hoặc ngược lại

#### 11.2. Phân biệt `Concurrency` và `Multithreading`

| Đặc điểm | Concurrency | Multithreading |
| --- | --- | --- |
| Định nghĩa | Khả năng xử lý nhiều tác vụ cùng lúc | Kỹ thuật thực thi nhiều luồng trên một CPU |
| Mục đích | Tối ưu hóa việc sử dụng tài nguyên, xử lý nhiều tác vụ | Cho phép chương trình thực hiện nhiều tác vụ đồng thời |
| Triển khai | Có thể thực hiện với một hoặc nhiều luồng | Luôn sử dụng nhiều luồng |
| Phạm vi | Rộng hơn, bao gồm multithreading | Là một phần của concurrency |
| Mô hình | Task-based | Thread-based |
| Ví dụ | Xử lý nhiều request trong ứng dụng web | Chạy đồng thời UI và xử lý backend |
| Đơn vị cơ bản | Task, Process | Thread |
| Quản lý | Thông qua ExecutorService, CompletableFuture | Thông qua Thread, Runnable |

**Giải thích chi tiết:**

**Concurrency (Đồng thời):**
- Là khái niệm rộng hơn, chỉ khả năng xử lý nhiều tác vụ cùng lúc
- Không nhất thiết phải thực thi song song, có thể luân phiên giữa các tác vụ
- Tập trung vào việc thiết kế hệ thống để xử lý nhiều tác vụ một cách hiệu quả
- Ví dụ: Một nhân viên phục vụ trong quán cà phê có thể nhận đơn, pha cà phê, thu tiền một cách luân phiên

**Multithreading (Đa luồng):**
- Là kỹ thuật cụ thể để đạt được concurrency
- Sử dụng nhiều luồng (threads) để thực thi nhiều phần của chương trình cùng lúc
- Mỗi luồng là một dòng thực thi riêng biệt
- Ví dụ: Nhiều nhân viên phục vụ trong quán cà phê, mỗi người làm một nhiệm vụ khác nhau cùng lúc

**Mối quan hệ:**
- Multithreading là một cách để đạt được concurrency
- Concurrency có thể đạt được mà không cần multithreading (ví dụ: event-driven programming)
- Multithreading không đảm bảo concurrency hiệu quả nếu không được thiết kế tốt

**Ví dụ minh họa:**

**Concurrency với một luồng (Single-threaded Concurrency):**
```java
// Sử dụng event loop trong Node.js
const fs = require('fs');

fs.readFile('file1.txt', (err, data) => {
  console.log('File 1 read');
});

fs.readFile('file2.txt', (err, data) => {
  console.log('File 2 read');
});

console.log('Reading files...');
// Output: 
// Reading files...
// File 1 read
// File 2 read
```

**Multithreading trong Java:**
```java
class Task implements Runnable {
    private String name;
    
    public Task(String name) {
        this.name = name;
    }
    
    @Override
    public void run() {
        System.out.println(name + " started");
        try {
            Thread.sleep(1000);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        System.out.println(name + " completed");
    }
}

public class MultithreadingExample {
    public static void main(String[] args) {
        Thread t1 = new Thread(new Task("Task 1"));
        Thread t2 = new Thread(new Task("Task 2"));
        
        t1.start();
        t2.start();
        
        try {
            t1.join();
            t2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("All tasks completed");
    }
}
```

**Khi nào nên sử dụng cái nào?**
- Sử dụng **Concurrency** khi:
  - Cần xử lý nhiều tác vụ mà không nhất thiết phải song song
  - Hệ thống có tài nguyên hạn chế
  - Cần đơn giản hóa thiết kế hệ thống

- Sử dụng **Multithreading** khi:
  - Cần tận dụng đa nhân CPU
  - Các tác vụ có thể thực thi độc lập
  - Hiệu suất là yếu tố quan trọng

**Lưu ý quan trọng:**
- Multithreading có thể dẫn đến các vấn đề như race condition, deadlock nếu không được quản lý tốt
- Concurrency model hiện đại (như Reactive Programming) thường dễ quản lý hơn multithreading truyền thống
- Java cung cấp nhiều công cụ để hỗ trợ cả concurrency và multithreading:
  - ExecutorService
  - CompletableFuture
  - Reactive Streams
  - Parallel Streams

---

## IV. File và I/O trong Java

### 12. File và I/O

#### 12.1. Cơ bản về `File`, `InputStream`, `Reader`

**1. Lớp File**

Lớp `File` trong Java đại diện cho một đường dẫn đến file hoặc thư mục trên hệ thống tập tin.

```java
import java.io.File;

public class FileExample {
    public static void main(String[] args) {
        // Tạo đối tượng File
        File file = new File("example.txt");
        
        // Kiểm tra sự tồn tại
        System.out.println("File exists: " + file.exists());
        
        // Tạo file mới
        try {
            boolean created = file.createNewFile();
            System.out.println("File created: " + created);
        } catch (Exception e) {
            e.printStackTrace();
        }
        
        // Thông tin về file
        System.out.println("File name: " + file.getName());
        System.out.println("Absolute path: " + file.getAbsolutePath());
        System.out.println("Readable: " + file.canRead());
        System.out.println("Writable: " + file.canWrite());
        System.out.println("File size: " + file.length() + " bytes");
        
        // Tạo thư mục
        File dir = new File("new_directory");
        boolean dirCreated = dir.mkdir();
        System.out.println("Directory created: " + dirCreated);
        
        // Liệt kê các file trong thư mục
        File currentDir = new File(".");
        String[] files = currentDir.list();
        System.out.println("Files in current directory:");
        for (String f : files) {
            System.out.println(f);
        }
    }
}
```

**2. InputStream và các lớp con**

`InputStream` là lớp cơ sở cho tất cả các luồng đọc dữ liệu dạng byte.

- **FileInputStream**: Đọc dữ liệu từ file
- **ByteArrayInputStream**: Đọc dữ liệu từ mảng byte
- **BufferedInputStream**: Thêm bộ đệm cho luồng đọc
- **DataInputStream**: Đọc dữ liệu nguyên thủy (int, float, v.v.)
- **ObjectInputStream**: Đọc đối tượng được serial hóa

```java
import java.io.*;

public class InputStreamExample {
    public static void main(String[] args) {
        try (FileInputStream fis = new FileInputStream("example.txt")) {
            int content;
            while ((content = fis.read()) != -1) {
                System.out.print((char) content);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
        
        // Sử dụng BufferedInputStream cho hiệu suất tốt hơn
        try (FileInputStream fis = new FileInputStream("example.txt");
             BufferedInputStream bis = new BufferedInputStream(fis)) {
            byte[] buffer = new byte[1024];
            int bytesRead;
            while ((bytesRead = bis.read(buffer)) != -1) {
                System.out.write(buffer, 0, bytesRead);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**3. Reader và các lớp con**

`Reader` là lớp cơ sở cho tất cả các luồng đọc dữ liệu dạng ký tự (character).

- **FileReader**: Đọc ký tự từ file
- **BufferedReader**: Thêm bộ đệm và phương thức đọc dòng
- **InputStreamReader**: Chuyển đổi InputStream thành Reader
- **CharArrayReader**: Đọc từ mảng ký tự

```java
import java.io.*;

public class ReaderExample {
    public static void main(String[] args) {
        // Sử dụng FileReader cơ bản
        try (FileReader fr = new FileReader("example.txt")) {
            int character;
            while ((character = fr.read()) != -1) {
                System.out.print((char) character);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
        
        // Sử dụng BufferedReader để đọc từng dòng
        try (BufferedReader br = new BufferedReader(new FileReader("example.txt"))) {
            String line;
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**4. So sánh InputStream và Reader**

| Đặc điểm | InputStream | Reader |
| --- | --- | --- |
| Dữ liệu | Byte (8-bit) | Ký tự (16-bit, Unicode) |
| Mục đích | Đọc dữ liệu nhị phân | Đọc văn bản |
| Encoding | Không xử lý encoding | Xử lý encoding (UTF-8, ASCII, v.v.) |
| Lớp cơ sở | java.io.InputStream | java.io.Reader |
| Phương thức đọc | read(), available() | read(), ready() |
| Lớp con phổ biến | FileInputStream, BufferedInputStream | FileReader, BufferedReader |
| Hiệu suất với văn bản | Thấp hơn | Cao hơn |

**5. NIO (New I/O) - Phiên bản cải tiến**

Từ Java 7, NIO.2 cung cấp API mạnh mẽ hơn cho thao tác file:

```java
import java.nio.file.*;
import java.io.IOException;
import java.util.List;

public class NIOExample {
    public static void main(String[] args) {
        Path path = Paths.get("example.txt");
        
        // Đọc toàn bộ nội dung file
        try {
            List<String> lines = Files.readAllLines(path);
            for (String line : lines) {
                System.out.println(line);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
        
        // Ghi file
        try {
            Files.write(path, "New content".getBytes());
        } catch (IOException e) {
            e.printStackTrace();
        }
        
        // Sao chép file
        try {
            Files.copy(path, Paths.get("example_copy.txt"), StandardCopyOption.REPLACE_EXISTING);
        } catch (IOException e) {
            e.printStackTrace();
        }
        
        // Di chuyển file
        try {
            Files.move(path, Paths.get("new_location/example.txt"), StandardCopyOption.REPLACE_EXISTING);
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

#### 12.2. Sử dụng `Files.walk`

Phương thức `Files.walk()` được sử dụng để duyệt cây thư mục một cách đệ quy.

**1. Cơ bản về Files.walk**

```java
import java.io.IOException;
import java.nio.file.*;

public class FilesWalkExample {
    public static void main(String[] args) {
        Path startPath = Paths.get(".");
        
        try {
            // Duyệt tất cả các file và thư mục từ đường dẫn bắt đầu
            Files.walk(startPath)
                 .forEach(path -> System.out.println(path));
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**2. Giới hạn độ sâu của việc duyệt**

```java
import java.io.IOException;
import java.nio.file.*;

public class FilesWalkDepthExample {
    public static void main(String[] args) {
        Path startPath = Paths.get(".");
        
        try {
            // Chỉ duyệt 2 cấp độ thư mục
            Files.walk(startPath, 2)
                 .forEach(path -> System.out.println(path));
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**3. Lọc các file theo điều kiện**

```java
import java.io.IOException;
import java.nio.file.*;
import java.util.stream.*;

public class FilesWalkFilterExample {
    public static void main(String[] args) {
        Path startPath = Paths.get(".");
        
        try {
            // Chỉ hiển thị các file .java
            Files.walk(startPath)
                 .filter(path -> path.toString().endsWith(".java"))
                 .forEach(System.out::println);
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**4. Xử lý ngoại lệ khi duyệt**

```java
import java.io.IOException;
import java.nio.file.*;
import java.nio.file.attribute.*;

public class FilesWalkExceptionExample {
    public static void main(String[] args) {
        Path startPath = Paths.get(".");
        
        try {
            Files.walkFileTree(startPath, new SimpleFileVisitor<Path>() {
                @Override
                public FileVisitResult visitFile(Path file, BasicFileAttributes attrs) {
                    System.out.println("File: " + file);
                    return FileVisitResult.CONTINUE;
                }
                
                @Override
                public FileVisitResult preVisitDirectory(Path dir, BasicFileAttributes attrs) {
                    System.out.println("Directory: " + dir);
                    return FileVisitResult.CONTINUE;
                }
                
                @Override
                public FileVisitResult visitFileFailed(Path file, IOException exc) {
                    System.err.println("Failed to access: " + file + ", " + exc);
                    return FileVisitResult.CONTINUE;
                }
            });
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**5. So sánh Files.walk và Files.walkFileTree**

| Đặc điểm | Files.walk | Files.walkFileTree |
| --- | --- | --- |
| Kiểu trả về | Stream<Path> | void |
| Cách sử dụng | Sử dụng với Stream API | Sử dụng với FileVisitor |
| Xử lý ngoại lệ | Ném IOException | Có thể xử lý ngoại lệ trong visitFileFailed |
| Linh hoạt | Ít linh hoạt hơn | Linh hoạt hơn |
| Hiệu suất | Tốt cho xử lý đơn giản | Tốt cho xử lý phức tạp |
| Ví dụ | `Files.walk(path).filter(...).forEach(...)` | `Files.walkFileTree(path, new SimpleFileVisitor<...>())` |

**6. Ví dụ thực tế: Tìm tất cả file lớn hơn 1MB**

```java
import java.io.IOException;
import java.nio.file.*;
import java.nio.file.attribute.*;

public class FindLargeFiles {
    public static void main(String[] args) {
        Path startPath = Paths.get(".");
        long minSize = 1024 * 1024; // 1MB
        
        try {
            Files.walkFileTree(startPath, new SimpleFileVisitor<Path>() {
                @Override
                public FileVisitResult visitFile(Path file, BasicFileAttributes attrs) {
                    if (attrs.isRegularFile() && attrs.size() > minSize) {
                        System.out.printf("Large file: %s (%d bytes)%n", 
                                file, attrs.size());
                    }
                    return FileVisitResult.CONTINUE;
                }
                
                @Override
                public FileVisitResult visitFileFailed(Path file, IOException exc) {
                    System.err.println("Error accessing file: " + file);
                    return FileVisitResult.CONTINUE;
                }
            });
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

**7. Lưu ý quan trọng khi sử dụng Files.walk**

- Đảm bảo đóng Stream sau khi sử dụng (sử dụng try-with-resources)
- Xử lý ngoại lệ IO thích hợp
- Cẩn thận khi duyệt cây thư mục lớn để tránh tràn bộ nhớ
- Sử dụng độ sâu giới hạn (depth) khi không cần duyệt toàn bộ cây
- Luôn kiểm tra quyền truy cập file/thư mục

---

## V. Quản lý Exception (Ngoại lệ) trong Java

### 13. Xử lý Exception

#### 13.1. Tổng quan về Exception và cơ chế xử lý

**1. Phân loại Exception trong Java**

Trong Java, Exception được phân thành 3 loại chính:

1. **Checked Exceptions** (Ngoại lệ kiểm tra):
   - Kế thừa từ lớp `Exception` nhưng không phải từ `RuntimeException`
   - Trình biên dịch yêu cầu phải xử lý hoặc khai báo với `throws`
   - Ví dụ: `IOException`, `SQLException`, `ClassNotFoundException`

2. **Unchecked Exceptions** (Ngoại lệ không kiểm tra):
   - Kế thừa từ `RuntimeException`
   - Không bắt buộc phải xử lý hoặc khai báo
   - Ví dụ: `NullPointerException`, `ArrayIndexOutOfBoundsException`, `IllegalArgumentException`

3. **Errors** (Lỗi hệ thống):
   - Kế thừa từ lớp `Error`
   - Đại diện cho các vấn đề nghiêm trọng mà ứng dụng thường không thể xử lý
   - Ví dụ: `OutOfMemoryError`, `StackOverflowError`, `NoClassDefFoundError`

**Sơ đồ phân cấp:**

```
Throwable
├── Error
│   ├── OutOfMemoryError
│   ├── StackOverflowError
│   └── ...
├── Exception
│   ├── RuntimeException
│   │   ├── NullPointerException
│   │   ├── ArrayIndexOutOfBoundsException
│   │   └── ...
│   ├── IOException
│   ├── SQLException
│   └── ...
```

**2. Cơ chế xử lý Exception**

Java cung cấp các cơ chế chính để xử lý exception:

**a. try-catch-finally**

```java
try {
    // Mã có thể ném exception
    int result = 10 / 0;
} catch (ArithmeticException e) {
    // Xử lý ArithmeticException
    System.out.println("Cannot divide by zero");
} catch (Exception e) {
    // Xử lý các exception khác
    System.out.println("An error occurred: " + e.getMessage());
} finally {
    // Luôn được thực thi, dù có exception hay không
    System.out.println("Cleanup code");
}
```

**b. try-with-resources (Java 7+)**

```java
try (FileInputStream fis = new FileInputStream("file.txt");
     BufferedReader br = new BufferedReader(new FileReader("file.txt"))) {
    // Sử dụng các resource
    String line = br.readLine();
    System.out.println(line);
} catch (IOException e) {
    e.printStackTrace();
}
// Resource tự động được đóng sau khối try
```

**c. throws**

```java
public void readFile(String fileName) throws IOException {
    FileInputStream fis = new FileInputStream(fileName);
    // Xử lý file
}
```

**3. Tạo và ném Exception tùy chỉnh**

```java
// Tạo exception tùy chỉnh
class InsufficientFundsException extends Exception {
    private double amount;
    
    public InsufficientFundsException(double amount) {
        this.amount = amount;
    }
    
    public double getAmount() {
        return amount;
    }
}

// Sử dụng exception tùy chỉnh
public class BankAccount {
    private double balance;
    
    public void withdraw(double amount) throws InsufficientFundsException {
        if (amount > balance) {
            throw new InsufficientFundsException(amount - balance);
        }
        balance -= amount;
    }
    
    public static void main(String[] args) {
        BankAccount account = new BankAccount();
        try {
            account.withdraw(1000.0);
        } catch (InsufficientFundsException e) {
            System.out.println("Insufficient funds: need $" + e.getAmount() + " more");
        }
    }
}
```

**4. Best Practices khi xử lý Exception**

- **Không bắt Exception chung (catch Exception e)** trừ khi thực sự cần thiết
- **Luôn ghi log exception** với thông tin đầy đủ
- **Đóng tài nguyên** trong khối finally hoặc sử dụng try-with-resources
- **Không để khối catch trống** (empty catch block)
- **Chuyển đổi exception** khi cần thiết để cung cấp ngữ cảnh phù hợp
- **Sử dụng finally cho cleanup**, không phải cho xử lý logic
- **Throw early, catch late**: Ném exception sớm nhất có thể, xử lý ở mức cao nhất có thể

**5. Ví dụ về xử lý Exception tốt**

```java
import java.io.*;
import java.sql.*;

public class GoodExceptionHandling {
    public static void main(String[] args) {
        // Xử lý từng loại exception cụ thể
        try {
            readFile("data.txt");
            connectToDatabase();
        } catch (FileNotFoundException e) {
            // Xử lý riêng cho FileNotFoundException
            System.err.println("File not found: " + e.getMessage());
            // Log chi tiết
            logError("FILE_ERROR", e);
        } catch (SQLException e) {
            // Xử lý riêng cho SQLException
            System.err.println("Database error: " + e.getMessage());
            logError("DB_ERROR", e);
        } catch (Exception e) {
            // Xử lý các exception còn lại
            System.err.println("Unexpected error: " + e.getMessage());
            logError("GENERAL_ERROR", e);
        } finally {
            // Cleanup
            System.out.println("Performing cleanup...");
        }
    }
    
    private static void readFile(String filename) throws FileNotFoundException {
        // Sử dụng try-with-resources để tự động đóng tài nguyên
        try (FileReader fr = new FileReader(filename);
             BufferedReader br = new BufferedReader(fr)) {
            String line;
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            // Chuyển đổi exception
            throw new FileNotFoundException("Error reading file: " + filename);
        }
    }
    
    private static void connectToDatabase() throws SQLException {
        // Kết nối cơ sở dữ liệu
        Connection conn = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "user", "password");
        // Xử lý cơ sở dữ liệu
    }
    
    private static void logError(String errorCode, Exception e) {
        // Ghi log với thông tin chi tiết
        System.err.println("[" + errorCode + "] " + e.getMessage());
        e.printStackTrace();
        // Có thể ghi vào file log hoặc hệ thống giám sát
    }
}
```

#### 13.2. Xử lý Exception trong trường hợp kế thừa (`extends`)

**1. Quy tắc override phương thức với exception**

Khi ghi đè (override) một phương thức có khai báo exception, có các quy tắc sau:

1. **Phương thức ghi đè không được khai báo throws checked exception rộng hơn** phương thức gốc
   - Có thể khai báo throws checked exception hẹp hơn hoặc không throws
   - Có thể khai báo throws unchecked exception dù phương thức gốc không throws

2. **Phương thức ghi đè có thể loại bỏ hoàn toàn throws** của phương thức gốc

**2. Ví dụ minh họa**

```java
// Lớp cha
class Parent {
    // throws IOException (checked exception)
    void readFile() throws IOException {
        // Đọc file
    }
    
    // throws SQLException (checked exception)
    void connectToDB() throws SQLException {
        // Kết nối cơ sở dữ liệu
    }
    
    // Không throws exception
    void process() {
        // Xử lý
    }
}

// Lớp con đúng theo quy tắc
class ChildCorrect extends Parent {
    // ĐÚNG: Loại bỏ throws IOException
    @Override
    void readFile() {
        // Đọc file
    }
    
    // ĐÚNG: throws exception hẹp hơn (con của SQLException)
    @Override
    void connectToDB() throws MySQLSyntaxErrorException {
        // Kết nối cơ sở dữ liệu MySQL
    }
    
    // ĐÚNG: throws unchecked exception dù phương thức gốc không throws
    @Override
    void process() {
        if (Math.random() > 0.5) {
            throw new NullPointerException();
        }
    }
}

// Lớp con sai theo quy tắc
class ChildIncorrect extends Parent {
    // SAI: throws checked exception rộng hơn (Exception là cha của IOException)
    @Override
    void readFile() throws Exception {
        // Đọc file
    }
    
    // SAI: throws checked exception không liên quan
    @Override
    void connectToDB() throws IOException {
        // Kết nối cơ sở dữ liệu
    }
    
    // ĐÚNG: Không throws nhưng ném unchecked exception
    @Override
    void process() {
        throw new IllegalArgumentException();
    }
}
```

**3. Bảng tóm tắt quy tắc override với exception**

| Trường hợp | Phương thức gốc | Phương thức ghi đè | Hợp lệ? | Lý do |
| --- | --- | --- | --- | --- |
| 1 | throws IOException | (không throws) | ✔ | Hẹp hơn |
| 2 | throws IOException | throws FileNotFoundException | ✔ | FileNotFoundException là con của IOException |
| 3 | throws IOException | throws Exception | ✘ | Exception là cha của IOException |
| 4 | throws IOException | throws SQLException | ✘ | SQLException không liên quan đến IOException |
| 5 | (không throws) | throws NullPointerException | ✔ | NullPointerException là unchecked exception |
| 6 | throws IOException | throws NullPointerException | ✔ | Có thể thêm unchecked exception |
| 7 | throws SQLException | throws MySQLSyntaxErrorException | ✔ | MySQLSyntaxErrorException là con của SQLException |

**4. Ví dụ thực tế với interface**

```java
// Interface
interface FileProcessor {
    void processFile(String filename) throws IOException;
}

// Implement interface
class TextFileProcessor implements FileProcessor {
    // Hợp lệ: Loại bỏ throws
    @Override
    public void processFile(String filename) {
        // Xử lý file văn bản
    }
}

class BinaryFileProcessor implements FileProcessor {
    // Hợp lệ: throws exception hẹp hơn
    @Override
    public void processFile(String filename) throws FileNotFoundException {
        // Xử lý file nhị phân
    }
}

class InvalidFileProcessor implements FileProcessor {
    // KHÔNG HỢP LỆ: throws exception rộng hơn
    @Override
    public void processFile(String filename) throws Exception {
        // Xử lý file
    }
}
```

**5. Best Practices khi làm việc với exception trong kế thừa**

- **Thiết kế interface và lớp cha với exception cụ thể**, tránh dùng Exception chung
- **Khi ghi đè, hãy giữ nguyên hoặc thu hẹp exception** được khai báo
- **Cung cấp tài liệu rõ ràng** về các exception có thể xảy ra
- **Sử dụng custom exception** để tạo hệ thống exception có cấu trúc
- **Tránh thay đổi hành vi exception** khi ghi đè phương thức

**6. Ví dụ về custom exception hierarchy**

```java
// Exception gốc cho ứng dụng
class ApplicationException extends Exception {
    public ApplicationException(String message) {
        super(message);
    }
}

// Exception cho xử lý file
class FileProcessingException extends ApplicationException {
    public FileProcessingException(String message) {
        super(message);
    }
}

class InvalidFileFormatException extends FileProcessingException {
    public InvalidFileFormatException(String message) {
        super(message);
    }
}

// Lớp xử lý file
class FileHandler {
    public void processFile(String filename) throws FileProcessingException {
        // Kiểm tra định dạng file
        if (!isValidFormat(filename)) {
            throw new InvalidFileFormatException("Invalid file format");
        }
        // Xử lý file
    }
    
    private boolean isValidFormat(String filename) {
        return filename.endsWith(".txt");
    }
}

// Lớp con
class TextFileHandler extends FileHandler {
    @Override
    public void processFile(String filename) {
        // Không throws FileProcessingException nhưng xử lý riêng
        try {
            super.processFile(filename);
        } catch (FileProcessingException e) {
            // Xử lý exception
            System.err.println("Error processing file: " + e.getMessage());
        }
    }
}
```

---

## VI. Các khái niệm nâng cao trong Java

### 14. Hibernate Annotations

#### 14.1. Các loại annotation trong Hibernate

**1. Entity Mapping Annotations**

| Annotation | Mô tả | Ví dụ |
| --- | --- | --- |
| `@Entity` | Đánh dấu một class là entity | `@Entity public class User { ... }` |
| `@Table` | Chỉ định tên bảng trong database | `@Table(name = "users")` |
| `@Id` | Đánh dấu trường là khóa chính | `@Id private Long id;` |
| `@GeneratedValue` | Chỉ định chiến lược tạo giá trị cho khóa chính | `@GeneratedValue(strategy = GenerationType.IDENTITY)` |
| `@Column` | Chỉ định mapping cho cột | `@Column(name = "username", length = 50, nullable = false)` |

**2. Relationship Annotations**

| Annotation | Mô tả | Ví dụ |
| --- | --- | --- |
| `@OneToOne` | Mối quan hệ một-một | `@OneToOne(mappedBy = "user")` |
| `@OneToMany` | Mối quan hệ một-nhiều | `@OneToMany(cascade = CascadeType.ALL, mappedBy = "user")` |
| `@ManyToOne` | Mối quan hệ nhiều-một | `@ManyToOne(fetch = FetchType.LAZY)` |
| `@ManyToMany` | Mối quan hệ nhiều-nhiều | `@ManyToMany(fetch = FetchType.EAGER)` |
| `@JoinColumn` | Chỉ định cột tham chiếu | `@JoinColumn(name = "user_id")` |
| `@JoinTable` | Chỉ định bảng trung gian cho @ManyToMany | `@JoinTable(name = "user_role", joinColumns = @JoinColumn(name = "user_id"), inverseJoinColumns = @JoinColumn(name = "role_id"))` |

**3. Fetch và Cascade Types**

| Annotation | Mô tả | Ví dụ |
| --- | --- | --- |
| `FetchType.LAZY` | Tải dữ liệu khi cần thiết | `@OneToMany(fetch = FetchType.LAZY)` |
| `FetchType.EAGER` | Tải dữ liệu ngay lập tức | `@ManyToOne(fetch = FetchType.EAGER)` |
| `CascadeType.PERSIST` | Cascade persist operation | `cascade = CascadeType.PERSIST` |
| `CascadeType.MERGE` | Cascade merge operation | `cascade = CascadeType.MERGE` |
| `CascadeType.REMOVE` | Cascade remove operation | `cascade = CascadeType.REMOVE` |
| `CascadeType.REFRESH` | Cascade refresh operation | `cascade = CascadeType.REFRESH` |
| `CascadeType.DETACH` | Cascade detach operation | `cascade = CascadeType.DETACH` |
| `CascadeType.ALL` | Tất cả các operation trên | `cascade = CascadeType.ALL` |

**4. Ví dụ đầy đủ về Entity**

```java
@Entity
@Table(name = "users")
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    @Column(name = "username", length = 50, nullable = false, unique = true)
    private String username;
    
    @Column(name = "email", length = 100, nullable = false)
    private String email;
    
    @Column(name = "password", length = 100, nullable = false)
    private String password;
    
    @Column(name = "created_at", nullable = false)
    private LocalDateTime createdAt;
    
    @OneToOne(mappedBy = "user", cascade = CascadeType.ALL)
    private UserProfile profile;
    
    @OneToMany(cascade = CascadeType.ALL, mappedBy = "user")
    private List<Order> orders = new ArrayList<>();
    
    @ManyToMany(fetch = FetchType.EAGER)
    @JoinTable(name = "user_role",
               joinColumns = @JoinColumn(name = "user_id"),
               inverseJoinColumns = @JoinColumn(name = "role_id"))
    private Set<Role> roles = new HashSet<>();
    
    // Constructors, getters, setters
}
```

**5. Các annotation nâng cao**

| Annotation | Mô tả | Ví dụ |
| --- | --- | --- |
| `@Transient` | Đánh dấu trường không được lưu vào database | `@Transient private String tempData;` |
| `@Temporal` | Chỉ định kiểu thời gian cho Date/Calendar | `@Temporal(TemporalType.TIMESTAMP) private Date createdAt;` |
| `@Lob` | Đánh dấu trường lưu trữ dữ liệu lớn | `@Lob private String bio;` |
| `@OrderBy` | Chỉ định thứ tự sắp xếp cho collection | `@OrderBy("orderDate DESC") private List<Order> orders;` |
| `@ElementCollection` | Mapping cho collection các giá trị đơn giản | `@ElementCollection private Set<String> tags;` |
| `@Embeddable` / `@Embedded` | Embed một object vào entity | `@Embeddable public class Address { ... }` |

**6. Best Practices khi sử dụng Hibernate Annotations**

- **Sử dụng tên bảng và cột có ý nghĩa**, tuân theo quy ước của database
- **Chỉ định fetch type phù hợp** với ngữ cảnh sử dụng
- **Sử dụng cascade type cẩn thận** để tránh xóa không mong muốn
- **Đặt tên cho các quan hệ rõ ràng** với thuộc tính `mappedBy`
- **Sử dụng Lombok** để giảm boilerplate code cho getters/setters
- **Tối ưu hóa các truy vấn** với fetch join khi cần thiết
- **Tránh N+1 query problem** bằng cách sử dụng batch fetching

**7. Ví dụ về giải quyết N+1 query problem**

```java
// Entity
@Entity
public class Department {
    @Id
    private Long id;
    
    private String name;
    
    // Sử dụng batch fetching để tránh N+1 problem
    @OneToMany(fetch = FetchType.LAZY)
    @BatchSize(size = 20)
    private List<Employee> employees;
}

// Repository
public interface DepartmentRepository extends JpaRepository<Department, Long> {
    // Sử dụng fetch join để tải employees cùng với department
    @Query("SELECT d FROM Department d LEFT JOIN FETCH d.employees WHERE d.id = :id")
    Department findByIdWithEmployees(@Param("id") Long id);
}
```

### 15. Date and Time API

**1. Giới thiệu về java.time API**

Java 8 giới thiệu API mới `java.time` để thay thế cho các lớp Date và Calendar cũ, với các ưu điểm:
- Không thay đổi được (immutable)
- An toàn với đa luồng
- API rõ ràng và dễ sử dụng
- Hỗ trợ timezone tốt hơn
- Xử lý ngày tháng chính xác hơn

**2. Các lớp chính trong Date and Time API**

| Lớp | Mô tả | Ví dụ |
| --- | --- | --- |
| `LocalDate` | Chỉ ngày (năm, tháng, ngày) | `LocalDate.now()` |
| `LocalTime` | Chỉ thời gian (giờ, phút, giây) | `LocalTime.now()` |
| `LocalDateTime` | Ngày và thời gian (không có timezone) | `LocalDateTime.now()` |
| `ZonedDateTime` | Ngày và thời gian với timezone | `ZonedDateTime.now()` |
| `Instant` | Thời điểm trên timeline (epoch-based) | `Instant.now()` |
| `Duration` | Khoảng thời gian tính bằng giây và nano giây | `Duration.between(start, end)` |
| `Period` | Khoảng thời gian tính bằng năm, tháng, ngày | `Period.between(startDate, endDate)` |
| `DateTimeFormatter` | Định dạng và parse ngày giờ | `DateTimeFormatter.ISO_LOCAL_DATE` |

**3. Ví dụ sử dụng các lớp cơ bản**

```java
import java.time.*;
import java.time.format.DateTimeFormatter;

public class DateTimeExamples {
    public static void main(String[] args) {
        // LocalDate - Chỉ ngày
        LocalDate today = LocalDate.now();
        System.out.println("Today: " + today);
        System.out.println("Year: " + today.getYear());
        System.out.println("Month: " + today.getMonth());
        System.out.println("Day of month: " + today.getDayOfMonth());
        System.out.println("Day of week: " + today.getDayOfWeek());
        
        // Thêm/xóa ngày
        LocalDate tomorrow = today.plusDays(1);
        LocalDate yesterday = today.minusDays(1);
        
        // LocalTime - Chỉ thời gian
        LocalTime now = LocalTime.now();
        System.out.println("\nCurrent time: " + now);
        System.out.println("Hour: " + now.getHour());
        System.out.println("Minute: " + now.getMinute());
        System.out.println("Second: " + now.getSecond());
        
        // Thêm/xóa thời gian
        LocalTime later = now.plusHours(2);
        LocalTime earlier = now.minusMinutes(30);
        
        // LocalDateTime - Ngày và thời gian
        LocalDateTime current = LocalDateTime.now();
        System.out.println("\nCurrent date and time: " + current);
        
        // ZonedDateTime - Ngày và thời gian với timezone
        ZonedDateTime utc = ZonedDateTime.now(ZoneId.of("UTC"));
        ZonedDateTime paris = ZonedDateTime.now(ZoneId.of("Europe/Paris"));
        ZonedDateTime newYork = ZonedDateTime.now(ZoneId.of("America/New_York"));
        System.out.println("\nUTC: " + utc);
        System.out.println("Paris: " + paris);
        System.out.println("New York: " + newYork);
        
        // Instant - Thời điểm trên timeline
        Instant instant = Instant.now();
        System.out.println("\nInstant: " + instant);
        
        // Duration - Khoảng thời gian
        Duration duration = Duration.between(now, later);
        System.out.println("\nDuration in hours: " + duration.toHours());
        System.out.println("Duration in minutes: " + duration.toMinutes());
        
        // Period - Khoảng thời gian theo ngày/tháng/năm
        Period period = Period.between(today, tomorrow);
        System.out.println("\nPeriod in days: " + period.getDays());
        
        // Định dạng ngày giờ
        DateTimeFormatter formatter = DateTimeFormatter.ofPattern("dd/MM/yyyy HH:mm:ss");
        String formattedDate = current.format(formatter);
        System.out.println("\nFormatted date: " + formattedDate);
        
        // Parse chuỗi thành ngày giờ
        String dateStr = "25/12/2023 10:30:00";
        LocalDateTime parsedDate = LocalDateTime.parse(dateStr, formatter);
        System.out.println("Parsed date: " + parsedDate);
    }
}
```

**4. So sánh java.time với Date và Calendar cũ**

| Đặc điểm | java.time (Java 8+) | Date/Calendar (Java 7-) |
| --- | --- | --- |
| Tính bất biến | Immutable (an toàn đa luồng) | Mutable (không an toàn đa luồng) |
| Thiết kế API | Logic và nhất quán | Thiếu nhất quán, phức tạp |
| Xử lý timezone | Được hỗ trợ tốt | Khó sử dụng |
| Hiệu suất | Tốt hơn | Kém hơn |
| Định dạng | Sử dụng DateTimeFormatter | Sử dụng SimpleDateFormat (không thread-safe) |
| Tính toán ngày tháng | Dễ dàng với plus/minus | Phức tạp với add/roll |
| Đơn vị thời gian | Rõ ràng (Duration, Period) | Không rõ ràng |
| Khởi tạo | Đơn giản, rõ ràng | Phức tạp |

**5. Chuyển đổi giữa java.time và Date cũ**

```java
import java.time.*;
import java.util.Date;

public class DateTimeConversion {
    // Chuyển từ Date sang java.time
    public static void convertFromDate() {
        Date date = new Date();
        
        // Date -> Instant
        Instant instant = date.toInstant();
        
        // Instant -> LocalDateTime (UTC)
        LocalDateTime utcDateTime = LocalDateTime.ofInstant(instant, ZoneId.of("UTC"));
        
        // Instant -> LocalDateTime (theo timezone cụ thể)
        LocalDateTime localDateTime = LocalDateTime.ofInstant(instant, ZoneId.systemDefault());
        
        // Instant -> ZonedDateTime
        ZonedDateTime zonedDateTime = ZonedDateTime.ofInstant(instant, ZoneId.systemDefault());
    }
    
    // Chuyển từ java.time sang Date
    public static void convertToDate() {
        LocalDateTime localDateTime = LocalDateTime.now();
        
        // LocalDateTime -> Instant
        Instant instant = localDateTime.atZone(ZoneId.systemDefault()).toInstant();
        
        // Instant -> Date
        Date date = Date.from(instant);
    }
    
    // Chuyển từ Calendar sang java.time
    public static void convertFromCalendar() {
        java.util.Calendar calendar = java.util.Calendar.getInstance();
        
        // Calendar -> Instant
        Instant instant = calendar.toInstant();
        
        // Calendar -> ZonedDateTime
        ZonedDateTime zonedDateTime = ZonedDateTime.ofInstant(instant, calendar.getTimeZone().toZoneId());
    }
    
    // Chuyển từ java.time sang Calendar
    public static void convertToCalendar() {
        ZonedDateTime zonedDateTime = ZonedDateTime.now();
        
        // ZonedDateTime -> Calendar
        java.util.Calendar calendar = java.util.Calendar.getInstance();
        calendar.setTimeInMillis(zonedDateTime.toInstant().toEpochMilli());
    }
}
```

**6. Best Practices khi sử dụng Date and Time API**

- **Sử dụng LocalDate/LocalTime/LocalDateTime** khi không cần timezone
- **Sử dụng ZonedDateTime** khi làm việc với múi giờ cụ thể
- **Sử dụng Instant** khi cần lưu trữ thời điểm trên timeline
- **Tránh sử dụng Date và Calendar cũ** trong code mới
- **Luôn chỉ định timezone rõ ràng** khi cần thiết
- **Sử dụng DateTimeFormatter** để định dạng và parse
- **Không sử dụng chuỗi cố định** cho định dạng ngày giờ (nên dùng hằng số)
- **Sử dụng Period cho khoảng thời gian theo ngày/tháng/năm**, Duration cho khoảng thời gian theo giờ/phút/giây

**7. Ví dụ thực tế: Tính toán ngày làm việc**

```java
import java.time.*;
import java.time.temporal.*;

public class BusinessDayCalculator {
    // Kiểm tra ngày có phải là ngày làm việc không
    public static boolean isBusinessDay(LocalDate date) {
        DayOfWeek dayOfWeek = date.getDayOfWeek();
        return !(dayOfWeek == DayOfWeek.SATURDAY || dayOfWeek == DayOfWeek.SUNDAY);
    }
    
    // Tính ngày làm việc tiếp theo
    public static LocalDate nextBusinessDay(LocalDate date) {
        LocalDate nextDay = date.plusDays(1);
        while (!isBusinessDay(nextDay)) {
            nextDay = nextDay.plusDays(1);
        }
        return nextDay;
    }
    
    // Tính ngày làm việc trước đó
    public static LocalDate previousBusinessDay(LocalDate date) {
        LocalDate prevDay = date.minusDays(1);
        while (!isBusinessDay(prevDay)) {
            prevDay = prevDay.minusDays(1);
        }
        return prevDay;
    }
    
    // Tính số ngày làm việc giữa hai ngày
    public static long businessDaysBetween(LocalDate startDate, LocalDate endDate) {
        LocalDate currentDate = startDate;
        long businessDays = 0;
        
        while (currentDate.isBefore(endDate)) {
            if (isBusinessDay(currentDate)) {
                businessDays++;
            }
            currentDate = currentDate.plusDays(1);
        }
        
        return businessDays;
    }
    
    // Sử dụng TemporalAdjuster để tính ngày làm việc
    public static TemporalAdjuster nextBusinessDayAdjuster() {
        return temporal -> {
            LocalDate date = LocalDate.from(temporal);
            do {
                date = date.plusDays(1);
            } while (!isBusinessDay(date));
            return temporal.with(date);
        };
    }
    
    public static void main(String[] args) {
        LocalDate today = LocalDate.now();
        System.out.println("Today: " + today);
        System.out.println("Next business day: " + nextBusinessDay(today));
        System.out.println("Previous business day: " + previousBusinessDay(today));
        
        // Sử dụng TemporalAdjuster
        LocalDate nextBusiness = today.with(nextBusinessDayAdjuster());
        System.out.println("Next business day (using adjuster): " + nextBusiness);
    }
}
```

### 16. Stream API và Java Reflection

#### 16.1. Tổng quan về `Stream API`

**1. Giới thiệu về Stream API**

Stream API được giới thiệu trong Java 8, cung cấp một cách mới để xử lý tập hợp dữ liệu theo phong cách functional programming.

**Đặc điểm chính:**
- Không thay đổi nguồn dữ liệu gốc
- Có thể xử lý tuần tự hoặc song song
- Hỗ trợ lazy evaluation (đánh giá lười)
- Có thể kết hợp nhiều thao tác với nhau
- Tích hợp với lambda expressions

**2. Các thành phần chính của Stream API**

- **Source**: Nguồn dữ liệu (Collection, Array, I/O channel, v.v.)
- **Intermediate operations**: Các thao tác trung gian (filter, map, sorted, v.v.)
- **Terminal operations**: Các thao tác kết thúc (forEach, collect, reduce, v.v.)

**3. Ví dụ cơ bản**

```java
import java.util.*;
import java.util.stream.*;

public class StreamBasicExamples {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("John", "Jane", "Adam", "Eve", "Michael");
        
        // Filter và forEach
        System.out.println("Names starting with J:");
        names.stream()
             .filter(name -> name.startsWith("J"))
             .forEach(System.out::println);
             
        // Map và collect
        List<String> upperCaseNames = names.stream()
                                          .map(String::toUpperCase)
                                          .collect(Collectors.toList());
        System.out.println("\nUpper case names: " + upperCaseNames);
        
        // Sorted
        List<String> sortedNames = names.stream()
                                       .sorted()
                                       .collect(Collectors.toList());
        System.out.println("\nSorted names: " + sortedNames);
        
        // Chaining operations
        long count = names.stream()
                          .filter(name -> name.length() > 3)
                          .map(String::toUpperCase)
                          .sorted()
                          .count();
        System.out.println("\nCount of names with length > 3: " + count);
    }
}
```

**4. Intermediate Operations (Thao tác trung gian)**

| Operation | Mô tả | Ví dụ |
| --- | --- | --- |
| `filter(Predicate)` | Lọc các phần tử dựa trên điều kiện | `stream.filter(x -> x > 5)` |
| `map(Function)` | Chuyển đổi mỗi phần tử | `stream.map(String::toUpperCase)` |
| `flatMap(Function)` | Chuyển đổi và làm phẳng stream | `stream.flatMap(list -> list.stream())` |
| `distinct()` | Loại bỏ phần tử trùng lặp | `stream.distinct()` |
| `sorted()` | Sắp xếp các phần tử | `stream.sorted()` |
| `sorted(Comparator)` | Sắp xếp với comparator tùy chỉnh | `stream.sorted(Comparator.reverseOrder())` |
| `peek(Consumer)` | Thực hiện hành động trên mỗi phần tử | `stream.peek(System.out::println)` |
| `limit(long)` | Giới hạn số phần tử | `stream.limit(5)` |
| `skip(long)` | Bỏ qua số phần tử | `stream.skip(2)` |

**5. Terminal Operations (Thao tác kết thúc)**

| Operation | Mô tả | Ví dụ |
| --- | --- | --- |
| `forEach(Consumer)` | Thực hiện hành động trên mỗi phần tử | `stream.forEach(System.out::println)` |
| `toArray()` | Chuyển thành mảng | `stream.toArray()` |
| `reduce(BinaryOperator)` | Kết hợp các phần tử thành một giá trị | `stream.reduce((a, b) -> a + b)` |
| `collect(Collector)` | Thu thập kết quả vào collection | `stream.collect(Collectors.toList())` |
| `min(Comparator)` | Tìm giá trị nhỏ nhất | `stream.min(Comparator.naturalOrder())` |
| `max(Comparator)` | Tìm giá trị lớn nhất | `stream.max(Comparator.naturalOrder())` |
| `count()` | Đếm số phần tử | `stream.count()` |
| `anyMatch(Predicate)` | Kiểm tra có phần tử nào thỏa mãn | `stream.anyMatch(x -> x > 5)` |
| `allMatch(Predicate)` | Kiểm tra tất cả phần tử thỏa mãn | `stream.allMatch(x -> x > 0)` |
| `noneMatch(Predicate)` | Kiểm tra không có phần tử nào thỏa mãn | `stream.noneMatch(x -> x < 0)` |
| `findFirst()` | Lấy phần tử đầu tiên | `stream.findFirst()` |
| `findAny()` | Lấy bất kỳ phần tử nào | `stream.findAny()` |

**6. Collectors - Thu thập kết quả**

```java
import java.util.*;
import java.util.stream.*;
import static java.util.stream.Collectors.*;

public class StreamCollectorsExamples {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("John", "Jane", "Adam", "Eve", "Michael", "Emma");
        
        // Collect vào List
        List<String> list = names.stream()
                                .filter(n -> n.length() > 3)
                                .collect(Collectors.toList());
        
        // Collect vào Set
        Set<String> set = names.stream()
                              .filter(n -> n.length() > 3)
                              .collect(Collectors.toSet());
        
        // Collect vào Map
        Map<String, Integer> map = names.stream()
                                       .collect(Collectors.toMap(
                                           Function.identity(), 
                                           String::length
                                       ));
        
        // Grouping by
        Map<Integer, List<String>> groupedByLength = names.stream()
                                                        .collect(groupingBy(String::length));
        
        // Partitioning by
        Map<Boolean, List<String>> partitionedByLength = names.stream()
                                                            .collect(partitioningBy(n -> n.length() > 3));
        
        // Summarizing
        IntSummaryStatistics stats = names.stream()
                                         .collect(summarizingInt(String::length));
        System.out.println("Count: " + stats.getCount());
        System.out.println("Average: " + stats.getAverage());
        System.out.println("Max: " + stats.getMax());
        
        // Joining
        String joined = names.stream()
                            .collect(joining(", ", "Names: ", "."));
        
        // Collecting andThen
        List<String> upperCaseList = names.stream()
                                        .collect(collectingAndThen(toList(), list -> {
                                            list.forEach(String::toUpperCase);
                                            return list;
                                        }));
    }
}
```

**7. Parallel Streams - Xử lý song song**

```java
import java.util.*;
import java.util.stream.*;

public class ParallelStreamExample {
    public static void main(String[] args) {
        List<Integer> numbers = new ArrayList<>();
        for (int i = 0; i < 1000000; i++) {
            numbers.add(i);
        }
        
        // Sequential stream
        long startSeq = System.currentTimeMillis();
        int sumSeq = numbers.stream()
                           .mapToInt(Integer::intValue)
                           .sum();
        long timeSeq = System.currentTimeMillis() - startSeq;
        System.out.println("Sequential sum: " + sumSeq + " took " + timeSeq + "ms");
        
        // Parallel stream
        long startPar = System.currentTimeMillis();
        int sumPar = numbers.parallelStream()
                           .mapToInt(Integer::intValue)
                           .sum();
        long timePar = System.currentTimeMillis() - startPar;
        System.out.println("Parallel sum: " + sumPar + " took " + timePar + "ms");
        
        // Khi nào nên sử dụng parallel stream:
        // - Dữ liệu lớn
        // - Các thao tác tốn nhiều CPU
        // - Các phần tử độc lập với nhau
        
        // Khi nào không nên sử dụng:
        // - Dữ liệu nhỏ
        // - Các thao tác đơn giản
        // - Cần thứ tự cụ thể
        // - Có side effects
    }
}
```

**8. Best Practices khi sử dụng Stream API**

- **Sử dụng stream khi xử lý tập hợp dữ liệu**
- **Tránh sử dụng stream cho các thao tác đơn giản**
- **Không sử dụng stream để thay đổi trạng thái bên ngoài**
- **Sử dụng method references khi có thể (`String::toUpperCase`)**
- **Chú ý hiệu suất với parallel stream**
- **Tránh lạm dụng chaining quá nhiều operations**
- **Sử dụng Optional cẩn thận với findFirst/findAny**
- **Không sử dụng stream để thay thế vòng lặp đơn giản**

#### 16.2. Java Reflection

**1. Giới thiệu về Java Reflection**

Java Reflection là API cho phép chương trình kiểm tra và thay đổi cấu trúc và hành vi của các class, method, field tại thời điểm chạy.

**Ưu điểm:**
- Linh hoạt, có thể làm việc với các class không biết trước
- Hỗ trợ framework và thư viện mạnh mẽ
- Cho phép tạo proxy, DI containers, ORM frameworks

**Nhược điểm:**
- Hiệu suất thấp hơn so với code bình thường
- Có thể phá vỡ encapsulation
- Không an toàn nếu sử dụng không cẩn thận
- Khó debug và maintain

**2. Các lớp chính trong Reflection API**

- `Class`: Đại diện cho một class hoặc interface
- `Method`: Đại diện cho một phương thức
- `Field`: Đại diện cho một trường (field)
- `Constructor`: Đại diện cho một constructor
- `Modifier`: Cung cấp thông tin về access modifier

**3. Ví dụ cơ bản**

```java
import java.lang.reflect.*;

public class ReflectionBasicExamples {
    public static void main(String[] args) throws Exception {
        // Lấy Class object
        Class<?> clazz = Class.forName("java.util.ArrayList");
        
        // Lấy thông tin class
        System.out.println("Class name: " + clazz.getName());
        System.out.println("Simple name: " + clazz.getSimpleName());
        System.out.println("Package: " + clazz.getPackage());
        System.out.println("Superclass: " + clazz.getSuperclass());
        
        // Lấy danh sách các method
        Method[] methods = clazz.getDeclaredMethods();
        System.out.println("\nMethods:");
        for (Method method : methods) {
            System.out.println("- " + method.getName());
        }
        
        // Lấy danh sách các field
        Field[] fields = clazz.getDeclaredFields();
        System.out.println("\nFields:");
        for (Field field : fields) {
            System.out.println("- " + field.getName());
        }
        
        // Lấy danh sách các constructor
        Constructor<?>[] constructors = clazz.getConstructors();
        System.out.println("\nConstructors:");
        for (Constructor<?> constructor : constructors) {
            System.out.println("- " + constructor);
        }
        
        // Tạo instance mới
        Object instance = clazz.newInstance();
        
        // Gọi method thông qua reflection
        Method addMethod = clazz.getMethod("add", Object.class);
        addMethod.invoke(instance, "Hello");
        addMethod.invoke(instance, "World");
        
        // Truy cập field private
        Field sizeField = clazz.getDeclaredField("size");
        sizeField.setAccessible(true); // Bỏ qua kiểm tra access
        int size = (int) sizeField.get(instance);
        System.out.println("\nSize: " + size);
    }
}
```

**4. Truy cập và thay đổi field private**

```java
import java.lang.reflect.Field;

class Person {
    private String name;
    private int age;
    
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
    
    @Override
    public String toString() {
        return "Person{name='" + name + "', age=" + age + "}";
    }
}

public class ReflectionPrivateFieldExample {
    public static void main(String[] args) throws Exception {
        Person person = new Person("John", 30);
        System.out.println("Before: " + person);
        
        // Truy cập field private
        Field nameField = Person.class.getDeclaredField("name");
        Field ageField = Person.class.getDeclaredField("age");
        
        // Cho phép truy cập field private
        nameField.setAccessible(true);
        ageField.setAccessible(true);
        
        // Đọc giá trị field
        String name = (String) nameField.get(person);
        int age = (int) ageField.get(person);
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        
        // Thay đổi giá trị field
        nameField.set(person, "Jane");
        ageField.set(person, 25);
        
        System.out.println("After: " + person);
    }
}
```

**5. Gọi method private**

```java
import java.lang.reflect.Method;

class Calculator {
    private int add(int a, int b) {
        return a + b;
    }
    
    private String formatResult(int result) {
        return "Result: " + result;
    }
}

public class ReflectionPrivateMethodExample {
    public static void main(String[] args) throws Exception {
        Calculator calculator = new Calculator();
        
        // Lấy method private
        Method addMethod = Calculator.class.getDeclaredMethod("add", int.class, int.class);
        Method formatMethod = Calculator.class.getDeclaredMethod("formatResult", int.class);
        
        // Cho phép truy cập method private
        addMethod.setAccessible(true);
        formatMethod.setAccessible(true);
        
        // Gọi method và lấy kết quả
        int sum = (int) addMethod.invoke(calculator, 5, 7);
        String formatted = (String) formatMethod.invoke(calculator, sum);
        
        System.out.println(formatted); // Output: Result: 12
    }
}
```

**6. Tạo instance với constructor có tham số**

```java
import java.lang.reflect.Constructor;

class Product {
    private String name;
    private double price;
    
    public Product(String name, double price) {
        this.name = name;
        this.price = price;
    }
    
    @Override
    public String toString() {
        return "Product{name='" + name + "', price=" + price + "}";
    }
}

public class ReflectionConstructorExample {
    public static void main(String[] args) throws Exception {
        // Lấy constructor với tham số
        Constructor<Product> constructor = Product.class
            .getConstructor(String.class, double.class);
        
        // Tạo instance mới
        Product product = constructor.newInstance("Laptop", 999.99);
        System.out.println(product);
        
        // Lấy tất cả constructors
        Constructor<?>[] constructors = Product.class.getConstructors();
        System.out.println("\nAll constructors:");
        for (Constructor<?> c : constructors) {
            System.out.println(c);
        }
    }
}
```

**7. Best Practices khi sử dụng Reflection**

- **Tránh sử dụng reflection khi không cần thiết** - chỉ dùng khi thực sự cần
- **Cache các đối tượng reflection** (Method, Field, Constructor) để tăng hiệu suất
- **Xử lý exception cẩn thận** - reflection ném nhiều loại exception
- **Cân nhắc hiệu suất** - reflection chậm hơn method call bình thường
- **Không sử dụng reflection để phá vỡ encapsulation** không cần thiết
- **Sử dụng SecurityManager** nếu cần hạn chế quyền truy cập
- **Document rõ ràng** khi sử dụng reflection trong code

**8. Ứng dụng thực tế của Reflection**

- Frameworks như Spring (Dependency Injection)
- ORM frameworks như Hibernate
- Unit testing frameworks như JUnit
- Serialization/deserialization libraries
- Proxy pattern implementation
- Plugin systems
- Dynamic class loading

**9. Ví dụ thực tế: Dependency Injection đơn giản**

```java
import java.lang.reflect.*;
import java.util.*;

// Annotation để đánh dấu field cần inject
@interface Inject {}

// Lớp service
class EmailService {
    public void sendEmail(String to, String message) {
        System.out.println("Sending email to " + to + ": " + message);
    }
}

// Lớp client
class NotificationService {
    @Inject
    private EmailService emailService;
    
    public void notifyUser(String userId, String message) {
        emailService.sendEmail(userId + "@example.com", message);
    }
}

// Simple DI Container
class SimpleContainer {
    private Map<Class<?>, Object> instances = new HashMap<>();
    
    public SimpleContainer() {
        // Đăng ký các instance
        instances.put(EmailService.class, new EmailService());
    }
    
    public <T> T getInstance(Class<T> clazz) throws Exception {
        T instance = (T) clazz.newInstance();
        
        // Inject các dependency
        for (Field field : clazz.getDeclaredFields()) {
            if (field.isAnnotationPresent(Inject.class)) {
                field.setAccessible(true);
                Object dependency = instances.get(field.getType());
                if (dependency != null) {
                    field.set(instance, dependency);
                }
            }
        }
        
        return instance;
    }
}

public class ReflectionDIExample {
    public static void main(String[] args) throws Exception {
        SimpleContainer container = new SimpleContainer();
        NotificationService service = container.getInstance(NotificationService.class);
        service.notifyUser("john", "Your account has been created");
    }
}
```

### 17. Regular Expressions (Biểu thức chính quy)

**1. Giới thiệu về Regular Expressions**

Biểu thức chính quy (Regular Expressions - regex) là một chuỗi ký tự định nghĩa mẫu tìm kiếm, được sử dụng để tìm kiếm, thay thế hoặc phân tích chuỗi.

**Ứng dụng:**
- Xác thực đầu vào (email, số điện thoại, v.v.)
- Tìm kiếm và thay thế trong văn bản
- Phân tích cú pháp (parsing)
- Tách dữ liệu từ chuỗi

**2. Các thành phần cơ bản của regex**

- **Ký tự thông thường**: a, b, c, 1, 2, 3
- **Ký tự đặc biệt**: . ^ $ * + ? { } [ ] \ | ( )
- **Character classes**: [abc], [^abc], [a-z], \d, \w, \s
- **Quantifiers**: *, +, ?, {n}, {n,}, {n,m}
- **Anchors**: ^, $, \b
- **Groups và capturing**: ( ), (?: ), (?<name> )

**3. Các pattern thường dùng**

| Pattern | Mô tả | Ví dụ khớp |
| --- | --- | --- |
| `\d` | Ký tự số (0-9) | "1", "2", "3" |
| `\D` | Không phải ký tự số | "a", "B", "@" |
| `\w` | Ký tự chữ số hoặc gạch dưới (a-z, A-Z, 0-9, _) | "a", "Z", "5", "_" |
| `\W` | Không phải ký tự chữ số hoặc gạch dưới | "@", "$", " " |
| `\s` | Khoảng trắng (space, tab, newline) | " ", "\t", "\n" |
| `\S` | Không phải khoảng trắng | "a", "1", "@" |
| `.` | Bất kỳ ký tự nào (trừ newline) | "a", "1", "$" |
| `^` | Bắt đầu chuỗi | "^Hello" khớp "Hello world" |
| `$` | Kết thúc chuỗi | "world$" khớp "Hello world" |
| `\b` | Biên từ | "\bword\b" khớp "a word here" |
| `\B` | Không phải biên từ | "\Bword\B" khớp "keyword" |
| `*` | 0 hoặc nhiều lần | "a*" khớp "", "a", "aa" |
| `+` | 1 hoặc nhiều lần | "a+" khớp "a", "aa" |
| `?` | 0 hoặc 1 lần | "a?" khớp "", "a" |
| `{n}` | Đúng n lần | "a{3}" khớp "aaa" |
| `{n,}` | Ít nhất n lần | "a{2,}" khớp "aa", "aaa" |
| `{n,m}` | Từ n đến m lần | "a{2,4}" khớp "aa", "aaa", "aaaa" |
| `[abc]` | Một trong các ký tự a, b, c | "a", "b", "c" |
| `[^abc]` | Không phải a, b, c | "d", "1", "$" |
| `[a-z]` | Ký tự thường từ a đến z | "a", "m", "z" |
| `[A-Z]` | Ký tự hoa từ A đến Z | "A", "M", "Z" |
| `[0-9]` | Số từ 0 đến 9 | "0", "5", "9" |

**4. Ví dụ cơ bản**

```java
import java.util.regex.*;

public class RegexBasicExamples {
    public static void main(String[] args) {
        // Kiểm tra chuỗi khớp pattern
        System.out.println("1. Simple match:");
        System.out.println("a".matches("a")); // true
        System.out.println("abc".matches("abc")); // true
        System.out.println("ab".matches("abc")); // false
        
        // Sử dụng ký tự đặc biệt
        System.out.println("\n2. Special characters:");
        System.out.println("a".matches(".")); // true (bất kỳ ký tự nào)
        System.out.println("1".matches("\\d")); // true (ký tự số)
        System.out.println("a".matches("\\D")); // true (không phải số)
        System.out.println(" ".matches("\\s")); // true (khoảng trắng)
        
        // Quantifiers
        System.out.println("\n3. Quantifiers:");
        System.out.println("".matches("a*")); // true (0 hoặc nhiều 'a')
        System.out.println("a".matches("a*")); // true
        System.out.println("aaa".matches("a*")); // true
        System.out.println("a".matches("a+")); // true (1 hoặc nhiều 'a')
        System.out.println("".matches("a+")); // false
        System.out.println("a".matches("a?")); // true (0 hoặc 1 'a')
        System.out.println("aa".matches("a?")); // false
        
        // Character classes
        System.out.println("\n4. Character classes:");
        System.out.println("a".matches("[abc]")); // true (một trong a,b,c)
        System.out.println("d".matches("[abc]")); // false
        System.out.println("a".matches("[^abc]")); // false (không phải a,b,c)
        System.out.println("d".matches("[^abc]")); // true
        System.out.println("a".matches("[a-z]")); // true (chữ thường)
        System.out.println("A".matches("[a-z]")); // false
        System.out.println("A".matches("[A-Z]")); // true (chữ hoa)
        
        // Anchors
        System.out.println("\n5. Anchors:");
        System.out.println("hello".matches("^h")); // false (phải khớp toàn bộ)
        System.out.println("hello".matches("^hello$")); // true
        System.out.println("hello world".matches("^hello")); // true (bắt đầu bằng hello)
        System.out.println("hello world".matches("world$")); // false
        System.out.println("hello world".matches(".*world$")); // true (kết thúc bằng world)
    }
}
```

**5. Sử dụng Pattern và Matcher**

```java
import java.util.regex.*;

public class RegexPatternMatcher {
    public static void main(String[] args) {
        String text = "Contact us at support@example.com or sales@company.co.uk";
        
        // Tạo pattern cho email
        Pattern emailPattern = Pattern.compile("[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}");
        
        // Tạo matcher
        Matcher matcher = emailPattern.matcher(text);
        
        // Tìm tất cả các email
        System.out.println("Found emails:");
        while (matcher.find()) {
            System.out.println("- " + matcher.group());
            System.out.println("  Start: " + matcher.start() + ", End: " + matcher.end());
        }
        
        // Ví dụ về thay thế
        String replaced = text.replaceAll("[a-zA-Z0-9._%+-]+@", "****@");
        System.out.println("\nAfter replacement: " + replaced);
        
        // Ví dụ về split
        String[] parts = text.split("@");
        System.out.println("\nSplit result:");
        for (String part : parts) {
            System.out.println("- " + part);
        }
        
        // Ví dụ về validating
        String email = "user@example.com";
        boolean isValid = email.matches("[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}");
        System.out.println("\nIs valid email: " + isValid);
    }
}
```

**6. Các pattern thông dụng trong thực tế**

```java
import java.util.regex.*;

public class CommonRegexPatterns {
    public static void main(String[] args) {
        // Email validation
        String emailRegex = "^[a-zA-Z0-9_!#$%&'*+/=?`{|}~^.-]+@[a-zA-Z0-9.-]+$";
        System.out.println("Email validation:");
        System.out.println("test@example.com: " + "test@example.com".matches(emailRegex));
        System.out.println("invalid-email: " + "invalid-email".matches(emailRegex));
        
        // Phone number (simple)
        String phoneRegex = "^\\+?[0-9. ()-]{7,25}$";
        System.out.println("\nPhone number validation:");
        System.out.println("+1 (123) 456-7890: " + "+1 (123) 456-7890".matches(phoneRegex));
        System.out.println("1234567: " + "1234567".matches(phoneRegex));
        
        // Password strength (at least 8 chars, 1 uppercase, 1 lowercase, 1 digit)
        String passwordRegex = "^(?=.*[0-9])(?=.*[a-z])(?=.*[A-Z])(?=\\S+$).{8,}$";
        System.out.println("\nPassword validation:");
        System.out.println("Password123: " + "Password123".matches(passwordRegex));
        System.out.println("weak: " + "weak".matches(passwordRegex));
        
        // Date (YYYY-MM-DD)
        String dateRegex = "^\\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$";
        System.out.println("\nDate validation:");
        System.out.println("2023-12-25: " + "2023-12-25".matches(dateRegex));
        System.out.println("2023-13-01: " + "2023-13-01".matches(dateRegex));
        
        // URL
        String urlRegex = "^(https?://)?([\\da-z.-]+)\\.([a-z.]{2,6})([/\\w .-]*)*/?$";
        System.out.println("\nURL validation:");
        System.out.println("https://example.com: " + "https://example.com".matches(urlRegex));
        System.out.println("invalid-url: " + "invalid-url".matches(urlRegex));
        
        // HTML tag
        String htmlTagRegex = "<[a-zA-Z0-9]+.*?>.*?</[a-zA-Z0-9]+>|<[a-zA-Z0-9]+.*?/>";
        System.out.println("\nHTML tag validation:");
        System.out.println("<div>Hello</div>: " + "<div>Hello</div>".matches(htmlTagRegex));
        System.out.println("<img src=\"image.jpg\">: " + "<img src=\"image.jpg\">".matches(htmlTagRegex));
    }
}
```

**7. Best Practices khi sử dụng Regular Expressions**

- **Sử dụng regex khi cần thiết**, tránh lạm dụng vì có thể làm code khó đọc và hiệu suất thấp
- **Test kỹ regex** với nhiều trường hợp đầu vào khác nhau
- **Sử dụng Pattern.compile()** để cache pattern nếu sử dụng nhiều lần
- **Tránh catastrophic backtracking** với các pattern phức tạp
- **Document regex** rõ ràng vì chúng thường khó hiểu
- **Sử dụng các thư viện hỗ trợ** cho các pattern phổ biến (ví dụ: URL validation)

**8. Ví dụ thực tế: Xác thực email**

```java
import java.util.regex.*;

public class EmailValidator {
    // Pattern cho email hợp lệ
    private static final String EMAIL_REGEX = 
        "^[a-zA-Z0-9_!#$%&'*+/=?`{|}~^.-]+@[a-zA-Z0-9.-]+$";
    
    private static final Pattern pattern = Pattern.compile(EMAIL_REGEX);
    
    public static boolean isValidEmail(String email) {
        if (email == null) {
            return false;
        }
        
        // Kiểm tra độ dài
        if (email.length() > 254) {
            return false;
        }
        
        // Tách local part và domain
        String[] parts = email.split("@");
        if (parts.length != 2) {
            return false;
        }
        
        // Kiểm tra local part (phần trước @)
        String localPart = parts[0];
        if (localPart.length() > 64) {
            return false;
        }
        
        // Kiểm tra domain (phần sau @)
        String domain = parts[1];
        String[] domainParts = domain.split("\\.");
        if (domainParts.length < 2) {
            return false;
        }
        
        // Kiểm tra regex
        Matcher matcher = pattern.matcher(email);
        return matcher.matches();
    }
    
    public static void main(String[] args) {
        String[] testEmails = {
            "user@example.com",
            "user.name+tag+sorting@example.com",
            "user@sub.example.com",
            "user@123.123.123.123",
            "user@[IPv6:2001:db8::1]",
            "plainaddress", // Invalid
            "@no-local-part.com", // Invalid
            "no-at.example.com", // Invalid
            "user@.invalid.com", // Invalid
            "user@com", // Invalid
            "user@localserver" // Invalid
        };
        
        for (String email : testEmails) {
            System.out.println(email + " is " + (isValidEmail(email) ? "valid" : "invalid"));
        }
    }
}
```

**9. Lưu ý quan trọng về hiệu suất**

- Regex có thể gây ra **catastrophic backtracking** với các pattern phức tạp
- Nên **compile pattern một lần** và sử dụng lại nếu có thể
- Tránh sử dụng regex cho các chuỗi rất dài
- Xem xét sử dụng phương pháp khác nếu regex quá phức tạp

```java
// Tốt: Compile pattern một lần và sử dụng lại
Pattern emailPattern = Pattern.compile(EMAIL_REGEX);
Matcher matcher = emailPattern.matcher(email);
boolean isValid = matcher.matches();

// Xấu: Compile pattern mỗi lần sử dụng
boolean isValid = email.matches(EMAIL_REGEX);
```