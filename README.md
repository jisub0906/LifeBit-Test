# LifeBit Project

## 시작하기

### 1. Docker 환경 설정(데이터베이스)
```bash
docker-compose up -d
```

### 2. AI API (FastAPI) 설정
```bash
# AI API 디렉토리로 이동
cd apps/ai-api-fastapi

# Python 가상환경 생성 및 활성화
python -m venv venv

# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# 의존성 설치
pip install -r requirements.txt

# FastAPI 서버 실행
uvicorn main:app --reload --port 8001
```

### 3. Core API (Spring Boot) 설정
```bash
# Core API 디렉토리로 이동
cd apps/core-api-spring

# Spring Boot 서버 실행
./mvnw spring-boot:run
```

### 4. Frontend (Vite) 설정
```bash
# Frontend 디렉토리로 이동
cd apps/frontend-vite

# 개발 서버 실행
pnpm dev
```

## 서비스 포트
- Frontend: http://localhost:5173
- Core API: http://localhost:8080
- AI API: http://localhost:8001