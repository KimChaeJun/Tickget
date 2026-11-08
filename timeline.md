# Tickget 프로젝트 작업 기록

## 기록 범위

| 항목 | 값 |
| --- | --- |
| 프로젝트명 | Tickget |
| 원본 저장소 / 소유자 | KimChaeJun/Tickget / KimChaeJun |
| 본인 소유 여부 / 확인 근거 | 소유 저장소. 연결 계정 KimChaeJun 및 GitHub owner 메타데이터 대조 (E01). 소유권과 코드 저작·개인 기여는 구별함. |
| 저장소 공개 범위 | 공개 |
| 기본 브랜치 / 문서 반영 브랜치 | master / master |
| 확인한 소스 커밋 / 조사 기준일 | 8400154c769b42a2ca352946dddd0c7237a43243 / 2026-11-05 (Asia/Seoul) |
| 기본 브랜치 루트 timeline.md 반영 상태 | 이 문서는 기본 브랜치 루트 timeline.md로 생성하는 기록. 문서 생성 커밋과 위 소스 확인 커밋은 다름. 사이트 등록·배포는 별도 작업. |
| 프로젝트 상태 / 실제 개발 기간 | 멀티플레이 예매·통계·AI 분석 및 좌석 배치 생성 코드가 존재함. 현재 운영 상태는 미확인 / 전체 개발 기간 미확인 |
| 본인 참여 기간 | 미확인. 커밋 날짜를 참여 시작·종료일로 사용하지 않음 (E91). |
| 개인·팀 / 팀 규모·역할 분담 | README와 다수 작성자 이력에서 협업 프로젝트임을 확인. 팀 규모·개인 담당은 미확인 |
| 연혁 날짜 기준 | Git author timestamp를 Asia/Seoul로 변환한 변경 기록일. 문서 작성일과 실제 개발·배포 사건일을 구별함. |

## 포트폴리오 공개용 데이터

프로젝트 전체의 확인된 구현을 설명하는 전달용 JSON입니다. 본인의 역할·참여 기간은 확인 후 채웁니다. 문서 작성만으로 사이트에 자동 등록되지는 않습니다.

