# Smart Weather Lab v3.1 — 오류 수정

수정 사항:
- Open-Meteo current 요청에 `wind_gusts_10m` 누락되어 돌풍 및 돌풍비가 표시되지 않던 문제 해결.
- 마이크 미시작 시 그래프에 시작 안내 표시, 오디오 스펙트럼 및 파형 API 호환성 보강, 마이크 오류 안내 개선.
- Service Worker 캐시 버전 변경 및 온라인 탐색 시 최신 HTML 우선 사용으로 오래된 버전 표시 문제 완화.

배포: ZIP 압축 해제 후 `index.html`, `service-worker.js`, `manifest.webmanifest`, `icons/`를 저장소 최상위에 업로드하고 커밋. 배포 후 앱 종료/재실행, 새로고침.

마이크는 사용자가 버튼을 누르고 HTTPS 사이트에 마이크 권한을 허용해야 동작합니다. API 돌풍은 모델 값이며 실제 센서 측정이 아닙니다.
