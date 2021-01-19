# REST-API_example


REST(Representational State Transfer) : HTTP 에서 필요한 자원에 접근할 때 웹의 장점을 최대한 활용하기 위한 아키텍쳐

REST API의 구성 요소
1. http Method
  * GET = 데이터 조회
  * POST = 새로운 데이터 추가
  * PUT = 데이터 전체 수정
  * PATCH = 데이터 일부 수정
  * DELETE = 정보 삭제
 
2. URL : 데이터 접근
3. Representation : 자원의 표현


REST API의 자원 표현을 위한 URL 설계 규칙
1. 소문자만 사용
2. 하이픈[-]은 사용하지 않고 밑줄[_]을 사용.
3. 확장자를 표시하지 않음.

---

## 실습 1. Google Books APIs with Vscode REST Client

https://developers.google.com/books/docs/v1/using


1. Vscode에서 REST Client 확장 설치하고 파일을 http 확장자로 만든다.

2. 책 저자 이름로 조회하기.
```
get https://www.googleapis.com/books/v1/volumes?q=inauthor=귀욤뮈소
```

* send Request를 클릭해보자.

<br>

결과 :
![저자](https://user-images.githubusercontent.com/43642411/105027943-bc40fc80-5a93-11eb-96ca-53d56f9581a6.PNG)

<br>

3. 책 고유번호인 isbn으로 조회하기.
```
get https://www.googleapis.com/books/v1/volumes?q=isbn=9791158883591
```



## 실습 2 YTS Movies APIs
* 영화 정보 리스트를 제공하는 API를 사용해보자.

조건을 추가하여 영화 조회

```
get https://yts.mx/api/v2/list_movies.json
 ?minimum_rating=8.5
 &sort_by=year
 &limit=5
 &genre=Sci-Fi
```

결과로 인터스텔라가 나왔습니다. <br> <br>
![인터](https://user-images.githubusercontent.com/43642411/105035113-d384e780-5a9d-11eb-8eba-c875b39a229a.PNG)


## 실습 3 API 인증을 위한 키를 발급 받아 사용. (developer console 활용)

[Kakao Developers](https://developers.kakao.com/)

[Kakao Map API Guide](https://apis.map.kakao.com/web/guide/)

![카카오지도](https://user-images.githubusercontent.com/43642411/105037102-d0d7c180-5aa0-11eb-82cd-4364c07921ce.PNG)



