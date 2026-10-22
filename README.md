# Smartphone Field Weather Lab v2.0 (오프라인 PWA)

## GitHub Pages 설치
1. 이 폴더의 **내용물 전체** (`index.html`, `service-worker.js`, `manifest.webmanifest`, `icons/`)를 GitHub 저장소의 최상위 경로에 업로드합니다. ZIP 파일 자체를 업로드하지 마세요.
2. Settings → Pages → Deploy from a branch → main → /(root) → Save.
3. `https://<계정>.github.io/<저장소>/`에서 실행합니다. 최초에는 인터넷이 필요합니다.
4. 페이지 로드 후 오프라인 준비 완료 안내를 확인하고 한 번 새로고침합니다. Chrome의 앱 설치/홈 화면에 추가 메뉴를 이용합니다.
5. 비행기 모드로 전환한 뒤 앱을 재실행해 확인합니다.

## 주의
- GPS와 마이크는 사용자가 허용해야 하며 기기/브라우저에 따라 오프라인 GPS 획득이 실패할 수 있습니다.
- 마이크의 저주파 지표는 실제 풍속(m/s)이 아닙니다.
- 기압, 기온, 습도, 일사량, 10m 풍속은 Open-Meteo API 데이터로 인터넷이 있어야 갱신됩니다. 오프라인 시 마지막 값은 저장된 과거 데이터로 표시합니다.
- IndexedDB는 브라우저 저장 데이터 삭제나 저장 공간 부족 시 손실될 수 있습니다. CSV로 정기 백업하세요.
- GitHub Pages는 HTTPS 환경이며 처음 설치와 버전 업데이트 시 인터넷이 필요합니다.
- 네트워크 연결 표시는 브라우저 연결 힌트이며 실제 API 사용 가능 여부는 API 요청 결과로 확인합니다.
