# Everyday Vocab: 14 Topics

**일상 영단어 14개 주제**를 카드 형식으로 학습하는 단일 HTML 웹앱입니다.

별도의 서버나 설치 과정 없이 `index.html`만 열면 바로 사용할 수 있습니다. 14개 본문 주제와 국가·수도 부록을 포함하며, 검색·음성 재생·학습 상태 기록을 지원합니다.

## 주요 기능

- 영어 단어, 한국어 뜻, 주제로 검색
- 14개 대분류와 95개 세부 주제 필터
- 단어 및 예문 영어 음성 재생
- 보통/느린 발음 속도 전환
- 순차/랜덤 학습
- 뜻 숨기기
- `낯섦 / 익힘 / 익숙` 학습 상태 기록
- 브라우저 `localStorage`에 진행 상황 자동 저장
- 코드 복사 방식의 학습 기록 내보내기·불러오기
- 모바일 화면 대응
- 단일 HTML 파일로 실행 가능

## 수록 내용

| 구분 | 수량 |
|---|---:|
| 본문 대분류 | 14개 |
| 세부 주제 | 95개 |
| 본문 카드 | 3,360개 |
| 부록 A: 국가·수도 | 197개 |
| 전체 카드 | 3,557개 |
| 전체 예문 | 3,898개 |

기본 **전체 학습**에서는 본문 14개 주제만 표시합니다. 국가·수도 197개는 `부록 A · 국가·수도 색인`을 선택했을 때 학습 목록에 포함되며, 검색에서는 항상 찾을 수 있습니다.

## 14개 주제

1. 사람과 신체 — People and the Body
2. 집과 생활 — Home and Living
3. 쇼핑과 음식 — Shopping and Food
4. 기초 개념·시간·날씨 — Basic Concepts, Time and Weather
5. 패션과 미용 — Fashion and Beauty
6. 동네와 도시 — Neighborhoods and Cities
7. 교통과 여행 — Transportation and Travel
8. 직업과 직장 — Jobs and the Workplace
9. 병원과 의료 — Hospitals and Healthcare
10. 취미·미디어·문화 — Hobbies, Media and Culture
11. 스포츠와 야외활동 — Sports and Outdoor Activities
12. 식물과 동물 — Plants and Animals
13. 학교와 교과 — School and Subjects
14. 세계 지리 — World Geography

**부록 A. 국가·수도 색인 — Countries and Capitals Index**

## 사용 방법

### 웹에서 사용

GitHub Pages를 활성화한 뒤 생성된 주소로 접속합니다.

### 컴퓨터에서 바로 사용

저장소를 내려받은 뒤 `index.html`을 브라우저로 엽니다.

일부 브라우저에서는 영어 음성의 종류와 품질이 운영체제에 설치된 음성 엔진에 따라 달라질 수 있습니다.

## GitHub Pages 배포

1. 이 저장소의 루트에 `index.html`을 둡니다.
2. 저장소의 **Settings → Pages**로 이동합니다.
3. **Build and deployment → Source**에서 `Deploy from a branch`를 선택합니다.
4. 브랜치는 `main` 또는 실제 배포 브랜치, 폴더는 `/(root)`를 선택하고 저장합니다.
5. 배포가 완료되면 표시된 Pages 주소로 접속합니다.

권장 저장소 이름:

```text
everyday-vocab-14-topics
```

일반적인 Pages 주소 형식:

```text
https://<GitHub-ID>.github.io/everyday-vocab-14-topics/
```

## 저장소 구성

```text
.
├─ index.html
├─ README.md
├─ data/
│  ├─ everyday-vocab-14-topics_content_v2.6.xlsx
│  ├─ everyday-vocab-14-topics_content_v2.6.csv
│  └─ everyday-vocab-14-topics_content_v2.6.md
└─ qa/
   └─ QA.json
```

- `index.html`: 실제 웹앱. GitHub Pages 배포에 반드시 필요합니다.
- `README.md`: 프로젝트 소개와 사용 방법입니다.
- `data/`: 웹앱에 반영된 영단어장 원본입니다.
- `qa/QA.json`: 카드 수, 예문 수, 분류 구조 등을 확인한 검수 결과입니다.

웹앱 실행만 필요하다면 `index.html`과 `README.md`만 올려도 됩니다. 데이터 원본과 검수 결과까지 공개하려면 위 구조 전체를 올리는 것을 권장합니다.

## 데이터 형식

동일한 콘텐츠를 세 가지 형식으로 제공합니다.

- **XLSX**: 표 형식 확인과 직접 편집에 적합
- **CSV**: 데이터 처리와 프로그램 연동에 적합
- **Markdown**: GitHub에서 내용을 바로 읽고 검토하기에 적합

웹앱 데이터는 `index.html` 내부에 포함되어 있으므로 실행 시 별도의 CSV나 서버가 필요하지 않습니다.

## 학습 기록

학습 상태는 현재 브라우저의 `localStorage`에 저장됩니다. 브라우저 데이터를 삭제하거나 다른 기기를 사용하면 기록이 자동으로 이동하지 않습니다. 앱의 **저장 / 불러오기** 기능으로 학습 상태 코드를 복사해 옮길 수 있습니다.

## 프로젝트 정보

- 프로젝트명: **Everyday Vocab: 14 Topics**
- 한국어명: **일상 영단어 14개 주제**
- 저장소명: `everyday-vocab-14-topics`
- 콘텐츠 버전: `v2.6`
