# ✈️ JORANG 여행에 대한 모든 것

## <br>📃 프로젝트 개발 동기
개인적으로 해외 여행을 좋아하는데, 다른 사람들은 내가 가고 싶은 여행지에 대해 어떻게 생각하고 계획과 경비를 어떻게 짰는지 확인하기 위해 서비스를 개발하였습니다.<br><br>

## 📃 프로젝트 목표
내가 쓰는 것은 제대로 알고 쓰자<br><br>

## 📃 프로젝트 소개
나의 여행 계획, 일지, 실제 사용한 경비를 관리하고 사람들과 공유하여 다른 사람들의 여행기를 읽고 소통하면서 내 여행을 준비하는데 필요한 정보를 얻을 수 있다.<br><br>

## 📃 프로젝트 기간
2024/6/3 ~ 2024/7/1<br><br>
         
## 📃 핵심 기능
### 1. 여행기, 경비, 계획 작성 및 공유

- 날짜별 여행기, 경비 작성 및 공유
- Google cloud storage를 이용하여 사진 업로드 및 가져오기
- 이미지 슬라이더 구현
- 경비를 도표로 구현
- 여행 일지 최신순, 좋아요순 정렬 및 여행 기간에 따른 여행 일지 필터 구현
- 유저 아이디, 이메일 변경 시 이메일로 임시 비밀번호 발송<br><br>

### 2. 챗봇 (아래 Chatbot server 참고)

- Langchain을 이용하여 명소, 여행지, 여행 계획 추천 기능 및 내 맞춤 여행 계획 추천 구현
  (LLM : Google Gemini)<br><br>

### Main server (Java with Spring boot)
https://github.com/encore-full-stack-5/JORANG-TRAVEL-BE

### Chatbot server (Python with Fast API, Langchain)
https://github.com/encore-full-stack-5/JORANG_LANGCHAIN_SERVER

### Front end (React)
https://github.com/encore-full-stack-5/JORANG-TRAVEL-FE<br><br>


## 🧑🏻‍💻 구성원 및 역할 분담
 
 - 조진호 : 날짜별 여행기 작성, 사진 업로드 및 가져오기, 유저 인증(JWT), Web Security, 검색 기능, 전체 Debugging
 - 김세현 : 퍼블리싱, 유저 로그인, 회원가입, 이메일 발송, 나라 소개 기능 구현 
 - 임서연 : 날짜별 여행 경비 작성 기능 구현
 - 공통 : 챗봇 (명소, 여행지, 여행 계획 추천 및 내 맞춤 여행 계획 추천) 기능 구현<br><br>

## 📃 화면 구성 및 기능 소개 (Video)
### 1. 나라별 여행 일지 확인 ###

https://github.com/user-attachments/assets/a2ea9a2e-9f42-490c-aff8-9575c6e234fd

### <br> 2. 전체 여행 일지 확인 ###

https://github.com/user-attachments/assets/b5763e68-649d-4c56-b9f9-6a492f1f1b8f

### <br> 3. 여행 일지 작성 및 공유 ###

https://github.com/user-attachments/assets/a62dcd25-fe13-4b7b-92ee-a55645de2555

### <br> 4. 여행 일지 임시 저장 및 수정 ###

https://github.com/user-attachments/assets/bb1a542d-729c-4390-8eb5-7b50abc26043

### <br> 5. 여행 챗봇 ###

https://github.com/user-attachments/assets/5277301b-6221-4451-9c30-7a4ac4897c13

## <br> ⚙️ 기술스택

