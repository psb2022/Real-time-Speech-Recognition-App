
# 🎙️ 실시간 음성 인식 웹 애플리케이션 (Whisper + Flask + React)

Google Colab + Whisper 모델 기반의 STT(음성 → 텍스트) 실시간 웹 앱

---

## 🚀 프로젝트 개요

이 프로젝트는 **브라우저에서 음성을 녹음하고**, **Flask 서버로 전송하여**, **Whisper AI 모델을 통해 실시간으로 텍스트로 변환**하는 웹 기반 음성 인식 서비스입니다.

- 실시간 WebSocket 통신
- OpenAI Whisper 모델 활용
- Google Colab + ngrok을 통한 서버 실행
- React 기반 프론트엔드

---

## 🧠 주요 기능

- ✅ 실시간 음성 → 텍스트 변환
- ✅ WebSocket을 통한 양방향 통신
- ✅ Whisper 모델을 Colab 환경에서 직접 구동
- ✅ ngrok을 통한 외부 공개 및 접근
- ✅ 자동 WebSocket URL 감지 (브라우저 주소 기반)

---

## 🏗️ 기술 스택

| 영역        | 기술                                   |
|-------------|----------------------------------------|
| Frontend    | React, Material-UI, WebSocket          |
| Backend     | Flask, flask-sock, whisper, pyngrok    |
| 모델        | OpenAI Whisper (base)                  |
| 개발 환경   | Google Colab (Jupyter Notebook 기반)   |
| 배포 접근   | ngrok (https 기반 터널링)              |

| 프론트엔드 | React, Material-UI, WebSocket |
| 백엔드 | Flask, flask-sock, whisper, pyngrok |
| AI 모델 | OpenAI Whisper (base) |
| 실행환경 | Google Colab + Python |
| 배포 접근 | ngrok (https 기반 터널링) |

---

## 📐 시스템 아키텍처

```plaintext
[Browser (React)] ⇄ WebSocket ⇄ [Flask 서버 (Colab)] → Whisper 모델
            │                            ↑
     사용자 음성 녹음             ngrok로 외부에 공개
```

---

## 📹 사용 방법

1. 브라우저 접속 → "Start Recording" 클릭  
2. 음성 입력 후 "Stop Recording"  
3. Whisper 모델이 음성을 텍스트로 변환  
4. 변환된 텍스트가 화면에 실시간 표시

---

## 🧩 해결한 주요 이슈

| 문제 | 해결 방법 |
|------|------------|
| ngrok 주소 매번 수정 | `window.location`으로 자동 설정 |
| 오디오 인식 오류 | Blob → .wav 저장 후 Whisper에 전달 |
| Colab 서버 외부 접근 불가 | pyngrok 사용해 HTTPS 터널 생성 |

---

## 🧠 학습한 기술 및 인사이트

- WebSocket 기반 실시간 처리 구조
- Whisper 모델 활용 및 입력 전처리
- 클라우드 기반 서버 공개 방식
- 클라이언트–서버 통합 구조 설계 및 구현
- 예외 상황 처리와 실전 문제 해결 경험

---

## 🔧 향후 개선 사항

- Whisper medium/large 모델로 정확도 향상
- WebSocket 자동 재접속 기능 추가
- 실시간 스트리밍 방식으로 구조 개선
- 모바일 반응형 UI 개선

---

```

---

## 🙋‍♂️ Contact

- GitHub: [your-username](https://github.com/your-username)
- Email: your.email@example.com
