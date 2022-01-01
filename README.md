
<!-- ![draw](https://user-images.githubusercontent.com/50126248/135090772-9f1a1d38-e6dc-4d0f-8512-36b22c790f56.png) -->
 
# 백엔드 개발자 백승호입니다

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fweirdbb91%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) ![Hits](https://img.shields.io/github/followers/weirdbb91?label=Follow)


![weirdbb91's GitHub stats](https://github-readme-stats.vercel.app/api?username=weirdbb91&count_private=true)
<br><br>


# 🏢 Wemember(2021.11 ~ 2021.12)  

## 여행 경험 공유 플랫폼 - 백엔드 개발
![Python](https://img.shields.io/badge/Python-3776ab?style=plastic&logo=Python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009485?style=plastic&logo=FastAPI&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=plastic&logo=PostgreSQL&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-007bff?style=plastic&logo=Docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-orange?style=plastic&logo=Amazon-AWS&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=plastic&logo=Swagger&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=plastic&logo=Git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=plastic&logo=Figma&logoColor=white)
![Jandi](https://img.shields.io/badge/Jandi-85EA2D?style=plastic&logo=Jandi&logoColor=white)

11월부터 입사해 현재까지 제가 작업한 부분은 아래와 같습니다
- 목록 반환시 페이징 처리 후 메타 데이터와 함께 반환
  - PageMeta(total, size, page, has_next)
- 토큰 생성/검증
  - 헤더로 반환, 브라우저 헤더 접근 허용 설정(expose headers)
  - 엑세스/리프레시, 각각 다른 시크릿 키, 만료시간
  - 토큰 리프레시
  - 토큰 입력을 옵셔널로 처리해 로그인/비로그인 사용자 요청처리
  - 각 상황에 맞는 예외처리(토큰이 필수인 요청에서의 토큰 미입력, 시그니처 불일치, 기간 만료, 권한 부족)
- 익셉션 핸들러(미들웨어)
  - 발생한 각 예외들에 따라 클라이언트로 반환되는 에러코드, 메시지 등을 한곳에서 통합 관리
- 카카오 알림톡(API STORE)
- AWS S3 이미지 업로드/삭제 - boto3
- docker-compose(로컬에서 서버, DB 이미지빌드/배포/연결/초기화/더미데이터/테스트)
- TestClient로 테스트 코드 작성
- API 작성/수정
- API 명세 작성



# 🏢 Gogiro110(2021.04 ~ 2021.10)  

## 대면 거래 불참 방지 안전거래 솔루션 - 백엔드 개발
![Python](https://img.shields.io/badge/Python-3776ab?style=plastic&logo=Python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009485?style=plastic&logo=FastAPI&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=plastic&logo=PostgreSQL&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-007bff?style=plastic&logo=Docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-orange?style=plastic&logo=Amazon-AWS&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=plastic&logo=Swagger&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=plastic&logo=Git&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=plastic&logo=Slack&logoColor=white)
![Jira-Software](https://img.shields.io/badge/Jira-0052CC?style=plastic&logo=Jira-Software&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=plastic&logo=Notion&logoColor=white)
![Zeplin](https://img.shields.io/badge/Zeplin-orange?style=plastic&logo=Zeplin&logoColor=white)

4월부터 입사해 백엔드 개발을 시작했습니다  

Python - FastAPI를 사용해 서버를 구성했고, 제가 개발한 내용은 아래와 같습니다  

![Diagram]  

AWS Route 53로 도메인을 등록했고  
AWS Certificate Manager에서 ssl 인증서를 발급받아 적용했습니다  
접근이 잦고 빠른 로딩이 필요한 리소스들은 CloudFront 서비스를 이용해 관리했습니다  

서버 업데이트시에도 서비스를 중단할 수 없어 롤링 업데이트 방식을 채택하기 위해  
AWS Elastic Beanstalk으로 서버를 배포했습니다  

DEV, TEST, PRODUCT와 로컬까지 4가지 서버 모두 다른 시크릿 키를 사용해야해서  
빈스톡 환경속성 설정을 이용해 각 서버별로 다른 환경변수 파일을 구분해 로드했습니다  

서비스에 필요한 회원, 기기, 상품, 주소, 만남, 거래, 후기, 포인트, 가상계좌, 트랜잭션 등의  
모델들을 설계하고 요구되는 비지니스 로직대로 API를 작성했습니다

테스트 환경은 도커로 구성했고, 테스트 코드는 FastAPI TestClient로 작성했습니다  

<br><br>
---

# 📋 개인 토이 프로젝트(2021.02 ~ 2021.03)

## 자바 스프링기반 소셜로그인 게시판
![Java](https://img.shields.io/badge/Java-007396?style=plastic&logo=Java&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=plastic&logo=Spring&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=plastic&logo=MySQL&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=plastic&logo=Thymeleaf&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-orange?style=plastic&logo=Amazon-AWS&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=plastic&logo=Git&logoColor=white)
[자세히/코드 보기](https://github.com/weirdbb91/lamb)

- 스프링, 스프링 시큐리티의 설정들과 전반적인 흐름 학습이 목적
- OAuth 2.0 기술을 통한 소셜 로그인 구현 (naver, kakao, google, github, facebook)
- 사용자 토큰을 저장해 로그인 횟수 감소 (remember me)
- AWS EC2와 RDS(MySQL) 사용
- batch, shell script를 활용해 빌드, 배포 자동화
- ssl 인증서 적용
- Thymeleaf를 이용해 간단한 프론트엔드 구현

---
<br><br>

## 🚀 Available
![Java](https://img.shields.io/badge/Java-007396?style=plastic&logo=Java&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=plastic&logo=Spring&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=plastic&logo=Thymeleaf&logoColor=white)  
![Python](https://img.shields.io/badge/Python-3776ab?style=plastic&logo=Python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009485?style=plastic&logo=FastAPI&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=plastic&logo=Swagger&logoColor=white)  
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=plastic&logo=MySQL&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=plastic&logo=PostgreSQL&logoColor=white)  
![Docker](https://img.shields.io/badge/Docker-007bff?style=plastic&logo=Docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-orange?style=plastic&logo=Amazon-AWS&logoColor=white)  
![Git](https://img.shields.io/badge/Git-F05032?style=plastic&logo=Git&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=plastic&logo=Slack&logoColor=white)
![Jira-Software](https://img.shields.io/badge/Jira-0052CC?style=plastic&logo=Jira-Software&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=plastic&logo=Notion&logoColor=white)
![Zeplin](https://img.shields.io/badge/Zeplin-orange?style=plastic&logo=Zeplin&logoColor=white)

---

### :mailbox_with_mail: Contacts
[![Gmail Badge](https://img.shields.io/badge/Gmail-d14836?style=flat-square&logo=Gmail&logoColor=white&link=mailto:weirdbb91@gmail.com)](mailto:weirdbb91@gmail.com)
[![Blog Badge](http://img.shields.io/badge/-Blog-black?style=flat-square&logo=github&link=https://weirdbb91.github.io)](https://weirdbb91.github.io)



[diagram]: <https://user-images.githubusercontent.com/50126248/135085032-8d7fb24b-e1ae-47ad-8a85-e018309a5d8d.png>


<!-- 
[docker]: <https://user-images.githubusercontent.com/50126248/111152182-cf73d280-85d3-11eb-9555-8016c1804a07.png>
[git]: <https://user-images.githubusercontent.com/50126248/111152187-d00c6900-85d3-11eb-8a55-37f2142a933e.png>
[html]: <https://user-images.githubusercontent.com/50126248/111152191-d0a4ff80-85d3-11eb-90db-7fc0e702e5e7.png>
[java]: <https://user-images.githubusercontent.com/50126248/111152193-d13d9600-85d3-11eb-86d6-f3c5c7e7dca7.png>
[javascript]: <https://user-images.githubusercontent.com/50126248/111152197-d13d9600-85d3-11eb-9a00-6160444a3f37.png>
[jenkings]: <https://user-images.githubusercontent.com/50126248/111152198-d1d62c80-85d3-11eb-9bc1-94487809f199.png>
[thymeleaf]: <https://user-images.githubusercontent.com/50126248/111281545-66966400-8680-11eb-8b65-fa44b27e0fb7.png>
[jenkings]: <https://user-images.githubusercontent.com/50126248/111281547-672efa80-8680-11eb-823a-9379f0860adf.png>
[jquery]: <https://user-images.githubusercontent.com/50126248/111152203-d3075980-85d3-11eb-99ee-d1d6e30df2a0.png>
[linux]: <https://user-images.githubusercontent.com/50126248/111152206-d3075980-85d3-11eb-8b16-872f9f5fab4d.png>
[mysql]: <https://user-images.githubusercontent.com/50126248/111152209-d39ff000-85d3-11eb-938d-4090d4d27e27.png>
[python]: <https://user-images.githubusercontent.com/50126248/111152212-d4388680-85d3-11eb-9c3a-4b354b34ec28.png>
[ubuntu]: <https://user-images.githubusercontent.com/50126248/111152215-d4d11d00-85d3-11eb-8d97-575d5ef3c792.png>
[vuejs]: <https://user-images.githubusercontent.com/50126248/111152216-d4d11d00-85d3-11eb-8faa-71349d68a622.png>
[spring]: <https://user-images.githubusercontent.com/50126248/111152217-d569b380-85d3-11eb-9b3c-35f070915d20.png>
[aws]: <https://user-images.githubusercontent.com/50126248/111152218-d569b380-85d3-11eb-9df2-85f9d67d305f.png>
[bootstrap]: <https://user-images.githubusercontent.com/50126248/111152219-d6024a00-85d3-11eb-8087-299af4494ee9.png>
[css]: <https://user-images.githubusercontent.com/50126248/111152220-d6024a00-85d3-11eb-824d-a720aa139cd0.png>
[atlas]: <https://user-images.githubusercontent.com/50126248/111276356-99d5f480-867a-11eb-925d-6bea38908eaa.png>
[jiraSW]: <https://user-images.githubusercontent.com/50126248/111279187-c9d2c700-867d-11eb-9876-8ac77b756dda.png>
[jira]: <https://user-images.githubusercontent.com/50126248/111279189-ca6b5d80-867d-11eb-9ad4-ba7d0313f726.png>
[bitbucket]: <https://user-images.githubusercontent.com/50126248/111279191-cb03f400-867d-11eb-82d1-52a499dde9d2.png>
[confluence]: <https://user-images.githubusercontent.com/50126248/111279184-c93a3080-867d-11eb-9f89-e8013461f545.png> -->
