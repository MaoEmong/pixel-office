# Windows 0.1.4 배포본 만들기

이 문서는 비공개 개발 저장소의 빌드 절차입니다. 공개 배포 저장소에는 개발 코드와 빌드 스크립트가 없어, 공개 저장소만으로는 앱을 빌드할 수 없습니다. 앱을 사용할 분은 배포 ZIP을 내려받으세요.

저장소 루트에서 dev/app/tool/package-windows.ps1을 실행합니다. 앱과 내부 프로그램은 0.1.4, Windows 빌드 번호는 1로 맞춥니다.

별도 폴더에서 빌드하며, 기존 실행 중인 앱을 덮어쓰지 않습니다. 공식 Node.js 24.14.1 배포 파일의 SHA256을 검사해 포함합니다. 결과 ZIP과 SHA256, 빌드 결과는 dist/v0.1.4/<시각>에 기록합니다.

ZIP에는 README-KO.md, RELEASE-NOTES.md, FIRST-USE-KO.md, 실행 구성품과 외부 구성품의 사용 조건을 포함합니다. 원본 TypeScript·Dart·소스맵·개발 도구·개인 계정·프로젝트 데이터는 포함하지 않습니다. 실행용 JavaScript와 외부 구성품은 포함됩니다.

ZIP을 새 경로에 다시 풀고 포함된 runtime/node.exe로 dev/app/tool/smoke-windows.mjs <압축 푼 폴더> <새 결과 폴더>를 실행합니다. 이 검사는 기존 사용자의 계정·작업·설정에 연결하지 않습니다.

최종 검사 결과와 제한은 [검증 기록](VERIFICATION.md)에 작성합니다.
