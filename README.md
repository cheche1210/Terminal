# Terminal
장고를 위한 터미널 명령어 모음
🌱터미널 열기
ctrl + shift + `

🌱새 프로젝트 생성
django-admin startproject 프로젝트명

🌱프로젝트에 App 추가
python manage.py startapp appname

🌱서버 켜기
python manage.py runserver

🌱migrations 만들기
python manage.py makemigrations

🌱DB migrate 하기
python manage.py migrate

🌱관리자(admin) 계정 만들기
python manage.py migrate

🌱Static 파일 collecting하기
python manage.py createsuperuser

🌱python -m venv 가상환경명
python -m venv myvenv

🌱가상환경 실행/켜기
source myvenv/bin/activate

🌱가상환경 끄기
deactivate

🌱django 설치하기
pip install django

🌱django 프로젝트 시작
django-admin startproject 파일명

🌱django 서버 실행/켜기
python manage.py runserver

🌱django 서버 끄기
ctrl + c

🌱app 만들기(manage.py 있는 폴더에 만들기)
python manage.py startapp 파일명

🌱페이지 만들기 순서
1. settings.py => project에게 app의 존재 알리기
2. templates => views.py에서 처리된 데이터를 받아 사용자에게 화면을 보여줌
3. views.py => 데이터를 처리하는 함수 작성
4. urls.py => 요청에 맞는 함수를 views.py 에서 찾아 요청 전달

settings.py =>templates => views.py => urls.py


🌱MTV 패턴
- 데이터 저장 형태를 어떻게 할지 설정하겠다. -> Model
- 유저에게 보여지는 화면을 고치고 싶다 -> Template
- 데이터를 처리해서 가공하고 싶다. -> View
- 가공한 데이터를 유저가 보는 화면으로 넘겨주고 싶다 -> URLconf


==========[Django]BASIC 2==========
🌱새 프로젝트 생성
django-admin startproject firstprojext

🌱app 만들기
python manage.py startalp wordcount


🌱template 만들기
INSTALLED_APPS에 wordcount.apps.WordcountConig

🌱View 만들기
render(request, ‘wordcount/home.html’)
//home.html이라는 template이 위치하는 경로. 앞서 템플릿을 templates/wordcount/home.html 경로에 만들었기 때문


#가상환경 설정(source myvenv/bin/activate가 먹히지 않을때)

🌱pyenv virtualenv 3.7.0 pagenation//가상환경설정

🌱pyenv local pagenation .//적용
