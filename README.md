<div align="center">
  
  # 기업 과제 04 - (주) 아이디어콘서트
  
</div>
<br><br>

## 목차
- [개발 기간](#--개발-기간--)  
- [프로젝트 설명 및 분석](#-프로젝트)
- [기술 스택](#기술-스택) 
<br><br>

<h2> ⌛ 개발 기간  </h2> 
 2022/07/18  ~ 2022/07/19
 <br><br>
  </div> 


# 💻 프로젝트
  ### 프로젝트 설명
  - Amazon EC2를 이용하여, Free-Tier 서버를 생성. 
      - Django 프로젝트 생성
      - Web Application Server : NGINX 사용 (80번 포트 오픈)
      - Elastic IP를 통한 IP
      - {IP}/api/hello 로 접속하였을때 웹브라우져 상에서 Hello 표시
<br>


  ### 프로젝트 분석

  - EC2에 Django + Nginx + gunicorn을 Dockerize하여 배포
      - Docker-Compose를 사용하여 Django와 Nginx 묶어 주기     
  - EC2 인스턴스에 Elastic IP 연결
  - Nginx 사용을 위한 환경설정 Dockerfile 작성
<br>


  ### 🔥 배포

- Docker를 이용해 프로젝트를 컨테이너화하여 AWS EC2에 배포했습니다.<br>
- AWS EC2에 배포, 테스트 및 동작을 확인하였으며, 비용 등의 이유로 접속이 불가할 수 있습니다.
<br><br>

[AWS EC2]
<br><br>
<img src="https://user-images.githubusercontent.com/44389424/179668506-5d37314c-6a83-44b4-b4e5-0f0830fb2a59.JPG"/>

<br><br>
[도커 컨테이너 리스트]
<br><br>
<img src="https://user-images.githubusercontent.com/44389424/179665670-d862d329-de6e-4fd7-95cf-e3fea2a398f8.JPG"/>
<br><br>



  ### 🚥 개발 조건 

  #### 🙆‍♂️ 필수사항  
    - Python, Django
    - AWS EC2, Elastic IP
    - NGINX
  #### 🔥 선택사항
    - Docker

## 📌 실행 방법

```
# 로컬에서 바로 서버 구동
pip install -r requirements.txt
python manage.py runserver

# 도커 실행 (prod branch)
pip install docker
pip install docker-compose
docker-compose up -d
```


## 기술 스택

> - Back-End :  <img src="https://img.shields.io/badge/Python 3.10-3776AB?style=flat&logo=Python&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/Django 4.0.4-092E20?style=flat&logo=Django&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/Django-DRF 3.13.1-009287?style=flat&logo=Django&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/Docker 20.10.14-2496ED?style=flat&logo=docker&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/Nginx-009639?style=flat&logo=Nginx&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
>
> - ETC　　　:  <img src="https://img.shields.io/badge/Git-F05032?style=flat-badge&logo=Git&logoColor=white"/>&nbsp;<img src="https://img.shields.io/badge/Github-181717?style=flat-badge&logo=Github&logoColor=white"/>&nbsp;
