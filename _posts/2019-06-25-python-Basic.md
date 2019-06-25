### Python

----

**mac jupyter note book 개발 환경 구축하기**



Anaconda(included python, Jupiter)Homepage

https://www.anaconda.com/

main page 최신 버전다운로드 완료 후 terminal 창 open



python 버전 확인 후 

`python —version`

쥬피터 노트북 open

`jupyter notebook`



`localhost:8888` 로 주소창 열림

---

**jupyter 단축키**

- run : shift+enter
- Cell add(upper) : a
- Cell add(down) : b
- 단축키 help : h
- markdown : m
- delete : x
- paste : v
- copy : c
- save : cmd + s
- source code 몇 번째 줄인지? : L



----

**python 언어 사용하기**



##### 변수명 규칙

> 1. 영문자, 숫자, 언더바 사용할 수 있다.
> 2. 숫자로 사용 불가능
> 3. 문법 keyword 사용 불가



##### 변수 대입

`a,b = 10, 15`

```python
a,b = 10, 15
s1 = s2 = "python"
```



##### 이스케이프 코드

```python
\n	#개행(줄 바꾼다.)
\r	#줄 바꾸면 문서 맨 앞에 커서 표시된다.
\"	#큰 따음표가 출력된다.
\'	#작은 따음표가 출력된다.
\t	#수평탭 표기된다.
//	#문자가 표기된다.
```



##### 주석

```python
'''
#
```



##### 문자열 인덱싱(List 활용)

```python
s= "Life is too short, You need python"
print(s[0:3]) //Life
print(s[12:17]) //Short
print(s[19:]) //python
print(s[:]) //Life is too short, You need python
```



##### 문자열 포매팅

```python
%s str
%c char
%d int //정수형
%f float
%.숫자f //소수점 아래 자리수

%x //16진수
%o //8진수
%% Literal%

#ex1
temp = 20
s = "지금 나이는 %d입니다"%temp
a = "00대학교 %d학년 %d학기"%(4,1)

#ex2
x=100
y=200
sum = x+y
print("%d와 %d의 합은 %d입니다."%(x,y,sum))
print("{}와 {}의 합은 {}입니다.".format(x,y,sum))

```



##### 문자열 함수

```python
s = "2019년 06월 25일 화요일 12:31"
s.count()

count("문자") //문자 개수 카운트
find("문자") //문자의 위치를 찾아줌, 없을시 -1
index("문자") //문자의 위치를 찾아줌, 없을시 error
join("문자") //문자 사이에 값넣기
upper() //소문자 > 대문자
lower() //대문자 > 소문자
lstrip() //왼쪽 공백 지우기
rstrip() //오른쪽 공백 지우기
strip() //모든 공백 지우기
replace("문자열1","문자열2") //문자열1을 문자열2로 바꾸기
split("문자") //문자 기준으로 문자열 나누기

```


*upper, lower, strip : 텍스트마이닝 전 단계인 데이터 전처리에 자주 사용