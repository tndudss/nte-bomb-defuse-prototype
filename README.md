# [개인 포트폴리오] 폭탄 이상 해체 — NTE Bomb Defuse Prototype

> **비공식 개인 포트폴리오입니다.** 원작 이환(NTE)의 공식 개발·서비스·배포와 무관한 프로토타입입니다.

이환(NTE)의 폭탄 이상 해체 콘텐츠를 참고해 Unreal Engine으로 구현한 개인 포트폴리오용 프로토타입입니다. 이 저장소는 에디터용 소스와 Windows v0.2 실행 빌드를 제공합니다.

## 시연 영상

https://github.com/user-attachments/assets/9d5374e8-468f-4740-8a48-2fbce33cdcb0

## 플레이 및 다운로드

| 용도 | 링크 |
| --- | --- |
| Windows 실행 파일 다운로드 | [Windows v0.2 릴리스](https://github.com/tndudss/portfolio-nte-bomb-defuse-prototype/releases/tag/v0.2) |
| Unreal 에디터용 소스 | 이 저장소를 클론하거나 **Code → Download ZIP** |

### Windows에서 실행

1. 릴리스의 **Assets**에서 `NTE_BombDefuse_Prototype_v0.2.zip`을 다운로드합니다.
2. ZIP 전체를 새 폴더에 압축 해제합니다.
3. `NTE_BombDefuse_Prototype_v0.2.exe`를 실행합니다.

Unreal Engine 에디터 설치는 필요하지 않습니다. `Engine/`, `BombDefuse_Prototype/` 폴더를 EXE와 함께 유지하세요. Visual C++ 런타임이 필요한 경우 동봉된 `Engine/Extras/Redist/en-us/vc_redist.x64.exe`를 사용하세요.

## Unreal 에디터에서 열기

- 제작 버전: **Unreal Engine 5.7.4** (`.uproject` 엔진 연결: 5.7)
- 시작 맵: `Content/Maps/L_Main.umap`
- 프로젝트 방식: Blueprint

1. Unreal Engine 5.7.4를 설치합니다.
2. 저장소를 클론하거나 ZIP을 내려받아 압축을 해제합니다.
3. Unreal Editor의 프로젝트 브라우저에서 **Browse(찾아보기)**를 선택하고 `BombDefuse_Prototype.uproject`를 엽니다. 파일 연결이 설정돼 있다면 `.uproject`를 더블 클릭해도 됩니다.
4. 셰이더와 에셋 캐시 생성이 끝나면 시작 맵을 열고 Play를 실행합니다.

Blueprint 기반이므로 별도 C++ 소스 빌드는 필요하지 않습니다. 활성화된 `ModelingToolsEditorMode`는 엔진에 포함된 에디터 플러그인입니다.

## 포함 파일

- `BombDefuse_Prototype.uproject`: Unreal 프로젝트 파일
- `Config/`: 엔진, 입력 및 패키징 설정
- `Content/`: Blueprint, 맵, UI, 데이터, 텍스처 및 오디오 리소스
- `Content/__ExternalActors__/`, `Content/__ExternalObjects__/`: 맵의 외부 액터 및 오브젝트 데이터

`Saved/`, `Intermediate/`, `DerivedDataCache/` 등의 캐시와 임시 파일은 버전 관리에서 제외합니다. 실행 빌드는 GitHub Releases에서 배포합니다.

## 구현 범위

- 3분 제한 시간
- 스트라이크 3회 시 실패
- 스위치 / 버튼 / 주파수 / 전선 퍼즐
- 통화형 적층 대화 UI
- 오답 시 RETRY 대사 및 재안내
- 성공 / 실패 결과 화면
