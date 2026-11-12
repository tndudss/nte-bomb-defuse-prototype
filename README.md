# NTE Bomb Defuse Prototype

이환(NTE)의 폭탄 이상 해체 콘텐츠를 Unreal Engine으로 구현한 포트폴리오용 프로토타입입니다. 핵심 플레이 루프를 검증하는 것을 목적으로 합니다.

## 개발 환경

- Unreal Engine **5.7.4** (`.uproject` 엔진 연결: 5.7)
- Windows
- Blueprint 기반 프로젝트

## 구현 범위

- 3분 제한 시간
- 스트라이크 3회 시 실패
- 스위치 / 버튼 / 주파수 / 전선 퍼즐
- 통화형 적층 대화 UI
- 오답 시 RETRY 대사 및 재안내
- 성공 / 실패 결과 화면

## 실행 방법

1. 이 저장소를 클론합니다.
2. Unreal Engine 5.7.4에서 `BombDefuse_Prototype.uproject`를 엽니다.
3. 시작 맵인 `Content/Maps/L_Main.umap`에서 Play를 실행합니다.

첫 실행 시 셰이더와 에셋 캐시 생성에 시간이 걸릴 수 있습니다.

## 프로젝트 구조

| 경로 | 내용 |
| --- | --- |
| `Config/` | 엔진, 입력 및 패키징 설정 |
| `Content/Blueprints/` | Blueprint 에셋 |
| `Content/UI/` | UI 에셋 |
| `Content/Data/` | 데이터 에셋 |
| `Content/Maps/` | 시작 맵과 관련 에셋 |
| `Content/Textures/`, `Content/Audio/` | 이미지 및 오디오 리소스 |
| `Content/__ExternalActors__/`, `Content/__ExternalObjects__/` | 맵의 외부 액터 및 오브젝트 데이터 |

`Saved/`, `Intermediate/`, `DerivedDataCache/` 등 자동 생성 파일은 버전 관리에서 제외합니다. 실행 빌드와 ZIP 파일은 이 소스 저장소에 포함하지 않습니다.
