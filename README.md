# LEWA

### 유노윤호 (2020.04 ~ 2020.06)

**2020년 1학기 스터디 상생플러스**

<img src = "https://user-images.githubusercontent.com/55044278/94947644-ee484600-0518-11eb-8c67-04d6a7754456.png" height = "250px">

----------

**주제** : 영어 단어 학습 사이트 (Learning English with Article)

**기획 배경** : 영어 기사를 활용하여 사용자 중심적으로 편리하게 영어를 공부하기 위해서

**팀원**

|                            이름                             |              역할              |                           책임                            |
| :---------------------------------------------------------: | :----------------------------: | :-------------------------------------------------------: |
|     [yoonho0922(안윤호)](https://github.com/yoonho0922)     |       Project Manager 👑        |                전체적인 프로젝트 관리 담당                |
|      [limjustin(임재영)](https://github.com/limjustin)      |         Back-end Coder         |               Server Side 기능 구현 및 관리               |
|    [ChaeheePark(박채희)](https://github.com/ChaeheePark)    |         Back-end Coder         |               Server Side 기능 구현 및 관리               |
| [hyejinHong0602(홍혜진)](https://github.com/hyejinHong0602) | UI Designer<br>Front-end Coder | 웹 사이트 UI Design 담당<br>Client Side 기능 구현 및 관리 |
|   [youngseo0526(김영서)](https://github.com/youngseo0526)   |        Front-end Coder         |               Client Side 기능 구현 및 관리               |
|         [polyn0(양정안)](https://github.com/polyn0)         |        Front-end Coder         |               Client Side 기능 구현 및 관리               |


----------

**1. 프로젝트 목적**

사용자가 영어 기사를 활용하여 자신만의 학습 컨텐츠를 만들어 공부할 수 있는 웹사이트를 개발하는 것

----------

**2. 기능**

- **회원가입 및 로그인** : 사용자 정보를 MongoDB에 등록 및 로그인 가능

- **기사 스크래핑** : 관리자 계정을 통해 기사 업로드 (제목, 본문, 썸네일)

- **영어 사전** : 모르는 단어의 한글 뜻과 예문 확인 가능

- **나만의 단어장** : 사용자가 중요하다고 생각하거나 어렵다고 생각한 단어들을 단어장에 저장 가능

- **단어 퀴즈** : 사용자가 만든 단어장을 기반으로 간단한 단어 퀴즈 수행

----------

**3. 상세 기능 다이어그램**

![image](https://user-images.githubusercontent.com/55044278/95486863-88533700-09ce-11eb-9cf3-eb1161882be9.png)
![image](https://user-images.githubusercontent.com/55044278/95486963-afaa0400-09ce-11eb-9528-1b952c28c08b.png)

----------

**4. 사용 프로그램**

- **Webstorm** : Meteor 구동 및 Javascript 코드 구현

- **MongoDB** : 기사 내용, 단어장 등 사이트에서 필요로 하는 정보들을 담아두는 곳

- **Kakao Oven** : 구체적인 UI 스케치


----------

**5. 웹사이트 실행 화면**

**회원가입 및 로그인 화면**

- 회원가입 시, ```이메일 / 비밀번호 / 비밀번호 확인``` 입력 과정을 거침

- 로그인 시, 사용자가 입력한 정보가 DB에 있는지 확인 후 로그인 여부 결정

![image](https://user-images.githubusercontent.com/55044278/95487602-80e05d80-09cf-11eb-956f-1bd2f9ffd5ef.png)

<br>

**기사 스크래핑 화면**

- 관리자 계정으로만 업로드 가능

- 기사의 URL만 붙여 넣으면 ```제목 / 본문 / 썸네일``` 항목이 자동으로 스크랩

![image](https://user-images.githubusercontent.com/55044278/95487683-9bb2d200-09cf-11eb-9bd1-c128ef701ec7.png)

![image](https://user-images.githubusercontent.com/55044278/95487696-9eadc280-09cf-11eb-8dcd-98c13e235aee.png)

<br>

**메인 화면**

- 당일 업로드 된 기사가 최신순으로 10개 표시

- 영단어 검색 창에서 검색한 단어의 빈도수를 가지고 My Words 차트를 제작

  - 사용자가 검색한 단어의 빈도수가 높은 순으로 정렬

- 기사 목록 화면에서는 날짜를 기준으로 기사 필터링 가능

![image](https://user-images.githubusercontent.com/55044278/95487849-cd2b9d80-09cf-11eb-81c7-01913f4dae5c.png)

![image](https://user-images.githubusercontent.com/55044278/95490405-26e19700-09d3-11eb-95fb-2d506d97601f.png)

<br>

**기사 본문 화면**

- 기사의 ```제목 / 썸네일 / 본문``` 표시

- 맨 아래 부분에는 기사의 원본 링크 포함

- 조회수, 업로드 날짜, 스크랩 버튼 확인 가능

- 우측에 영단어 검색 창 존재

![image](https://user-images.githubusercontent.com/55044278/95488065-0ebc4880-09d0-11eb-890f-46902ba9484b.png)

![image](https://user-images.githubusercontent.com/55044278/95488119-1ed42800-09d0-11eb-9b00-aabd8a0c2599.png)

<br>

**영어 사전 기능**

- 사용자가 입력한 단어의 뜻과 예문을 제공

- TTS 기술을 사용하여 단어의 발음까지 들려줌

- ```중요한 단어 / 어려운 단어``` 버튼을 통해 나만의 단어장에 추가 가능

![image](https://user-images.githubusercontent.com/55044278/95488158-2a275380-09d0-11eb-9d46-57c1379d2b82.png)

<br>

**기사 스크랩 화면**

- 사용자가 스크랩한 기사들을 모아 볼 수 있음

![image](https://user-images.githubusercontent.com/55044278/95488504-97d37f80-09d0-11eb-8c21-4202064ff0bf.png)

<br>

**나만의 단어장 화면**

- ```중요한 단어 / 어려운 단어``` 로 구분하여 단어장 제시

- 빈도 수, 최근 등록 날짜, 해당하는 기사 제목, 삭제 버튼이 포함

- 단어를 클릭하면 해당하는 단어의 한글 뜻 제시

![image](https://user-images.githubusercontent.com/55044278/95488279-4dea9980-09d0-11eb-9cfa-29ad3ff2e60d.png)

![image](https://user-images.githubusercontent.com/55044278/95488337-622e9680-09d0-11eb-98f3-b176a1e79085.png)

<br>

**단어 퀴즈 화면**

- ```퀴즈 시작하기``` 버튼을 통해 진행

- 한글 뜻 -> 영단어 스펠링을 맞히는 방식

- ```이전 문제 / 다음 문제``` 버튼을 통해 문제 이동 가능

  - 정답일 경우, "정답입니다!" 라는 팝업을 표시

  - 오답일 경우, "틀렸습니다! 답은 OOO입니다!" 라는 팝업을 표시

![image](https://user-images.githubusercontent.com/55044278/95488409-796d8400-09d0-11eb-88e6-8bc69f192e9b.png)

![image](https://user-images.githubusercontent.com/55044278/95488425-7d010b00-09d0-11eb-8f50-04cec48f4916.png)

![image](https://user-images.githubusercontent.com/55044278/95488437-80949200-09d0-11eb-9f40-c5d37ca520fa.png)

![image](https://user-images.githubusercontent.com/55044278/95488446-84c0af80-09d0-11eb-9d6d-047e7682261c.png)

----------

6. **프로젝트 정보**

#### Install meteor

* [미티어 설치](https://www.meteor.com/install)

#### npm install (최초 1회 실행)

```
meteor npm install
```

#### Run

```
meteor
```

* 실행 후 웹 브라우저에서 localhost:3000 접속  (```meteor run --port <port number>```로 포트번호 지정 가능)

* Sign up 또는 Login. admire@gmail.com으로 Sign Up하면 관리자 계정임

* localhost:3000/postingAuto에서
  [The Korea Herald](http://www.koreaherald.com/index.php) 기사의 링크를 Scraping한 후 Upload하여 기사 업로드 가능

----------

7. **관련 문서**

* [페이지 구성](/docs/client_structure.md)

* [DB 구조](/docs/DB_collection.md)

* [추가한 package](/docs/npm_install.md)

* [참조](/docs/reference.md)

----------

8. **프로젝트 구조**

* Client : 화면 구성 모음

* docs : 정리한 문서 모음

* public : 사진 파일 등 모음

* server : 백엔드 관련

* lib : html HEAD, 라이브러리, 함수 등..  
