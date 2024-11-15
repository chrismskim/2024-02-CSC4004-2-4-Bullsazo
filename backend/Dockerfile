# Python 기반 이미지
FROM python:3.10

# 작업 디렉토리 설정
WORKDIR /app

# 요구 사항 파일 복사 및 설치
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 프로젝트 파일 복사
COPY . .

# 실행 명령어
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]