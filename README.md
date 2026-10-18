# 픽셀 오피스 · Pixel Office

**Claude Code와 Codex가 일하는 모습을 픽셀 사무실에서 확인하세요.**

부장에게 만들고 싶은 것을 이야기하면, 부장이 팀을 구성하고 팀장·팀원이 일을 나눕니다. 대화, 회의, 작업 결과와 필요한 승인을 한 화면에서 확인할 수 있는 데스크톱 앱입니다.

[Windows 0.1.0 다운로드](https://github.com/MaoEmong/pixel-office/releases/tag/v0.1.0) · [설치·사용 안내](docs/release/0.1.0/README-KO.md) · [스크린샷 27장](docs/screenshots/README.md) · [문제 해결](docs/환경-문제해결.md)

![픽셀 오피스에서 부장과 세 팀의 작업 상태와 작업 기록을 함께 보는 화면](docs/screenshots/01-hero.jpg)

> **Windows 0.1.0 시험판을 배포합니다.** 사용할 Claude Code·Codex 프로그램과 계정 로그인은 별도로 필요합니다. 확인한 범위와 남은 확인 사항은 [배포 검증 기록](docs/release/0.1.0/VERIFICATION.md)에서 확인하세요.
>
> 아래 사진은 **실제 앱에 소개용 예시 데이터를 넣어 촬영한 화면**입니다. 프로젝트·대화·작업 결과·사용량·연결 상태는 기능 설명을 위한 예시이며, 실제 계정이나 실제 AI 작업 결과를 공개한 사진이 아닙니다. 사진을 누르면 크게 볼 수 있습니다.

## 어떤 앱인가요?

여러 AI의 터미널을 번갈아 확인하는 대신, 누가 어떤 일을 하고 누구의 답을 기다리는지 사무실에서 살펴봅니다. 캐릭터마다 하나의 실제 Claude Code 또는 Codex 작업 세션이 연결됩니다.

| 하고 싶은 일 | 픽셀 오피스에서 하는 방법 |
|---|---|
| 새 프로젝트 시작 | 작업 폴더를 골라 부서와 부장을 만듭니다. |
| 목표와 작업 범위 정리 | 부장과 대화하며 완료 기준을 정합니다. |
| 역할 나누기 | 부장이 팀을 만들고, 팀장이 필요한 팀원을 배치합니다. |
| 진행 상황 확인 | 사무실, 회의, 작업 계획, 단계 기록을 확인합니다. |
| 방향 바꾸기 | 작업 중에도 부장에게 질문하거나 변경 지시를 보냅니다. |
| 실행 여부 판단 | 내 책상에 온 명령을 읽고 허가하거나 거부합니다. |

## 화면으로 살펴보기

### 1. 팀 전체의 상태를 한눈에

부장과 팀별 자리가 구분됩니다. 캐릭터의 움직임, 말풍선, 상태 표시로 작업·질문·보고·사용자 승인 대기를 확인합니다. 원하는 캐릭터를 누르면 오른쪽에 그 멤버의 상세 정보가 열립니다.

![부장과 백엔드·프론트·문서QA팀을 배치한 사무실 전체 화면](docs/screenshots/02-office-overview.jpg)

### 2. 부장과 목표를 정하고, 작업 중에도 대화하기

사용자의 요청과 부장의 답변을 별도 카드로 보여 줍니다. 긴 답변의 제목·목록·표도 구분해 읽을 수 있고, 답변 완료 여부와 최근 대화를 확인할 수 있습니다.

![사용자 요청과 부장의 진행 상황 답변을 구분한 대화 화면](docs/screenshots/03-conversation.jpg)

<details>
<summary>목표와 완료 기준을 정리하는 화면도 보기</summary>

담당 팀과 할 일, 완료 기준을 먼저 합의합니다.

![팀별 담당과 첫 작업 범위 및 완료 기준을 정리한 대화](docs/screenshots/04-goals-and-criteria.jpg)

</details>

### 3. 팀장들의 회의와 결정 과정 확인하기

회의에서 나온 팀별 의견과 부장이 확정한 작업 순서를 따로 읽습니다. 회의 진행 중에는 의견 제출 수와 아직 답변 중인 팀장을 표시합니다.

![팀장별 발언을 구분해서 보여 주는 회의 기록](docs/screenshots/06-team-opinions.jpg)

<details>
<summary>회의 결정과 실시간 진행 상황 보기</summary>

![부장이 확정한 작업 순서와 회의 결정](docs/screenshots/05-meeting-decisions.jpg)

![2차 회의의 의견 제출 수와 팀장별 진행 상태](docs/screenshots/17-meeting-progress.jpg)

</details>

### 4. 작업 계획과 단계별 결과 따라가기

팀별 업무와 완료 기준을 작업 계획에서 확인합니다. 단계가 끝나면 부장이 결과를 검토하고, 완료한 일·검증 내용·다음 진행을 기록합니다. 사용자는 단계마다 진행 버튼을 반복해서 누를 필요 없이 중간 결과를 살펴볼 수 있습니다. 사용자의 판단이 필요한 승인과 질문은 별도로 표시됩니다.

![백엔드와 프론트팀에 배정한 업무와 완료 기준](docs/screenshots/07-work-plan.jpg)

![단계 완료 요약과 검증 결과 및 다음 진행을 기록한 화면](docs/screenshots/08-stage-history.jpg)

### 5. 질문과 보고가 누구에게 가는지 구분하기

**팀원 → 팀장 → 부장 → 사용자** 순서로 질문과 보고를 전달합니다. 팀원과 팀장의 일반 질문은 상위 AI가 처리하고, 부장만 사용자에게 보고하러 옵니다. 화면에서도 받는 사람과 사용자의 응답이 필요한지를 구분합니다.

![프론트팀장에게 보낸 질문과 사용자 답변 불필요 안내](docs/screenshots/14-question-to-lead.jpg)

<details>
<summary>사용자에게 온 질문과 보고하러 이동하는 모습 보기</summary>

부장이 사용자의 판단을 요청하면 `사용자에게 온 질문`으로 표시합니다.

![부장이 사용자에게 확인하는 질문과 답변 선택지](docs/screenshots/16-question-to-user.jpg)

팀원은 직속 팀장에게 결과를 전달합니다.

![프론트팀장에게 보고하러 이동한 화면 개발자](docs/screenshots/23-report-to-manager.jpg)

부장은 사용자 책상으로 와서 결과를 보고합니다.

![사용자에게 보고하러 온 부장](docs/screenshots/24-head-report-to-user.jpg)

</details>

### 6. 필요한 실행은 내용을 읽고 승인하기

실행 허가는 보고 체계와 별개로 사용자에게 표시합니다. 내 책상에서 요청한 멤버와 실제 명령을 확인하고 허가·거부할 수 있습니다.

![실행할 명령과 허가·거부 버튼을 보여 주는 승인 카드](docs/screenshots/15-command-approval.jpg)

### 7. 이미지로 설명하고 확대해서 확인하기

입력창의 첨부 버튼이나 **Ctrl+V**로 참고 이미지와 스크린샷을 보낼 수 있습니다. 보낸 이미지는 대화에 남고, 누르면 확대해서 확인할 수 있습니다. PNG·JPG·WEBP를 한 번에 4장까지 첨부할 수 있으며 한 장당 최대 8MB·1600만 화소를 지원합니다.

![참고 이미지가 첨부된 사용자 요청](docs/screenshots/25-image-request.jpg)

<details>
<summary>첨부 이미지 확대 화면 보기</summary>

![대화의 참고 이미지를 크게 연 미리보기 화면](docs/screenshots/26-image-preview.jpg)

</details>

### 8. 작업 기록·터미널·지시문·보고서 확인하기

멤버를 선택하면 읽은 파일과 실행한 명령을 확인할 수 있습니다. 터미널에서는 해당 세션의 실제 출력을 보고, 지시문에서는 멤버별 작업 원칙을 정합니다. 결과는 보고서 탭에서 다시 읽습니다.

![앱 안에서 멤버의 터미널 출력을 보는 화면](docs/screenshots/09-terminal.jpg)

<details>
<summary>멤버별 지시문과 보고서 보기</summary>

![UI 디자이너에게 적용할 역할과 작업 원칙](docs/screenshots/10-member-instructions.jpg)

![작업 지시와 결과 및 검증 내용을 펼친 보고서](docs/screenshots/11-work-report.jpg)

</details>

### 9. 사용할 AI와 사용량 확인하기

Claude Code만, Codex만, 또는 두 서비스를 함께 사용하도록 선택합니다. 사용량 화면에서는 서비스별 남은 사용량과 멤버별 대화 길이 정보를 확인합니다. 확인하지 못한 값은 미확인 상태로 표시합니다.

![Claude와 Codex 사용량 및 멤버별 대화 길이 정보](docs/screenshots/12-ai-usage.jpg)

<details>
<summary>AI 선택과 실행 환경 점검 화면 보기</summary>

![Claude만·Codex만·두 AI 함께 사용 설정](docs/screenshots/13-ai-selection.jpg)

![AI 연결 상태와 동시 작업 수 및 저장 상태 점검](docs/screenshots/27-environment-check.jpg)

</details>

### 10. 문제가 생기면 원인과 복구 상태 확인하기

진행을 막는 문제는 팝업으로 알리고, 닫은 뒤에도 해결이 필요한 문제를 화면에 남깁니다. 연결 복구를 기다리는 멤버는 일반 오류·퇴근과 구분하며, 기존 업무와 대화의 보존 여부를 안내합니다.

![작업이 멈춘 이유와 필요한 조치를 알려 주는 오류 팝업](docs/screenshots/22-error-popup.jpg)

<details>
<summary>기존 업무를 유지하는 연결 복구 대기 화면 보기</summary>

![기존 업무와 대화를 유지하며 자동 재연결을 기다리는 멤버](docs/screenshots/18-connection-recovery.jpg)

</details>

## 처음 시작하기

1. [Windows 배포 ZIP](https://github.com/MaoEmong/pixel-office/releases/download/v0.1.0/PixelOffice-0.1.0-windows-x64.zip)을 내려받아 **전체**를 새 폴더에 풀고 `pixel_office.exe`를 실행합니다.
2. 사용할 Claude Code 또는 Codex를 설치하고 로그인합니다.
3. `AI 설정 변경`에서 실제 사용할 서비스를 선택하고 연결 상태를 확인합니다.
4. `부서 만들기`에서 작업할 프로젝트 폴더와 부장 AI를 고릅니다.
5. 부장에게 목표와 완료 기준을 설명합니다. 이후 팀 구성·회의·작업 결과를 화면에서 확인합니다.

Windows 배포본에는 앱 실행에 필요한 Node.js와 기본 구성품이 포함됩니다. AI 프로그램 설치와 계정 이용은 각 서비스의 조건을 따릅니다. 상세한 실행·업데이트·백업 방법은 [설치·사용 안내](docs/release/0.1.0/README-KO.md)를 참고하세요.

<details>
<summary>첫 실행·부서 만들기·허가 방식 설정 화면 보기</summary>

![첫 실행에서 부서 만들기를 안내하는 빈 사무실](docs/screenshots/19-first-launch.jpg)

![프로젝트 폴더와 부서 이름 및 부장 AI를 고르는 대화상자](docs/screenshots/20-create-department.jpg)

![실행 허가 방식별 설명을 펼친 부서 설정](docs/screenshots/21-permission-options.jpg)

</details>

## 저장과 재시작

조직과 앱 설정은 PC의 앱 데이터 폴더에, 프로젝트별 대화와 작업 기록은 해당 프로젝트의 `.pixel-office` 폴더에 저장합니다. 재실행하면 기존 세션과 업무의 복구를 시도합니다. 로그인 만료나 실행 권한 문제처럼 사용자의 조치가 필요한 경우에는 화면 안내를 확인하세요.

프로젝트를 옮기거나 업데이트할 때는 앱 데이터와 `.pixel-office`를 함께 백업하세요. `.pixel-office`에는 인증 정보가 포함될 수 있으므로 공유하거나 공개 저장소에 올리지 마세요.

## 더 알아보기

| 문서 | 내용 |
|---|---|
| [전체 스크린샷 갤러리 · 27장](docs/screenshots/README.md) | 기능별 화면과 촬영 기준 |
| [설치·사용 안내](docs/release/0.1.0/README-KO.md) | AI 연결, 사용법, 백업과 업데이트 |
| [문제 해결](docs/환경-문제해결.md) | 설치·로그인·실행 권한·연결 복구 |
| [원격 접속 안내](docs/원격접속.md) | 선택 기능: 다른 기기의 브라우저에서 연결하기 |
| [검증 기록](docs/release/0.1.0/VERIFICATION.md) | 확인한 범위와 실제 환경 확인 사항 |

문제 제보에는 오류 문구, 앱 버전, 사용하는 AI와 재현 순서를 함께 남겨 주세요. 계정 정보나 비공개 프로젝트 내용은 제외해 주세요.

이 저장소는 앱 소개·스크린샷·사용 안내·다운로드 배포용입니다. 앱의 원본 개발 코드는 포함하지 않습니다. 배포 ZIP에도 원본 개발 파일은 제외하며, 실행에 필요한 변환된 JavaScript와 외부 구성품은 포함합니다.
