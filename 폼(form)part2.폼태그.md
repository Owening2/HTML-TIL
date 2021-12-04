[toc]

## form 

form 은 입력 요소들을 감싸며, 입력 값을 서버 측으로 제출(submit)할 수 있다.

![image-20211203202616200](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203202616200.png)



## form의 내용을 제출

form의 내용 (입력값) 을 제출하기 위해 input 태그의 submit 타입 사용 가능!

![image-20211203202708815](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203202708815.png)

**=> '로그인'버튼을 누르면 입력된 아이디와 비밀번호가 서버로 전송되고(요청), 서버 측에서 데이터를 처리한 결과를 클라이언트에게 보내준다(응답).**

 

## form의 속성

action : 입력값을 전송할 서버의 url

method :  클라이언트가 입력한 데이터를 어떤 식으로 전송할지 (GET or POST)

![image-20211203202853748](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203202853748.png)

**=> 위 예제는**

- example.php 라는 서버 프로그램으로 입력값을 전송하여 요청할 것이다.
- POST 방식으로 전송할 것이다.



## GET vs POST

GET : 서버에 요청을 보내어 응답을 받아낸다.

서버로부터 정보를 '가져오겠다'는 성격의 요청이다.



POST : 서버에 요청을 보내어 작업을 수행한다.

서버에 있는 데이터를 추가/수정/삭제 한 후에 응답을 받아낸다.

서버의 정보를 '조작하겠다' 는 성격의 요청이다.



### 실습

```html
<! DOCTYPE html>
<html>
    <head>
        <meta charset = "utf-8">
        <title>서버에 요청을 보내자, 폼!</title>
    </head>
    <body>
        <h1> 키우고 싶은 동물 고르기</h1>
        <form action = "exam.php" method = "POST">
            <input type = "text" placeholder = "NAME" name = "name">
            <br>
            <select name = "pet">
                <option value = "dog">강아지</option>
                <option value = "cat">고양이</option>
                <option value = "parrot">앵무새</option>
            </select>
        </form>
    </body>
</html>
```





