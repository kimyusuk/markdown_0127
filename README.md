# markdown_0127
마크다운 설명


### 11. 테이블 표 만들기
콜론 왼쪽 왼쪽 정렬  
콜론 오른쪽 오른쪽 정렬  
콜론 양쪽 가운데 정렬  
|번호|아이디|이름|레벨|이메일|등록일|
|:--------|:--------|:--------|---------:|:--------|:--------:|
|1|airheart0422|김둥이|192|airheart0422@naver.com|2023-01-27
|2|airheart0422|김둥이|192|airheart0422@naver.com|2023-01-27
|3|airheart0422|김둥이|192|airheart0422@naver.com|2023-01-27
|4|airheart0422|김둥이|777777|airheart0422@naver.com|2023-01-27
|5|airheart0422|김둥이|4444|airheart0422@naver.com|2023-01-27
|6|airheart0422|김둥이|100000|airheart0422@naver.com|2023-01-27


### 10. 인라인 코드
블럭코드랑 다르게 한줄짜리 코드를 뜻한다.  
문단 중간에 `CODE`를 넣을 수 있습니다.  
`question_list = Question.objects.order_by("-create_date")`  
고정형 폭 폰트로 표시해야할 때 사용한다.


### 9. 강조
**spring**을 만끽하세요.  
*spring*을 만끽하세요.

### 8. 이미지 넣기
![파이참](https://github.com/kimyusuk/markdown_0127/blob/main/%EB%A7%88%ED%81%AC%EC%88%98%EC%97%85/%EC%BA%A1%EC%B2%98.PNG "파이참 설명 / 파이참 툴팁")


### 7. 하이퍼 링크
[e클래스](https://cafe.daum.net/pcwk "e 클래스의 cafe 입니다.")


### 6. 가로 라인
---
***
-----

### 5. 코드블록
```
빽코트는 엔터가 자동으로 들어와진다.
def index(request):
    # return HttpResponse("Hello pybo에 안녕하세요.pybo")
    # list order create_date desc
    # order_by('-필드') = desc,order_by('필드') = asc
    question_list = Question.objects.order_by("-create_date")
    # question_list = Question.objects.filter(id=1)
    context = {"question_list":question_list} # list order creat_date desc
    # print("question_list:{}".format(question_list))
    return render (request,'pybo/question_list.html',context)
```

### 4. 모크로쿠
상위 하위 목록  
- 아이템 1  
+ 아이템 2  
  - 1단계 하위 아이템  
    * 2단계 하위 아이템  

1. 아이템 1  
2. 아이템 2  
  9. 단계 하위 아이템  
    3.1 단계 하위 아이템  
5. 아이템 


순서없는 목록  
* 목록이름
- 목록
+ 목록

순서있는 목록  
1. 목록이름
2. 목록
3. 목록
4. 모크로쿠

### 3. 인용문
> 문자 앞에 꺽새 넣고 인용할 내용을 넣으면 된다.  
> 빈 줄이 없으면 자동으로 인용 상자에 포함이 된다. 

### 2. 헤더
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5
즉 #이 헤더라는 뜻이다.


### 1.문단 구분을 위한 개행.
문단을 작성합니다.(개행은 공백 두개다.)  
겨울이 가고 봄이 옵니다.