### Server language and framework
![Java](https://img.shields.io/badge/java-%23ED8B00?style=for-the-badge&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Spring-Boot](https://img.shields.io/badge/spring--boot-%236DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white)
![FASTAPI](https://img.shields.io/badge/FASTAPI-%23009688?style=for-the-badge&logo=fastapi&logoColor=white)

### Database
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">

### Image storage
![Google Cloud Storage](https://img.shields.io/badge/google%20cloud%20storage-%23AECBFA?style=for-the-badge&logo=googlecloudstorage&logoColor=black)

### LLM
![Google gemini](https://img.shields.io/badge/google%20gemini-%238E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)<br><br>

   
## 느낀 점
진호 : 전체적으로 프로젝트의 front에서 back을 A부터 Z까지 경험을 하여 크게 성장할 수 있는 프로젝트 였다. 이 과정에서 에러를 많이 마주치고 해결해나가면서 각종 에러 케이스에 대한 시야를 넓힐 수 있었다. 특히, join 관계에 따라 query를 어떻게 쳐야하는지에 대해 심도 있게 알게 되었다. 이를 통해 N+1 loading이 왜 발생하고 fetch join으로 해결하는 과정을 몸소 느낄 수 있었다. 또한, 팀장으로서 다른 사람들의 코드를 읽어야 하는 경우가 많았는데, 이를 통해 다른 사람의 코드를 이해하는 눈을 기르고 미처 알지 못하거나 간과했던 부분에 대해 깨달았다. 이러한 과정을 통해 내 코드 뿐만 아니라, 다른 사람의 코드를 읽는 것이 실력 향상에 굉장히 도움이 된다는 것을 느꼈다. 아쉬웠던 점은 elastic search setup 을 하는 과정에서 인증서 문제로 시간을 많이 잡혀 구현을 못한 것이다. 또한, 부모 entity를 삭제할 때 자식 entity를 자동으로 삭제하기 위해 cascade를 사용함으로써 양방향 맵핑을 사용하였다. 하지만, 이 부분 때문에 순환 참조가 생기고 이를 회피하기 위해 @JsonManagedReference, @JsonBackReference를 사용하였지만 결과적으로 부모 entity의 data 덩치가 너무 커졌다. 이를 통해 data 삭제는 isDeleted로 대체하고 순환 참조는 dto 를 사용하여 회피하는 것이 좋다는 것을 깨달았다. 또한, jpa named query로 모든 것을 해결하고자 하였지만, 3개 테이블의 join 및 LIMIT를 사용할 수 없는 JPQL의 한계를 겪었기 때문에 너무 ORM에 의지하지 않고 SQL문(native query)을 사용하여 필요한 데이터만 한 번에 가져올 수 있는 것의 필요성을 깨닫는 계기가 되었다. 마지막으로 debuggging을 하면서 생각보다 많은 문제를 깨닫고 이를 해결해나가면서 버튼의 구성 및 이에 따른 server api의 편의성이 중요하다는 것을 깨달았다.<br>
<br>세현 : 이번 JORANG 프로젝트를 진행하면서 여러 가지 어려움을 극복하고 많은 것을 배울 수 있었습니다. 처음에는 여러 에러들을 보고 오류를 수정하는 것이 힘들었지만, 반복되는 에러를 몇 번 경험하고 나서 직접 오류를 고칠 수 있게 되었습니다. 초기 ERD를 설계하고 수정하는 과정에서 Redis를 활용하지 못한 점이 아쉬웠으며, 다음 프로젝트에서는 꼭 사용해보고 싶다고 생각했습니다. 챗봇 페이지를 구현하면서 스프링부트와는 다른 파이썬 서버를 연결하는 것이 처음에는 복잡하게 느껴졌지만, 직접 서버를 연결해 보면서 생각보다 간단하다는 것을 깨달았습니다. 이를 통해 랭체인을 활용하는 법도 배웠으나, 시간 부족으로 인해 충분히 활용하지 못한 점이 아쉬움으로 남습니다. 또한 프론트엔드와 서버 간 Axios를 활용하여 데이터를 주고받는 방법을 학습했습니다. 이를 통해 데이터 통신의 기초를 이해하게 되었습니다. 처음에는 비동기 함수를 잘 알지 못해 사용하는 데 어려움이 있었지만, 프로젝트를 진행하면서 async와 await에 대해 공부하고 비동기 함수를 이해하게 되었습니다. 프론트엔드 화면을 처음부터 구성하는 것이 초반에는 헷갈렸지만, 처음부터 직접 화면을 구성해보면서 리액트의 전체적인 흐름과 구조 및 작동 방식을 더욱 자세하게 이해할 수 있었습니다. 또한 CSS를 사용할 때 팀원과 클래스 이름이 겹치는 문제가 발생했지만, 이후에 클래스 이름을 신중하게 관리하고 네이밍 규칙을 정하면서 충돌을 방지했습니다. 리액트에서 화면이 원하는 대로 렌더링되지 않는 문제도 겪었으나, 리액트의 렌더링 기준과 useEffect에 대해 자세히 공부한 후 리액트의 렌더링 메커니즘을 이해하게 되어 원하는 대로 화면을 구성할 수 있었습니다. 이번 프로젝트를 진행하면서 백엔드와 프론트엔드에서 다양한 기술적 어려움을 극복하고 많은 것을 배울 수 있는 시간이었습니다.<br>
<br>서연 : API를 통한 요청과 응답 과정을 직접 구현하면서 이를 통해 어떻게 서버가 클라이언트의 요구에 반응하여 필요한 데이터를 제공하는지 프로젝트의 전체적인 흐름을 알게되는 프로젝트였다
프론트 컴포넌트 구성에 있어서 컴포넌트를 명확히 분리하지 않음으로써 코드가 지나치게 길어지고
이로 인해 전체적인 코드의 가독성이 떨어지는 문제를 경험했다
이는 코드 내에서 정보를 찾기가 어려웠고, 유지보수의 효율을 저하시켰다
또한 CSS 클래스 이름이 겹치는 문제도 발생했다
앞으로는 컴포넌트 설계에서 주의를 기울여야겠다는 생각이 들었다.



