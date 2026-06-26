# 연세솔안과 드림렌즈/RGP 피팅 가이드

정적 웹앱입니다. GitHub Pages로 배포하면 브라우저에서 바로 사용할 수 있습니다.

## 사용 방법

- 웹앱 URL을 Chrome 또는 Edge에서 엽니다.
- 검사값을 입력하면 드림렌즈, RGP, 공막렌즈 피팅 가이드가 표시됩니다.
- `K5M 붙여넣기` 탭에서 topography 텍스트나 이미지를 붙여넣어 수치를 추출할 수 있습니다.

## 2026-06-26 자료 반영 v2

추가 제공 자료를 기반으로 다음 로직을 보강했습니다.

- OK 중심이탈 troubleshooting: 상측/이측, 하측/비측, lateral decentration, central island, staining/erosion별 수정 방향
- Loose/Tight 판별: movement, fitting curve, alignment curve, edge lift 기준
- OK 처방 경고: 낮은/높은 eccentricity, 난시교정 OK 렌즈의 loose 경향
- RGP 고난시: Supervision toric/back toric 후보와 spectacle cylinder 2/3 rule 표시
- 공막렌즈: Ampleye 4-zone(CVZ, PCZ, LLZ, SLZ)과 central vault/settling 가이드 강화

## OCR 참고

이미지 OCR은 브라우저 내장 OCR을 먼저 사용하고, 없으면 Tesseract.js를 CDN에서 불러옵니다. 인터넷이 차단된 환경에서는 OCR이 실패할 수 있으므로 수치를 직접 입력하거나 텍스트로 붙여넣어 사용하세요.

## 주의

이 도구는 렌즈 피팅 의사결정을 돕는 내부 참고용 가이드입니다. 최종 처방은 진료 소견, slit lamp/fluorescein 소견, 착용 시간, 환자 증상, over-refraction과 함께 판단하세요.
