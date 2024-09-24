# AI 디지털 도슨트: 미래 교육의 혁신적 안내자

<p align="center">
  <img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white" alt="Unity">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/AWS_Polly-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="AWS Polly">
  <img src="https://img.shields.io/badge/LangChain-121D33?style=for-the-badge&logo=chainlink&logoColor=white" alt="LangChain">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/eecc04ac-079d-439b-a841-6e2f1af1b109" alt="AI Digital Docent Concept" width="600">
</p>

## 📚 목차
1. [프로젝트 개요](#-프로젝트-개요)
2. [주요 기능](#-주요-기능)
3. [기술 스택](#-기술-스택)
4. [시스템 아키텍처](#-시스템-아키텍처)
5. [개발 기간](#-개발-기간)
6. [개발자 정보](#-개발자-정보)

## 🎨 프로젝트 개요

AI 디지털 도슨트는 최첨단 AI 기술을 활용하여 방문객들에게 개인화된 안내 서비스를 제공하는 혁신적인 시스템입니다. 이 프로젝트는 자연어 처리, 음성 인식 및 합성 기술을 결합하여 방문객들과 자연스러운 대화를 나누며, 센터의 다양한 전시물과 주제에 대해 심도 있는 설명을 제공합니다.

### 💡 개발 배경
전통적인 안내 서비스의 한계를 극복하고, 4차 산업혁명 시대에 걸맞은 미래지향적 학습 경험을 제공하고자 본 프로젝트를 기획하였습니다. AI 기술의 발전을 교육 분야에 적용함으로써, 방문객들에게 더욱 풍부하고 인터랙티브한 학습 기회를 제공하는 것이 목표입니다.

## 🚀 주요 기능

1. **음성 기반 상호작용**
   - 웨이크워드 감지 시스템으로 간편한 대화 시작
   - AWS Polly를 이용한 자연스러운 음성 합성(TTS)
   - Web Speech API를 활용한 실시간 음성 인식(STT)

2. **지능형 대화 시스템**
   - LLama3 모델 기반의 고급 자연어 처리
   - 맥락을 고려한 지능적 응답 생성
   - 개인화된 정보 제공 및 질문 응답
![image](https://github.com/user-attachments/assets/539b0dce-e778-420c-8500-7eb0c0f91a88)
(html 파일은 텍스트를 시각화 하기위해 넣어놨습니다)

3. **실시간 시각적 피드백**
   - Unity 기반 동적 이퀄라이저로 음성 출력 시각화
   - 사용자 친화적 인터페이스로 몰입감 증대

4. **확장 가능한 지식 베이스**
   - 벡터 데이터베이스를 활용한 효율적인 정보 검색 및 관리
   - LangChain을 이용한 유연한 AI 파이프라인 구축
![image](https://github.com/user-attachments/assets/e2557b5f-af46-4935-8df0-374df2921a05)
![image](https://github.com/user-attachments/assets/ac2c9263-8d1e-44fe-9099-657f105e97e9)
(html 파일은 텍스트를 시각화 하기위해 넣어놨습니다)


5. **멀티모달 학습 지원**
   - 음성, 텍스트, 시각적 요소를 결합한 종합적 학습 경험 제공

## 🛠 기술 스택

| 분야 | 기술 |
|------|------|
| 프론트엔드 | ![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white) |
| 백엔드 | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white) |
| 음성 합성 (TTS) | ![AWS Polly](https://img.shields.io/badge/AWS_Polly-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white) |
| 음성 인식 (STT) | Web Speech API |
| AI 모델 | ![LLama3](https://img.shields.io/badge/LLama3-4B275F?style=for-the-badge&logo=meta&logoColor=white) (Ollama 활용) |
| 벡터 데이터베이스 | ![Chroma](https://img.shields.io/badge/Chroma-00ADD8?style=for-the-badge) |
| AI 파이프라인 | ![LangChain](https://img.shields.io/badge/LangChain-121D33?style=for-the-badge&logo=chainlink&logoColor=white) |
| 시각화 | Unity 커스텀 이퀄라이저 |

## 📐 시스템 아키텍처

```mermaid
graph TD
    A[방문객] -->|음성 입력| B[Web Speech API]
    B --> C[FastAPI 백엔드]
    C -->|쿼리| D[벡터 데이터베이스]
    D -->|관련 정보| C
    C -->|프롬프트 + 컨텍스트| E[LLama3 모델]
    E -->|생성된 응답| C
    C -->|텍스트| F[AWS Polly]
    F -->|음성 데이터| C
    C -->|음성 + 텍스트| G[Unity 프론트엔드]
    G -->|이퀄라이저 시각화| A
```

## ⏳ 개발 기간
- 전체 개발 기간: 2024-09-10 ~ 2024-09-24

## 👨‍💻 개발자 정보

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/chanhyuckkim">
        <img src="https://github.com/KIMGUUNI/A_EyeF/assets/118683437/278b105e-c98e-4238-a8b3-0a6a54cd0908" width="100px;" alt="김찬혁 프로필 사진"/><br />
        <sub><b>김찬혁</b></sub>
      </a>
    </td>
  </tr>
</table>
---
