# portfolio

강릉원주대학교 컴퓨터공학부 2학년 재학 중인 박석규입니다.  
컴퓨터공학 분야에 대해 높은 관심과 열정을 가지고 공부하고 있으며, 지금은 기초적인 프로그래밍 지식과 데이터 구조등을 학습하는중입니다.  
앞으로는 보다 깊이 있는 프로그래밍 지식을 습득하고, 실제 업무에서 사용되는 기술들을 익히며 성장해 나가려고 노력하고 있습니다.  
공부하는 동안 열심히 노력하고 성과를 내기 위해 노력하고 있으며, 향후 목표는 컴퓨터 공학 분야에서의 전문성을 쌓아 대학을 무사히 졸업하고 현업에서 좋은 성과를 내는 것입니다.  
감사합니다.

# Community_Project
첫 프로젝트로 간단한 커뮤니티 어플리케이션 프로젝트입니다.  
코틀린과 파이어 베이스를 활용했습니다.

## 개발도구 및 환경
+ 개발 도구: Android Studio
+ 프로그래밍 언어: 코틀린
+ 프레임워크: Firebase
+ 버전 관리 도구: GitHub

## 프로젝트 목적 및 배경
+ 대학교 1학년을 마친 2022년 겨울 방학, 2학년 준비를 위해 자바를 공부했지만 심화학습과 프로젝트를 위해선 자습으론 부족하다고 느껴 
코틀린으로 전향하여 간단한 어플리케이션 프로젝트를 시작했다.

+ 이 어플리케이션은 한국의 각종 커뮤니티 어플(Ex 에브리타임 등...)을 보고 클론코딩에 가깝게 커뮤니티 화면을 구현하였다.

## 프로젝트의 핵심 기능 소개
+ 이 어플리케이션의 핵심 기능은 파이어베이스의 클라우드 파이어스토어를 사용하여 데이터를 실시간으로 읽고 쓸 수 있다는 점이다.  
기존의 나와있는 코틀린 책에서는 리얼타임 데이터베이스를 사용하여 커뮤니티 어플리케이션을 구현하는 것이 대부분이지만,
이 어플리케이션은 *리얼타임 데이터베이스*의 상위호환격인 *클라우드 파이어스토어*를 이용하여 좀 더 유연한 쿼리를 사용할 수 있어 **관리**(글의 정렬 등...)가 편리해졌다.  

## 프로젝트 결과
### 회원가입
어플리케이션을 사용 하기 위해서 회원가입이 필요하다.  
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221890752-c1736045-3f49-4b8a-9135-acdd213b590e.gif"/>  
↑↑↑또한 파이어베이스를 이용해 이메일 인증을 받은 계정만이 메인화면으로 이동할 수 있도록 하였다.  
<img width="40%" src="https://user-images.githubusercontent.com/70646278/221889655-bb191c12-01d3-42c4-9b62-07c31c3e5a52.png"/>  
실제 네이버 계정으로 이메일이 온 화면.  
<img width="40%" src="https://user-images.githubusercontent.com/70646278/221890454-dba513f5-e0d8-426f-873b-66b4cd211a5b.png"/>  
  
  
### 로그인
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221891852-4244e4ad-4db6-41ed-9bc8-d42315bc24db.gif"/>  
로그인 완료후 다른 사용자의 글을 볼수 있다.  

### 글쓰기
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221892489-477fa25d-a477-4bf7-b61d-e5012a225f8f.gif"/>  
이미지를 첨부하고 글 쓰기를 완료하는 모습.  
  
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221892779-e04af262-35bf-4d01-9912-f0f6e95aae29.gif"/>  
자신이 쓴 글을 확인후(조회수도 올라간다) 추천과 삭제를 할 수 있다.  

### 다른 유저의 글을 삭제하려고 한다면?
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221893074-85d7b1c8-3ae5-4fda-92dd-a1fdba08e6c7.gif"/>  
사용자의 UID가 데이터베이스에 저장된 해당 글의 UID와 맞지않아 삭제가 되지 않는다.  

### 댓글
<img width="25%" src="https://user-images.githubusercontent.com/70646278/221899494-145b6410-d5a4-448f-82b8-40c882b4344b.gif"/>  

## 프로젝트 평가 및 개선 방향

### 장점
+ 가장 큰 장점은 디자인이 전체적으로 클론 코딩에 가깝지만 이미 시장에서 검증된 UI이기도 하여서 사용자가 불편한 위치에 무엇이 있는 경우가 적다.
+ 두번째 장점은 클라우드 파이어스토어를 사용하여서 다양한 쿼리를 사용할 수 있기에 리얼타임 데이터베이스 대비 정렬을 위해 난잡한 코드가 나오지않으며 유지보수가 굉장히 좋다.

### 단점
+ 이미지를 원본 그대로 스토리지에 저장하는 방식이기에 매우 큰 용량을 어플리케이션이 스스로 압축하지 못하고 나중에 그대로 사용자에게 보여준다. 그래서 대량의 트래픽이 발생하게된다.
+ 아직 완성도가 높지 못하게 겉만 구현된 경우가 많다. (글 쓰기 중에 비디오나, 글씨크기등)

### 개선방향
+ 스토리지에 업로드 할 수 있는 최대 크기를 지정한다.
+ 긴 시간을 들여 추가적인 업데이트를 지속하는 방법으로 완성도를 높여가야 한다고 생각한다.

## 결론
+ 이 프로젝트는 코틀린을 배운 내가 커뮤니티 어플리케이션을 어디만큼 구현해낼수 있는지를 알아 볼 수있던 프로젝트였다.  
이 프로젝트를 진행하며 코틀린과 데이터베이스 관리 능력이 향상되는것이 스스로 느껴졌다.  
특히 처음에 어플리케이션을 만들때 데이터베이스로 리얼타임 베이스를 선택했었는데 복잡한 쿼리를 담당해내야하는 게시판의 특성상
데이터베이스를 바꿀 필요가 있었고 내 스스로의 힘으로 데이터베이스를 클라우드 파이어스토어로 바꿔냈을때 크게 느꼈던것 같다.

+ 나는 이 다음 프로젝트에 내에 댓글 기능을 넣을듯 한데, 이 프로젝트의 경험을 통해 다음 프로젝트에서는 댓글기능을 구현할때 적은 시간소모와 높은 완성도를 기대할 수 있을듯 하다.
