# DOOM / AFTER THE END

GitHub → Vercel 배포용 정적 HTML 게임입니다. 원작과 다른 설정의 비공식 팬 패러디입니다.

## 배포 방법
1. ZIP을 압축 해제합니다.
2. GitHub에서 새 저장소를 만들고 Add file → Upload files로 압축 해제한 파일을 올립니다. ZIP 자체를 올리지 마세요.
3. 저장소 최상위에 index.html과 vercel.json이 보여야 합니다.
4. Vercel에서 Add New → Project를 선택하고 GitHub 저장소를 Import합니다.
5. Framework Preset은 Other, Root Directory는 저장소 루트(기본값)로 둡니다.
6. vercel.json이 빌드·설치 명령을 비우고 출력 폴더를 현재 폴더로 지정합니다. 추가 명령이나 환경 변수는 필요하지 않습니다.
7. Deploy를 누른 뒤 발급된 주소를 엽니다.

이후 GitHub의 배포 브랜치 파일을 수정해 커밋하면 연결된 Vercel 프로젝트가 다시 배포합니다.
기존 Vercel 프로젝트를 재사용한다면 이전 프레임워크·Root Directory 설정을 확인하세요.

## 파일
- index.html: 게임 전체 (CSS, JavaScript 포함)
- vercel.json: 정적 배포 설정
- .gitignore: 로컬 작업 파일 제외

## 조작
WASD / 방향키: 이동 · Space: 회피 · E: 둠 파동 · P: 일시정지.
태블릿: 화면 왼쪽 조이스틱과 하단 버튼. 공격은 자동입니다.
5개 챕터: 쉬헐크 / 정복자 캉 / 닉 퓨리와 스크럴 군단 / 더 마블스 3인 보스 / 아이언하트.
최고 도달 기록은 각 브라우저에 저장되며 다른 기기와 동기화되지 않습니다.
기존 파일을 직접 열어 저장한 기록은 배포 주소로 이전되지 않습니다.

## 로컬 실행
index.html을 브라우저로 열면 됩니다. 외부 패키지나 API 키가 필요하지 않습니다.

## 참고
https://vercel.com/docs/deployments/configure-a-build
https://vercel.com/docs/project-configuration

## 비주얼 패치 0.2
- 첨부한 1번 이미지의 짙은 녹색, 금속성 은색, 역광을 반영한 타이틀·HUD·전장.
- 첨부 이미지 기반 초상 토큰: 둠, 쉬헐크, 캉, 퓨리, 스크럴, 캡틴 마블, 모니카, 미즈 마블, 아이언하트.
- 4레벨: 세 보스 동시 등장, 개별 체력바, 셋 모두 격파 후 진행.
- 캡틴 마블: 황금빛 광자 연사 / 모니카: 청색 원형 탄막·재배치 / 미즈 마블: 보라색 하드라이트 장판.
- 이미지는 index.html 안에 포함되어 별도 assets 폴더나 외부 이미지 서버가 필요 없습니다.
- 기존 저장소의 index.html을 교체하면 적용됩니다.

검증: JavaScript 구문, 5개 챕터 진행, 3인 보스 격파 조건, 강화, 엔딩 로직을 테스트했습니다. 실제 브라우저 화면과 터치 조작은 미검증입니다.
