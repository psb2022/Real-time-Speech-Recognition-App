
# 실시간 음성 인식 웹 애플리케이션 (Whisper + Flask + React)

## 프로젝트 개요

이 프로젝트는 **브라우저에서 음성을 녹음하고**, **Flask 서버로 전송하여**, **Whisper AI 모델을 통해 실시간으로 텍스트로 변환**하는 웹 기반 음성 인식 서비스입니다.
- **프로젝트명:** Google Colab + Whisper 모델 기반의 STT(음성 → 텍스트) 실시간 웹 앱
- **주요 목표:** 브라우저에서 실시간으로 음성을 텍스트로 변환하여 화면에 출력
- **사용 환경:** Google Colab (Python 기반), 모바일 웹 접속 가능

---

## 주요 기능

- 실시간 음성 인식
- 웹 기반 인터페이스 제공
- WebSocket 기반의 양방향 통신
- 녹음 시작/중지 제어 기능
- 인식 결과 시각화 기능

---

## 기술 스택

| 영역        | 기술                                   |
|-------------|----------------------------------------|
| Frontend    | React, Material-UI, WebSocket          |
| Backend     | Flask, flask-sock, whisper, pyngrok    |
| 모델        | OpenAI Whisper (base)                  |
| 개발 환경   | Google Colab (Jupyter Notebook 기반)   |
| 배포 접근   | ngrok (https 기반 터널링)              |

---

## 시스템 아키텍처

```plaintext
[Browser (React)] ⇄ WebSocket ⇄ [Flask 서버 (Colab)] → Whisper 모델
            │                            ↑
     사용자 음성 녹음             ngrok로 외부에 공개
```

---

## 해결한 주요 이슈

| 문제 | 해결 방법 |
|------|------------|
| ngrok 주소 매번 수정 | `window.location`으로 자동 설정 |
| Colab 서버 외부 접근 불가 | pyngrok 사용해 HTTPS 터널 생성 |

---

## 학습한 기술 및 인사이트

- WebSocket 기반 실시간 처리 구조
- Whisper 모델 활용 및 입력 전처리
- 클라우드 기반 서버 공개 방식
- 클라이언트–서버 통합 구조 설계 및 구현

---

## 향후 개선 사항

- 실시간 스트리밍 처리 방식으로 개선
- Whisper 모델 업그레이드
- WebSocket 재접속 로직 구현
- 지속 가능한 배포 환경 이전
- UI/UX 개선
- 모바일 최적화 및 반응형 디자인

---

## 포트폴리오 링크

[[GitHub Repository Link](https://github.com/your-username/yolov8-object-detection-webapp)](https://github.com/psb2022/Real-time-Speech-Recognition-App)

---