```json
{
  "slug": "tickget",
  "title": "Tickget",
  "subtitle": "실제 예매 흐름과 실시간 좌석 경쟁을 재현하는 티켓팅 연습 플랫폼",
  "category": "REALTIME WEB · TICKETING",
  "role": "",
  "roleTags": [],
  "year": "",
  "period": "",
  "award": "",
  "summaryLines": [
    "방 생성부터 대기열·캡챠·좌석 선택·결과 확인까지 예매 연습 흐름을 제공합니다.",
    "WebSocket으로 방과 경기 상태를 연결하고 개인 기록·경기 분석 화면을 구성합니다.",
    "Python API에 경기 분석 리포트와 이미지 기반 좌석 배치 생성 경로가 있습니다."
  ],
  "overviewLines": [
    "티켓팅을 미리 연습하려는 사용자를 위해 여러 사람이 함께 참여하는 예매 시뮬레이션을 구성한 프로젝트입니다.",
    "React 화면, Java 서비스, Python 분석·좌석 배치 처리 모듈이 나뉘어 있습니다.",
    "공연장 좌석 상태, 예매 단계별 기록과 AI 피드백을 연습 경험으로 연결합니다."
  ],
  "tags": [
    "React",
    "TypeScript",
    "FastAPI",
    "OpenCV",
    "WebSocket"
  ],
  "roles": [],
  "technologyStack": [
    {
      "category": "Frontend",
      "description": "예매 연습 화면과 사용자 상태·실시간 메시지를 연결합니다.",
      "technologies": [
        "React",
        "TypeScript",
        "Zustand",
        "WebSocket"
      ]
    },
    {
      "category": "AI & Analytics",
      "description": "경기 이력을 분석 문맥과 피드백 응답으로 구성합니다.",
      "technologies": [
        "Python",
        "FastAPI",
        "Pandas",
        "HTTPX"
      ]
    },
    {
      "category": "Image Processing",
      "description": "공연장 이미지의 좌석 배치 처리와 생성 결과 구성을 담당합니다.",
      "technologies": [
        "OpenCV",
        "NumPy"
      ]
    },
    {
      "category": "Backend",
      "description": "방 서비스 실행 기반입니다.",
      "technologies": [
        "Java",
        "Spring Boot"
      ]
    }
  ],
  "metrics": [],
  "pipeline": [
    {
      "label": "ROOM",
      "description": "공연·연습 조건을 선택하고 방에 참가합니다."
    },
    {
      "label": "PRACTICE",
      "description": "대기열·캡챠·실시간 좌석 선택 등 예매 단계를 진행합니다."
    },
    {
      "label": "RESULT",
      "description": "경기 기록과 개인 통계를 조회합니다."
    },
    {
      "label": "FEEDBACK",
      "description": "이력 기반 분석 리포트와 세션 피드백을 연결합니다."
    }
  ],
  "improvements": [],
  "timeline": [
    {
      "date": "2025-11-16",
      "title": "분석 서버 배포 관련 변경",
      "description": "분석 서버 배포를 제목으로 한 코드 변경이 기록되어 있습니다. 운영 성공을 별도 확인한 것은 아닙니다."
    },
    {
      "date": "2025-11-17",
      "title": "분석 최소 이력·좌석 데이터 보완",
      "description": "분석관 최소 세션 수와 배치 데이터 수정 기록을 확인했습니다."
    },
    {
      "date": "2025-11-18",
      "title": "세션 피드백 응답 보완",
      "description": "LLM 피드백 답변 다양성을 조정한 코드 변경이 기록되어 있습니다."
    },
    {
      "date": "2025-11-26",
      "title": "누락 파일 복원",
      "description": "기본 브랜치에 누락 파일 복구 기록이 반영되어 있습니다."
    }
  ],
  "aiCollaboration": [
    {
      "title": "좌석도 분석과 티켓팅 연습의 구현 근거 정리",
      "tools": "Codex",
      "stage": "문서화",
      "problem": "좌석도 분석과 티켓팅 연습을 포함한 프로젝트를 코드 근거와 함께 설명할 기록이 필요했습니다.",
      "approach": "Codex로 README·실행 코드·의존성·변경 이력을 조사하고, 확인된 처리 흐름과 기술 구성만 timeline.md로 정리했습니다.",
      "humanReview": "기록 작성과 수상 없음은 확인했습니다. 좌석도 처리 오류를 해결할 때 사용한 AI 도구, 주고받은 입력과 직접 검증한 과정은 추가 확인이 필요합니다.",
      "outcome": "구현 기능과 개인 담당 범위·측정값의 확인 공백을 구분한 포트폴리오 자료를 만들었습니다.",
      "evidence": "2026-11-05 Codex 문서 작성 대화 및 timeline.md. 앱 실행·AI 호출·성능 재측정은 수행하지 않았습니다."
    }
  ]
}
```

## 문제와 설계 배경

- 대상·문제: 실제 티켓팅 전에 예매 순서와 좌석 경쟁에 익숙해지고 싶은 사용자 (E02).
- 목표: 여러 사용자의 좌석 선택을 같은 경기 흐름에 연결하고 연습 결과를 돌아볼 수 있도록 구성합니다.
- 제약: 좌석·방 상태 동기화, 공연장마다 다른 배치, 분석에 필요한 경기 이력과 외부 모델 응답을 다룹니다.
- 접근: 웹 UI·방 서비스·분석 서버·좌석 배치 생성 서버로 나누고 각각 API 또는 실시간 메시지로 연결합니다 (E03~E05).
- 성공 판단: 현재 문서는 기능 경로의 존재만 확인했습니다. 실제 예매 성공률 개선이나 운영 성능을 측정한 근거는 없습니다.
- 한계: 전체 구현은 팀 결과물입니다. 개인 역할·참여 기간, 현재 모델·스토리지 설정과 서비스 가용성은 미확인입니다.

## 본인 역할과 기여

대표 직무는 아직 확정하지 않았습니다. 다음은 현재 구현에서 확인한 **담당 범위 확인 후보**이며, 프로젝트 전체 기능을 본인의 기여로 단정하지 않습니다. Git 작성자는 변경 추적의 단서로만 사용합니다 (E91).

