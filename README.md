# REST-API_example


REST(Representational State Transfer) : HTTP 에서 필요한 자원에 접근할 때 웹의 장점을 최대한 활용하기 위한 아키텍쳐


실습 1. Google Books APIs with Vscode REST Client

https://developers.google.com/books/docs/v1/using

REST API의 구성 요소
1. http Method
  * GET = 데이터 조회
  * POST = 새로운 데이터 추가
  * PUT = 데이터 전체 수정
  * PATCH = 데이터 일부 수정
  * DELETE = 정보 삭제
 
2. URL : 데이터 접근
3. Representation : 자원의 표현

---

Vscode에서 REST Client 확장 설치

1. 책 저자 이름로 조회하기
```
get https://www.googleapis.com/books/v1/volumes?q=inauthor=귀욤뮈소
```


결과 :
![저자](https://user-images.githubusercontent.com/43642411/105027943-bc40fc80-5a93-11eb-96ca-53d56f9581a6.PNG)
