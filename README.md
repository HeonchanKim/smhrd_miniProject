# :pushpin: 시대별 유행어 맞추기 게임
>2000~2020년대 유행어 맞추기 게임
>

</br>

## 1. 제작 기간 & 참여 인원
- 2022년 1월 17일 ~ 1월 20일
- 팀 프로젝트(4명)

</br>

## 2. 사용 기술
#### `Back-end`
  - Java 8
  - Oracle Database


</br>

## 3. ERD 설계
<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/mini.png?raw=true">
</p>


## 4. 핵심 기능
이 서비스의 핵심 기능은 단어 맞추기 기능입니다.</br>
사용자는 로그인 후 목록 중 게임 하기를 선택하면 3가지 연도 목록 중 하나를 선택하고 게임을 진행합니다. </br>
문제가 출력되고 정답입력과 힌트 보기 두 가지 선택으로 나뉩니다.</br>

<details>
<summary><b>기능 설명</b></summary>
<div markdown="1">

### 4.1. 전체 흐름

<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%ED%9D%90%EB%A6%84%EB%8F%84.png?raw=true">
</p>

전체 흐름을 간단히 표시했습니다. 실행하면 먼저 1.회원가입 2.로그인 3.종료 3가지 선택을 할 수 있고 회원가입을 하면 다시 첫 화면으로 돌아옵니다. 로그인을 선택 시 로그인 성공과 실패로 나뉩니다. 로그인 실패 시 실패 문구와 함께 다시 첫 화면으로 돌아옵니다.

</br></br>    

<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%EA%B2%8C%EC%9E%84%EC%8B%9C%EC%9E%91.PNG?raw=true">
<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%ED%9E%8C%ED%8A%B8%EB%B0%8F%EC%A0%95%EB%8B%B5%EC%9E%85%EB%A0%A5.PNG?raw=true">
<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%EA%B2%8C%EC%9E%84%ED%9B%84%EA%B2%B0%EA%B3%BC.PNG?raw=true">
</p>

<b>로그인에 성공하면</b> 게임하기, 누적결과보기, 랭킹보기, 로그아웃 4가지 선택지가 있습니다. 게임하기를 누르면 또다시 2000년대 2010년대 2020년대 3가지 년도 선택이 주어지고 년도를 선택하면 문제와 함께 다시 정답입력, 힌트보기 선택이 주어집니다. <b>힌트보기는 두 번까지만</b> 볼 수 있고 이후에 힌트보기를 선택하면 "모든힌트를 다 보셨습니다!!"가 출력됩니다. 문제를 모두 풀고 난 후 맞춘 점수가 표시됩니다.
</br></br>

<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%EB%88%84%EC%A0%81%EA%B2%B0%EA%B3%BC.PNG?raw=true">
</p>

누적결과를 선택하면 로그인한 아이디의 누적된 점수 보여주며 점수별로 보이는 모습과 소리가 다릅니다.
</br></br>
</br></br>

<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%EB%9E%AD%ED%82%B9.PNG?raw=true">
</p>
랭킹 확인을 선택하면 상위점수 10명이 출력됩니다.
</br></br>

### 4.2. 회원가입
<p align="center">
    <img src="https://github.com/HeonchanKim/smhrd_miniProject/blob/master/images/%ED%9A%8C%EC%9B%90%EA%B0%80%EC%9E%85.png?raw=true">
</p>
:pushpin: [코드 확인](https://github.com/HeonchanKim/smhrd_miniProject/blob/master/miniProject/src/Model/UserInfoDAO.java#L49)
회원가입 기능 insertUser()메서드는 id, pw를 매개변수로 받아 USER_INFO 테이블에 삽입하면 boolean 타입을 반환해 사용자에게 가입성공, 실패를 보여줍니다.



### 4.3. 로그인
</div>
</details>


</br>

## 5. 핵심 트러블 슈팅
### 5.1. 컨텐츠 필터와 페이징 처리 문제
</br>

## 6. 그 외 트러블 슈팅
</br>

## 7. 회고 / 느낀점
>프로젝트 개발 회고 글: 
