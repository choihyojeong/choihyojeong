### Hi there 👋

## Introduction
안녕하세요.


## Link
E-mail: chj030405@yu.ac.kr

<!--
**choihyojeong/choihyojeong** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->



# Sonnuri_Server

# Sign Language Learning API (FastAPI)

이 프로젝트는 수어 학습 웹 애플리케이션의 백엔드 API입니다.  
FastAPI 기반으로 구축되었으며, 수어 단어 조회, 영상 제공, 업로드, 번역 및 정확도 측정 기능을 포함합니다.

---

## 📁 프로젝트 구조

sign_app/
├── api.py # FastAPI 라우터 정의
├── main.py # 애플리케이션 실행 엔트리포인트
├── static/ # 정적 파일 디렉터리 (영상, 사전 등)
│ └── data/
│ └── sign_dictionary.json
│ └── videos/
├── uploads/ # 업로드된 사용자 영상 저장 디렉터리
└── requirements.txt # 의존성 목록

yaml
복사
편집

---

## 🚀 주요 기능

| 엔드포인트 | 메서드 | 설명 |
|------------|--------|------|
| `/` | GET | 기본 확인용 |
| `/learn/{lang}/{text}` | GET | 특정 언어의 수어 영상 제공 |
| `/upload` | POST | 사용자 영상 업로드 |
| `/translate` | POST | 수어 ↔ 텍스트 변환 (샘플 반환) |
| `/accuracy` | POST | 업로드된 영상과 목표 단어 비교 정확도 평가 (미구현) |
| `/words` | GET | 수어 단어 목록 조회 |
| `/words/{word_id}` | GET | 단어 상세 정보 조회 |

---

## 🛠️ 로컬 개발 환경

### 1. 필수 패키지 설치
```bash
pip install fastapi uvicorn
2. 서버 실행 (main.py)
bash
복사
편집
python main.py
3. 접속 확인
브라우저에서 http://localhost:8000/docs 접속

📎 주의사항
pyngrok 설치 및 사용은 필요하지 않습니다.

본 API는 로컬 테스트 전용으로 설계되어 있습니다.

static/videos/, uploads/ 디렉터리는 수동으로 생성 후 사용하세요.

정확도 비교 기능(accuracy)은 추후 AI 모델 연동 필요.

👨‍💻 개발자 정보
이름: Hyoje

이메일: hyoje@example.com (원하는 경우만 기재)

깃허브: github.com/hyoje



이런 내용으로 README.md 꾸며줘
