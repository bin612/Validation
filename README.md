# Validation

validation 체크를 해주는 Annotation들이 존재한다.

@Email : 이메일 형식을 체크하는 Annotation 이다.

```java
@Email
    private String email;
````

@Pattern : 유효성 검사를 위해 사용을 했다.

```java
@Pattern(regexp = "^\\d{2,3}-\\d{3,4}-\\d{4}$", message = "핸드폰 번호의 양식과 맞지 않습니다. 01x-xxxx-xxxx ")
```
<br>

#### Custom Validation

<br>

1. AssertTrue / False 와 같은 method 지정을 통해서 Custom Logic 적용 가능 
 <br>

2. ConstraintValidation 를 적용하여 재사용이 가능한 Custom Logic 적용 가능

