
# 책 관리 시스템
- 도서관 비슷 (책 빌리기, 책 반납하기, 
책 등록하기, 책 비등록과정)
- 구조: 객체지향 중점 (함수랑 자료가 모인 객체들의 상호작용)
> 예. 도서관, 책, 저자, 독자

---


## 도서관
- 책 등록
- 책 등록 해제
- 대출
- 반납
- 회원 등록
- 회원 탈퇴

``` java
Set<Book> presentBooks;
Set<Book> borrowedBooks;
Set<Person> registeredMember;
```


## 책
- 제목, 저자, 출판사
- 책 등록할 때 title, author, publisher 무조건 써야 책을 등록할 수 있게 하기


``` java
String title;
String author;
String publisher;
Book(title, author, publisher);
```

ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ


## Person
- 이름, 나이, 성별, 주소 


``` java
String personName;
int age;
String gender;
String address;
```

ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

### 저자
- 저서

``` java
List <Book> onesBook;
```

ㅡㅡㅡㅡㅡ

### 독자
- 회원/비회원, 대출한 책 목록

``` java
List <Book> checkOutBooksList;
boolean MeberStatus;

```

- 회원 등록할 때 이름, 나이, 성별, 주소를 무조건 써야 회원 등록할 수 있게 하기
super(personName, age, gender, address);

- borrowedbooks를 없애고 boolean 값으로 대출했는지 반납했는지 확인하기
