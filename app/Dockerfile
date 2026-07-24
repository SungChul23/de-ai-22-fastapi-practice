# 1. 기본이미지
FROM python:3.14.0-slim

# 2. 작업디렉토리 지정 (/app)
WORKDIR /app

# 3. requirements.txt 복사
COPY requirements.txt .

# 4. requirements.txt 설치 명령 진행
RUN pip install -r requirements.txt

# 5. 원본소스 전체 복사 (main.py, templates/, static/ 등 다 포함)
COPY . .

# 6. 서버가동 => 도커 컴포즈로 이관, 여기서는 생략됨