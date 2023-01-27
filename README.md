# markdown_0127
마크다운 설명


### 8. 이미지 넣기
![리자몽]()


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
