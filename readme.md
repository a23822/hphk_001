# 20181217에 배운 내용

## 위에꺼보다 좀더 작음 - 파이썬 기초

### ㅇㅇ - 1.카카오톡 챗봇 이용하기

##### 좀더좀더

###### 얘는 되나?

####### ㅇㅇㅇㅇㅇㅇㅇ



- 안녕 -하고 띄우기
- 카카오톡 챗봇 친구 추가하기
  - 탭누르면 됨. @sspy-003 검색하기
  - 친구추가하기
    - 다른 반들과 섞이지 ㅇ낳게 주의할 것
      - 가나다라
        - 마ㅏ사라\\



1. 미세먼지를 입력하면 강남구의 미세먼지 농도를 알 수 있다.

안녕 하세요   는 영어로 ` hi! `

```python
def cal():
    return a+b
```

"``` 세번하면 바꿔짐"

```swift
let abd = 10
var a = 10
```





1. 미세먼지는 미세먼지, 날씨는 날씨를 알 수 있다.
2. ㅇ
   1. ㄱ
      1. ㅇ ㄷㅂ
         1. ㄳ ㄷㅇㅆㅈㄴ

가. ㅁㄴㅇ

나. ㄷ랍ㅈㄷ

- 미세먼지 코드

**볼드처리** 

아스타리스크 는 띄어쓰기하면 안됨.

```python
#app.py

... 이 부분에서 전체를 말하지 않으면 ... 를 붙여주는 것이 관례.2
```

//링크는  [    ] ()

[이것은 링크입니다](https://www.naver.com)

![](http://tenasia.hankyung.com/webwp_kr/wp-content/uploads/2018/05/2018050412180760599-540x360.jpg)

// 링크 앞에 ! 달면ㄷ ㅚㅁ

이것은 문서입니다.

> 이것은 문서가 아닐 수도 있습니다.
>
> <이것은 책 제목> ㄴㅇ\
>
> > > >

|  가  |  나  |   다 |      |      |
| :--: | :--: | ---: | ---- | ---- |
|  마  |  바  |   사 |      |      |
|      |      |      |      |      |
|      |      |      |      |      |
|      |      |      |      |      |
|      |      |      |      |      |
|      |      |      |      |      |



## 미세먼지

&&

&

||

|

2개짜리는 전자 쪽이 false 일 경우 뒤 조건들을 처리하지 않고 바로 넘어감.

1개짜리는 모든 조건을 다 처리함.

```python
import requests
from bs4 import BeautifulSoup

url = 'http://openapi.airkorea.or.kr/openapi/services/rest/ArpltnInforInqireSvc/getCtprvnRltmMesureDnsty?sidoName=%EC%84%9C%EC%9A%B8&ServiceKey={}&ver=1.3&pageNo=3'.format(key)
response = requests.get(url).text
soup = BeautifulSoup(response, 'xml')
gn = soup('item')[7]
location = gn.stationName.text
time = gn.dataTime.text
dust = int(gn.pm10Value.text)

print('{0} 기준: 서울시 {1}의 미세먼지 농도는 {2} 입니다.'.format(time, location, dust))
condition = ""

if dust > 0 and dust < 30 :
  condition = "좋음"
elif dust > 30 and dust < 80 :
  condition = "보통"
elif dust > 80 and dust < 150 :
  condition = "나쁨"
else :
  condition = "매우 나쁨"

print("오늘의 미세먼지 농도는 " + condition + " 입니다.")
```



## 반복문

```python
//while
//조건이 true일때까지 반복적으로 작용
while true:
    print("앙")
    n = n + 1
    
//for
//범위를 정해서 반복 종료조건이 필요없음.
list = [1,2,3,4,5]
for i in list:
	print(i)
```



## ## 셀리니움

크롤링할때 씀.

