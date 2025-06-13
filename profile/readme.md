## 🫧 Bubblog - Personalized Blog AI Chatbot

Bubblog은 사용자의 블로그 콘텐츠를 기반으로, 맞춤형 AI 챗봇을 생성해 방문자와 소통할 수 있게 해주는 플랫폼입니다. 단순한 블로그를 넘어, 나만의 디지털 페르소나를 구축할 수 있는 새로운 웹 경험을 제공합니다.

⸻

### 📌 프로젝트 개요
	•	주제: 개인 블로그 콘텐츠 기반 AI 챗봇 시스템
	•	목표: 블로그 글을 벡터 기반 검색증강 RAG(Retrieval-Augmented Generation)를 활용해 구축한 챗봇을 제공해, 방문자와 지능적인 대화가 가능하도록 구현
	•	활용: 카테고리, 태그 기반 필터링 / SSE 기반 실시간 응답 / 사용자별 챗봇 비교 분석 등

⸻

👥 팀 소개

이름	역할	주요 업무


⸻

🧱 시스템 구조

User ──> Frontend (Next.js)
               │
               ▼
      Backend (Spring Boot) ──> DB (PostgreSQL + pgvector)
               │
               ▼
          AI Server (FastAPI) ──> DB (PostgreSQL + pgvector)  Embedding Model + OpenAI API

	•	인증 및 블로그 관리: Spring Boot
	•	AI 챗봇 응답 처리: FastAPI + RAG 구조
	•	DB: PostgreSQL, pgvector

⸻

🛠 기술 스택

영역	스택
프론트엔드	Next.js, TypeScript, Tailwind CSS
백엔드	Spring Boot, JPA, PostgreSQL, Redis
AI 서버	FastAPI, OpenAI API, pgvector, Faiss
인증	JWT, OAuth2 (구글 로그인)
배포 및 운영	Docker, Nginx, EC2, GitHub Actions CI/CD
