# Smartphone Field Weather Lab v3.0

독립형 오프라인 PWA. GitHub Pages의 저장소 최상위에 ZIP 내부 파일과 icons 폴더를 업로드하세요. ZIP 자체를 올리지 마세요.

- Open-Meteo current API: wind_speed_10m, wind_gusts_10m (m/s). 돌풍비=gust/wind (풍속>0).
- GPS, 마이크, 기상 API, IndexedDB, CSV 기록 및 기준 풍속계와 마이크의 보정점 수집.
- 보정점 5개 이상일 때 참고용 선형 회귀(log10 마이크 지표) 결과 표시. R² 0.6 미만, 음의 기울기, 보정범위 밖은 추정 보류. 연구·실험용이며 검증된 풍속계 대체 불가.
- 기존 v2 IndexedDB 측정 기록은 스키마 업그레이드로 유지.
- 오프라인: 첫 온라인 로딩 및 캐시 후 가능. Open-Meteo 갱신은 온라인에서만 가능.
- 캐시 업데이트 후 새 버전이 반영되지 않으면 페이지 새로고침 및 앱 재실행.
- 파일: index.html, service-worker.js, manifest.webmanifest, icons/icon-192.png, icons/icon-512.png.
