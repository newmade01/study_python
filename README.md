기본
------------


**함수: 들여쓰기**
일반적으로 4개의 공백을 들여쓰기에 사용



 **import문**
 함수 라이브러리


| import종류  | 호출  | 비고|
| ------------ | ------------ |
| math  |  math.sqrt() ||
|random|random.random()|0과 1 사이의 값을 랜던 추출|

*외부모듈 사용방법 pip install (외부 모듈명)-> import (외부모듈명)

 **코멘트**
 '# ' 문자로 주석처리
 
 **PEP**
 Python Enhancement Prosals 
 파이썬 개선 제안서
 파이썬 코딩 관련 코딩표준문서
 
 
 **데이터타입**
 int, float, bool(0, 비어있음:거짓 ), None(Null과 같은 표현)
 
 **복소수** 
>  a+bj
j로 복소수 표현

 .real : 복소수명
 .img: 변수명
 
 

연산자
------------


 **: 제곱
 //: 나누기에 소수점 이하를 버림 Floor Division
 
 **논리연산자**
>  x=True
y=False
if x and y:
print("yes")
else:
print("no")

**Bitwise연산자**
**멤버쉽 연산자**
in, not in 우측 컬렉션에 속해 있는지 체크
> a="ABC"
b=3 in a
print(b)

**Identity연산자**
is , is not 동일한 object인지 체크


문자열
------------
''' 라인에 걸쳐서표현 OR \n 사용
\t, \", \\\\ 사용

**포맷팅**
> p="이름: **%s** 나이**:%d** " **%** ("김유신", 65)
print(p)




| Conversion Specifier  | 뜻 |
| ------------ | ------------ |
| %s  |  문자열 srt()사용하여 변환 |
|  %r |  문자열 repr() 사용하여 변환 |
|  %c | 문자char  |
|  %d, %i |  정수int |
|%f, %F   | 부동소수 float  |
|  %e, %E | 지수형 부동소수  |
|%g, %G|일반형|
|%o, %O|8진수|
|%x, %X|16진수|
|%%|퍼센트 리터럴|


**문자열 클래스**
type(s) : class 'str'
type(s[1]) 
r'문자열': raw String

**자주 사용되는 str**
- str.join(): 여러 개 문자를 하나도 결합, 결합 앞에 공백으로도 사용 가능
> s=','.join(['가나','다라','마바'])
print(s) 

출력:가나,다라,마바
- str.split(): seperator 기본으로 문자열 배열 분리
> itmes='가나,다라,마바'.split(',')
print (items)

출력:['가나', '다라', '마바']

- str.partition(): (prefix)+(separator)+(suffix) 3Tuple 
> departure="Seattle-Seoul".partition('-')
print(departure)

출력: Seattle

- srt.format(): 값을 지정하고 가져옴
> area=(10,2)
s="width:{x[0]}, he:{x[1]}".format(x=area)