| 영역 | 확인한 구현·의사결정과 개인 확인 범위 | 개인·팀 경계 | 근거 |
| --- | --- | --- | --- |
| 예매 UI·실시간 상태 | 방·좌석·인증·실시간 연결 구현이 존재함. 직접 담당한 화면·메시지 처리는 확인 필요. | 개인·팀별 담당 미확인 | E02, E03 |
| 분석·좌석 생성 | 분석 리포트·세션 피드백·배치 생성 코드가 존재함. 설계·구현·외부 모델 통합의 개인 범위는 확인 필요. | 개인·팀별 담당 미확인 | E04, E05, E20~E22 |
| 서비스 분리·통합 | Java 방 서비스와 Python API가 나뉨. 백엔드·배포·통합 중 직접 수행한 범위 확인 필요. | 개인·팀별 담당 미확인 | E06 |

## 기술별 사용 내역

기술명은 확인한 코드·문서·매니페스트에서 실제 사용 맥락이 드러나는 항목만 기록했습니다. 아래 목록은 저장소 스택이며 개인 숙련도 목록이 아닙니다.

| 그룹 | 기술 | 용도·사용 위치 | 본인 사용 여부 | 상태 | 근거 |
| --- | --- | --- | --- | --- | --- |
| Frontend | React | 라우터 기반 웹 화면; [Frontend/src/App.tsx](Frontend/src/App.tsx) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E03 |
| Frontend | TypeScript | 웹 UI와 통신 타입; [Frontend/src/shared/lib/websocket.ts](Frontend/src/shared/lib/websocket.ts) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E03 |
| Frontend | Zustand | 인증 사용자 상태 관리; [Frontend/src/features/auth/store.ts](Frontend/src/features/auth/store.ts) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E03 |
| Frontend | WebSocket | STOMP/SockJS 기반 실시간 메시지 연결; [Frontend/src/shared/lib/websocket.ts](Frontend/src/shared/lib/websocket.ts) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E03 |
| AI & Analytics | Python | 분석 서버와 리포트 처리; [AI/AI_analyst/analysis_main.py](AI/AI_analyst/analysis_main.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E04 |
| AI & Analytics | FastAPI | 분석·리포트 HTTP API; [AI/AI_analyst/analysis_main.py](AI/AI_analyst/analysis_main.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E04 |
| AI & Analytics | Pandas | 리포트 입력 데이터와 문맥 구성; [AI/AI_analyst/LLM_main.py](AI/AI_analyst/LLM_main.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E04 |
| AI & Analytics | HTTPX | 외부 모델 서버 비동기 요청; [AI/AI_analyst/analysis_main.py](AI/AI_analyst/analysis_main.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E04 |
| Image Processing | OpenCV | 이미지·마스크·영역 처리; [AI/seatmap_to_html/main_modular.py](AI/seatmap_to_html/main_modular.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E05 |
| Image Processing | NumPy | 영상 배열과 좌표 계산; [AI/seatmap_to_html/main_modular.py](AI/seatmap_to_html/main_modular.py) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E05 |
| Backend | Java | 방 서비스 애플리케이션; [Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java](Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E06 |
| Backend | Spring Boot | Java 서비스 초기화와 서버 실행; [Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java](Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java) | 확인 필요 | 확인 커밋에서 사용; 현재 운영 여부 미확인 | E06 |

## 성과와 검증

| 항목·값 | 측정일·환경·집계 대상 | 방법·출처 | 제한·근거 |
| --- | --- | --- | --- |
| 기능 경로 | 2026-11-05; 확인 커밋의 소스 | README·진입점·API·클라이언트 대조 | E02~E06. E2E·외부 모델 호출 미실행. |
| 정량 성과·성능 | 측정 로그 미확인 | 동시 사용자 수·지연·예매 성공률 개선 수치 없음 | metrics=[]; 테스트 파일 수·README 기능 개수를 성과로 쓰지 않음 (E92). |

신규 실행 결과나 개선율은 없습니다. 코드·문서로 확인한 범위와 과거 기록의 한계를 구별하며, 서로 다른 테스트 집합을 합산하지 않습니다 (E92).

### 수상·외부 평가

수상 이력 없음. 2026-11-05 사용자 확인에 근거하며 공개 JSON의 award는 빈 문자열로 유지합니다 (E90). 외부 평가나 고객·사용자 수는 확인되지 않았습니다.

## 문제 해결과 개선

| 문제·제약 | 확인된 접근·변경과 이유 | 정적 검증 범위 | 남은 한계·근거 |
| --- | --- | --- | --- |
| 복수 사용자의 방·경기 상태 공유 | STOMP/SockJS 연결과 상태 저장소로 실시간 이벤트를 처리 | 클라이언트 연결 코드·README 대조 | 메시지 유실·동시성·부하 재현은 미수행 (E03). |
| 경기 결과를 연습 피드백으로 연결 | 이력 기반 차트·프롬프트·리포트·세션 피드백 API 분리 | API와 응답 구성 코드 확인 | 모델 응답 품질·비용·외부 API 장애 시 동작 미검증 (E04). |
| 공연장마다 다른 좌석 배치 | 이미지 처리와 생성 결과 저장·응답 경로 구성 | OpenCV/NumPy 및 API 구현 확인 | 변환 정확도와 전후 작업 시간은 미측정 (E05). |

상기 내용은 설계 선택과 현재 구현을 설명합니다. 비교 가능한 과거 구현·전후 측정이 부족하므로 공개 JSON의 improvements는 빈 배열로 두었습니다.

## 상세 작업 기록

날짜는 모두 연도를 포함한 KST 변경 기록일입니다. 조사한 대표 커밋만 수록하며 전체 개발 기간이나 모든 작업을 뜻하지 않습니다.

### 2025-11-16 / 분석 서버 배포 관련 변경

- 상태: 코드 이력 확인. 실제 실행·배포 성공 여부는 별도 검증하지 않았습니다.
- 기록된 작업: 분석 서버 배포를 제목으로 한 코드 변경이 기록되어 있습니다. 운영 성공을 별도 확인한 것은 아닙니다.
- 수행 주체: 저장소 변경 기록입니다. 개인 담당 범위는 아래 기여 확인 항목과 구별합니다.
- 산출물·근거: `1c5367ee9d0a4b14502fd77a3860d8c406388ab7` (E20). 커밋 메시지와 현재 구현·문서 범위에서 확인했습니다.

### 2025-11-17 / 분석 최소 이력·좌석 데이터 보완

- 상태: 코드 이력 확인. 실제 실행·배포 성공 여부는 별도 검증하지 않았습니다.
- 기록된 작업: 분석관 최소 세션 수와 배치 데이터 수정 기록을 확인했습니다.
- 수행 주체: 저장소 변경 기록입니다. 개인 담당 범위는 아래 기여 확인 항목과 구별합니다.
- 산출물·근거: `86b42a69a7bb24f9e50339eaefb67e5016e2e8db` (E21). 커밋 메시지와 현재 구현·문서 범위에서 확인했습니다.

### 2025-11-18 / 세션 피드백 응답 보완

- 상태: 코드 이력 확인. 실제 실행·배포 성공 여부는 별도 검증하지 않았습니다.
- 기록된 작업: LLM 피드백 답변 다양성을 조정한 코드 변경이 기록되어 있습니다.
- 수행 주체: 저장소 변경 기록입니다. 개인 담당 범위는 아래 기여 확인 항목과 구별합니다.
- 산출물·근거: `d3be3210566f00b1bddf1b5f55614abe3ed091b3` (E22). 커밋 메시지와 현재 구현·문서 범위에서 확인했습니다.

### 2025-11-26 / 누락 파일 복원

- 상태: 코드 이력 확인. 실제 실행·배포 성공 여부는 별도 검증하지 않았습니다.
- 기록된 작업: 기본 브랜치에 누락 파일 복구 기록이 반영되어 있습니다.
- 수행 주체: 저장소 변경 기록입니다. 개인 담당 범위는 아래 기여 확인 항목과 구별합니다.
- 산출물·근거: `a2f2938f984060026e701f7b3295cb22de17f93a` (E23). 커밋 메시지와 현재 구현·문서 범위에서 확인했습니다.

### 2026-11-05 / 프로젝트 기록 작성

- 상태: 문서 작성.
- 수행 내용: 기본 브랜치의 README·구현 코드·매니페스트·Git 기록을 대조하고 공개용 JSON, 기술 사용 내역, 근거 색인과 확인 항목을 작성했습니다.
- 검증: JSON 파싱·필수 키·배열 항목 구조·근거 경로를 검사했습니다. 애플리케이션 실행이나 과거 테스트 재실행은 수행하지 않았습니다.
- 수상: 사용자가 수상 이력이 없다고 확인한 내용을 반영했습니다 (E90).

## 다음 계획

아래는 자료에서 확인한 미수행 계획 또는 기록 보완 과제입니다. 완료 이력·성과에 포함하지 않습니다.

- 실제 담당한 분석·좌석 생성·프런트엔드·인프라 범위를 확인해 역할을 채웁니다.
- 외부 모델·스토리지 접근이 가능한 별도 환경에서 기능과 오류 흐름을 재현하고 측정 조건을 남깁니다.

## 공개 자료

| 항목 | 값 | 공개 여부·한계 |
| --- | --- | --- |
| 서비스·데모 URL (liveUrl) | 빈 값 | 현재 유효한 공개 운영 주소를 검증하지 않음. 로컬·임시·사내 주소는 공개 URL로 옮기지 않음. |
| 공개 저장소 URL (githubUrl) | https://github.com/KimChaeJun/Tickget | GitHub 공개 저장소 메타데이터 확인 |
| 대표 이미지 (coverImage) | 빈 값 | 대표 이미지와 재사용 가능 범위 미확인 |
| 이미지 대체 텍스트 / 시연·발표 자료 | 미확인 | 검증한 공개 대표 자료가 없으면 링크·설명을 생성하지 않음 |

## 근거 색인

소스 위치는 위 확인 커밋을 기준으로 읽습니다. 비공개 원문의 코드·비밀값·사내 주소는 복사하지 않고 최소한의 상대 경로와 커밋만 기록합니다. 공개용 문자열에는 근거 ID나 구현 경로를 넣지 않습니다.

| ID | 뒷받침하는 필드·주장 | 출처 종류·참조 | 출처 시점 | 확인 내용·한계 | 공개 범위 |
| --- | --- | --- | --- | --- | --- |
| E01 | slug, title, 기록 범위와 소유·브랜치·버전 | GitHub 저장소 메타데이터·기본 브랜치 파일 목록 | 2026-11-05 | 소유자 KimChaeJun, 확인 커밋 8400154c769b42a2ca352946dddd0c7237a43243; 전체 트리 비절단, 조사 당시 timeline.md 없음. 저장소 생성일·push일은 참여 기간으로 사용하지 않음. | 공개 |
| E02 | subtitle, category, summaryLines, overviewLines, pipeline, 문제 배경 | 문서·코드 / [README.md](README.md), [AI/AI_analyst/analysis_main.py](AI/AI_analyst/analysis_main.py), [AI/seatmap_to_html/main_modular.py](AI/seatmap_to_html/main_modular.py) | 8400154c769b | README는 프런트엔드 중심 소개이며, AI 분석·좌석 배치 생성은 별도 Python 구현과 대조함. 팀 전체 구현과 본인 기여를 구분함. | 공개 |
| E03 | technologyStack[0], 화면·상태·실시간 통신 | 문서·코드 / [Frontend/package.json](Frontend/package.json), [Frontend/src/App.tsx](Frontend/src/App.tsx), [Frontend/src/features/auth/store.ts](Frontend/src/features/auth/store.ts), [Frontend/src/shared/lib/websocket.ts](Frontend/src/shared/lib/websocket.ts) | 8400154c769b | React 라우팅·Zustand 인증 상태·STOMP/SockJS 연결 코드를 확인함. 패키지 버전을 운영 검증 결과로 해석하지 않음. | 공개 |
| E04 | technologyStack[1], 분석 API·리포트 흐름 | 문서·코드 / [AI/AI_analyst/analysis_main.py](AI/AI_analyst/analysis_main.py), [AI/AI_analyst/LLM_main.py](AI/AI_analyst/LLM_main.py), [AI/AI_analyst/requirements.txt](AI/AI_analyst/requirements.txt) | 8400154c769b | FastAPI 분석·차트·리포트·세션 피드백 경로와 HTTPX 기반 모델 호출, Pandas 기반 문맥 구성을 확인함. 외부 모델 호출은 실행하지 않음. | 공개 |
| E05 | technologyStack[2], 좌석 배치 생성·이미지 처리 | 문서·코드 / [AI/seatmap_to_html/main_modular.py](AI/seatmap_to_html/main_modular.py), [AI/seatmap_to_html/requirements.txt](AI/seatmap_to_html/requirements.txt) | 8400154c769b | 이미지 업로드·OpenCV/NumPy 처리·좌석 컴포넌트/메타데이터 생성 및 오브젝트 저장 연동 코드가 있음. 특정 스토리지 운영과 생성 품질은 미검증. | 공개 |
| E06 | technologyStack[3], Java 서비스 | 문서·코드 / [Backend/room-server/build.gradle](Backend/room-server/build.gradle), [Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java](Backend/room-server/src/main/java/com/tickget/roomserver/RoomServerApplication.java) | 8400154c769b | Java Spring Boot 방 서비스의 실제 애플리케이션 진입점과 빌드 구성을 확인함. 모든 백엔드 서비스의 동작을 전수 검증하지 않음. | 공개 |
| E20 | timeline[0], 상세 작업 기록 | Git commit / 1c5367ee9d0a4b14502fd77a3860d8c406388ab7 | 2025-11-16 KST | 커밋 기록: feat: 분석가 서버 배포 (analyst-server). 변경 기록일이며 착수·배포·수상일 또는 개인 수행 확정 근거로 확대하지 않음. | 공개 |
| E21 | timeline[1], 상세 작업 기록 | Git commit / 86b42a69a7bb24f9e50339eaefb67e5016e2e8db | 2025-11-17 KST | 커밋 기록: refactor: 분석관 최소 세션 수 지정 및 json 데이터 수정. 변경 기록일이며 착수·배포·수상일 또는 개인 수행 확정 근거로 확대하지 않음. | 공개 |
| E22 | timeline[2], 상세 작업 기록 | Git commit / d3be3210566f00b1bddf1b5f55614abe3ed091b3 | 2025-11-18 KST | 커밋 기록: refacter: report-toast-llm에서 생성되는 답변 다양하게 나오게 변경. 변경 기록일이며 착수·배포·수상일 또는 개인 수행 확정 근거로 확대하지 않음. | 공개 |
| E23 | timeline[3], 상세 작업 기록 | Git commit / a2f2938f984060026e701f7b3295cb22de17f93a | 2025-11-26 KST | 커밋 기록: chore: 누락된 파일들 복구. 변경 기록일이며 착수·배포·수상일 또는 개인 수행 확정 근거로 확대하지 않음. | 공개 |
| E90 | award, 수상·외부 평가 | 사용자 진술 / 이 작업의 채팅 | 2026-11-05 KST | 사용자가 선택한 8개 프로젝트에 수상 이력이 없다고 확인함. award는 빈 문자열이며 미확인 수상을 만들지 않음. | 사용자 확인 사실; 대화 원문은 복사하지 않음 |
| E91 | role, roleTags, roles, year, period와 개인 기여 | 자료 공백 / 확인한 문서·코드·Git 이력의 범위 | 2026-11-05 | 담당 직무·전체 참여 기간·개인/팀 규모는 별도 확인이 필요함. Git 작성자 계정, 저장소 소유권, 제공 코드의 존재만으로 직접 기여를 확정하지 않음. | 미확인 |
| E92 | metrics, 성과와 검증 | 정적 조사 / 본 문서 작성 절차 | 2026-11-05 | 애플리케이션 실행·모델 학습·외부 API 호출·운영 환경 변경은 수행하지 않음. 문서의 JSON 형식·필수 키·근거 경로를 검증함. 과거 문서 수치는 아래 한계와 함께 보존하며 신규 실측값으로 표시하지 않음. | 검증 범위 공개 가능 |

## 확인 필요 / 해당 없음

| 항목 | 상태 | 현재 알려진 사실 | 추가 확인 |
| --- | --- | --- | --- |
| 대표 역할·개인 기여 | 미확인 | role은 빈 문자열, roleTags·roles는 빈 배열. 아래 후보 영역을 개인 실적으로 확정하지 않음. | 본인이 수행한 기능·설계·검증·협업 범위 확인 |
| 참여·개발 기간 / year | 미확인 | year·period는 빈 문자열. 소스 연혁은 별도로 보존. | 실제 시작·종료 또는 진행 중 여부와 참여 기간 확인 |
| 팀 규모·역할 분담 | 미확인 | README와 다수 작성자 이력에서 협업 프로젝트임을 확인. 팀 규모·개인 담당은 미확인 | 원 팀원 수와 역할 분담표 확인 |
| 수상 | 해당 없음 | 사용자 확인에 따라 수상 이력 없음 (E90). | 없음 |
| 성과 수치 / metrics | 미확인 | 신규 실측값 없음. metrics는 빈 배열이며 미측정 수치를 0으로 대체하지 않음. | 동일 조건의 측정 로그·기간·환경·집계 대상 확인 |
| 실행·테스트 | 미실행 | 이번 작업은 정적 조사와 문서 검증. 테스트 코드의 존재를 통과 결과로 바꾸지 않음 (E92). | 필요한 실행 환경에서 별도 재현 |
| 실서비스·AI 모델 운영 | 미확인 | 소스에는 모델 호출·스토리지 설정 경로가 있으나 현재 접근성과 실제 운영 모델은 검증하지 않음. | 실행 환경·배포 기록·응답 품질 근거 |
| 기간·수상 혼동 | 확인 필요 | SSAFY 프로젝트라는 메타데이터만으로 참여 기간·수상을 정하지 않음. | 실제 참여 기록 |

## 사이트 반영 메모

- 문서 위치: 소유 저장소 기본 브랜치 `master`의 루트 `timeline.md`. 해당 브랜치에 생성된 문서가 사이트 수록 여부를 검토할 근거입니다.
- 역할·기여·참여 기간·팀 규모는 확인 후 공개 데이터를 보완합니다. AI PM은 선택하지 않았으므로 추가하지 않았습니다.
- 수상 표시와 미측정 성과 카드는 숨겨야 하며, 빈 문자열·빈 배열을 가상의 값으로 대체하지 않습니다.
- 공개 URL·대표 이미지가 확인되기 전에는 관련 링크·일러스트를 임의로 만들지 않습니다.
- 이번 작업은 해당 저장소 문서 작성입니다. 포트폴리오 데이터 수정·사이트 등록·배포는 수행 범위에 포함하지 않습니다.

## AI 에이전트 활용 기록

추가 조사일: 2026-11-09. 개발자가 문제를 해결할 때 사용한 AI 도구의 기록이다. 서비스 안의 OCR·LLM·예측 모델 기능과 구분한다. 기존 개발 연혁을 이번 기록 보완일로 바꾸지 않는다.

### 확인된 사례

#### 1. 좌석도 분석과 티켓팅 연습의 구현 근거 정리

- 활용 도구: Codex
- 활용 단계: 문서화
- 문제 상황: 좌석도 분석과 티켓팅 연습을 포함한 프로젝트를 코드 근거와 함께 설명할 기록이 필요했습니다.
- AI와 진행한 작업: Codex로 README·실행 코드·의존성·변경 이력을 조사하고, 확인된 처리 흐름과 기술 구성만 timeline.md로 정리했습니다.
- 나의 판단·검토: 기록 작성과 수상 없음은 확인했습니다. 좌석도 처리 오류를 해결할 때 사용한 AI 도구, 주고받은 입력과 직접 검증한 과정은 추가 확인이 필요합니다.
- 결과와 한계: 구현 기능과 개인 담당 범위·측정값의 확인 공백을 구분한 포트폴리오 자료를 만들었습니다.
- 확인 근거: 2026-11-05 Codex 문서 작성 대화 및 timeline.md. 앱 실행·AI 호출·성능 재측정은 수행하지 않았습니다.

### 근거와 공개 범위

2026-11-05 Codex 대화 「timeline.md 없는 프로젝트 목록화」에서 해당 저장소의 README·코드·Git 이력을 조사하고 timeline.md를 작성·반영했다. 사용자는 선택한 8개 프로젝트의 수상 이력이 없음을 확인했다. 상세 근거는 본 문서의 기존 근거 색인을 따른다. 이 기록 작성은 최초 개발 당시의 AI 코딩 사용 근거가 아니다.

대화 원문, 인증정보, 비공개 코드와 개인정보는 공개용 데이터에 포함하지 않는다. AI 초안의 주장, 코드의 존재, 실행 결과, 사용자 확인을 서로 다른 근거로 구별한다.

### 추가로 필요한 본인 기록

좌석 구역 분할·배경/색상 오류·결과 변환·API 구현 중 AI와 해결한 실제 사례, 제공한 이미지/로그/코드, 채택·수정한 대안과 확인 결과.

다음 형식으로 보완: **문제 상황 / 사용 도구 / 제공한 입력·요청 / AI 제안 / 직접 채택·수정·기각한 판단 / 검증 방법·결과**. 모르는 도구명·날짜·개선율은 추정하지 않는다.
