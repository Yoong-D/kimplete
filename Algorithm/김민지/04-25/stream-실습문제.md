### 실습 문제 1: 숫자 배열 처리
주어진 정수 배열에서 짝수만을 찾아 그 합을 구하시오.

**예시 입력**
```java
int[] numbers = {3, 10, 4, 17, 6};
```
**예시 출력**
```java
20
```

### 실습 문제 2: 문자열 리스트 필터링
주어진 문자열 리스트에서 길이가 5 이상인 문자열만을 선택하여 대문자로 변환하고, 결과를 리스트로 반환하시오.

**예시 입력**
```java
List<String> words = Arrays.asList("apple", "banana", "cherry", "date");
```
**예시 출력**
```java
["APPLE", "BANANA", "CHERRY"]
```

### 실습 문제 3: 학생 성적 처리
학생 객체의 리스트가 주어졌을 때, 성적(score)이 80점 이상인 학생들만을 선택하고, 이들의 이름을 알파벳 순으로 정렬하여 출력하시오.

**예시 입력**
```java
List<Student> students = Arrays.asList(
    new Student("Alice", 82),
    new Student("Bob", 90),
    new Student("Charlie", 72),
    new Student("David", 76)
);
```
**예시 출력**
```java
["Alice", "Bob"]
```
**필요한 `Student` 클래스**
```java
public class Student {
    private String name;
    private int score;

    public Student(String name, int score) {
        this.name = name;
        this.score = score;
    }

    public String getName() {
        return name;
    }

    public int getScore() {
        return score;
    }
}
```

### 실습 문제 4: 직원 관리
직원 객체의 리스트에서 각 부서(department)별로 평균 급여를 계산하시오.

**예시 입력**
```java
List<Employee> employees = Arrays.asList(
    new Employee("Alice", "HR", 3000),
    new Employee("Bob", "HR", 2000),
    new Employee("Charlie", "Engineering", 5000),
    new Employee("David", "Engineering", 4000)
);
```
**예시 출력**
```java
HR: 2500.0
Engineering: 4500.0
```
**필요한 `Employee` 클래스**
```java
public class Employee {
    private String name;
    private String department;
    private double salary;

    public Employee(String name, String department, double salary) {
        this.name = name;
        this.department = department;
        this.salary = salary;
    }

    public String getDepartment() {
        return department;
    }

    public double getSalary() {
        return salary;
    }
}
```

여기 몇 가지 더 실습 문제를 제공해 드리겠습니다. 이 문제들은 자바의 Stream API를 사용하여 다양한 데이터 처리 요구 사항을 해결하는 데 초점을 맞추고 있습니다. 다양한 스트림 연산을 활용하여 문제를 해결해 보세요.

### 실습 문제 5: 제품 카테고리별 평균 가격 계산
주어진 제품 리스트에서 각 카테고리별로 평균 가격을 계산하시오.

**예시 입력**
```java
List<Product> products = Arrays.asList(
    new Product("Laptop", "Electronics", 1200.00),
    new Product("Smartphone", "Electronics", 700.00),
    new Product("Desk", "Furniture", 300.00),
    new Product("Chair", "Furniture", 150.00)
);
```
**예시 출력**
```java
Electronics: 950.0
Furniture: 225.0
```
**필요한 `Product` 클래스**
```java
public class Product {
    private String name;
    private String category;
    private double price;

    public Product(String name, String category, double price) {
        this.name = name;
        this.category = category;
        this.price = price;
    }

    public String getCategory() {
        return category;
    }

    public double getPrice() {
        return price;
    }
}
```

### 실습 문제 6: 나이대별 평균 점수 계산
학생 리스트에서 나이대별(10대, 20대 등)로 평균 점수를 계산하시오.

**예시 입력**
```java
List<Student> students = Arrays.asList(
    new Student("Alice", 14, 88),
    new Student("Bob", 23, 82),
    new Student("Charlie", 17, 95),
    new Student("David", 21, 73)
);
```
**예시 출력**
```java
10s: 91.5
20s: 77.5
```
**필요한 `Student` 클래스 (새 버전)**
```java
public class Student {
    private String name;
    private int age;
    private int score;

    public Student(String name, int age, int score) {
        this.name = name;
        this.age = age;
        this.score = score;
    }

    public int getAge() {
        return age;
    }

    public int getScore() {
        return score;
    }
}
```

### 실습 문제 7: 도시별 최고 온도 기록
여러 도시의 일일 최고 온도가 주어졌을 때, 각 도시의 최고 온도를 찾으시오.

**예시 입력**
```java
List<Temperature> temperatures = Arrays.asList(
    new Temperature("Seoul", 33),
    new Temperature("New York", 30),
    new Temperature("Seoul", 34),
    new Temperature("New York", 28)
);
```
**예시 출력**
```java
Seoul: 34
New York: 30
```
**필요한 `Temperature` 클래스**
```java
public class Temperature {
    private String city;
    private int maxTemp;

    public Temperature(String city, int maxTemp) {
        this.city = city;
        this.maxTemp = maxTemp;
    }

    public String getCity() {
        return city;
    }

    public int getMaxTemp() {
        return maxTemp;
    }
}
```