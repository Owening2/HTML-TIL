[toc]

## 보기 중에 골라보자

select 는 다수의 옵션(선택지)을 포함할 수 있는 선택 메뉴이다.

메뉴 안에 포함되는 옵션은 option 태그를 사용해 표시한다.

![image-20211203174202893](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203174202893.png)

**'cafe의 입력 값은 coffeebean이다'라는 결론!**



## textarea

textarea는 여러 줄의 일반 텍스트를 입력할 수 있는 입력 요소이다.

textarea 역시 name 을 추가하여 구별해줄 수 있는 입력 요소이다.

![image-20211203174318554](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203174318554.png)



### 실습

```html
<! DOCTYPE html>
<html>
    <head>
        <meta charset = "utf-8">
        <title>다양한 입력 요소 만들기</title>
    </head>
    <body>
        <h1>키우고 싶은 동물 고르기</h1>
        <select name = "pet" multiple>
            <option value = "dog">강아지</option>
            <option value = "cat" selected>고양이</option>
            <option value = "hamster">햄스터</option>
            <option value = "parrot">앵무새</option>
        </select>
        <br>
        
        <textarea name = "content"
                  rows = "10" cols = "10">기본적으로 쓰여 있는 텍스트</textarea>
    </body>
</html>

```



![image-20211203175227315](C:/Users/kazio/AppData/Roaming/Typora/typora-user-images/image-20211203175227315.png)





