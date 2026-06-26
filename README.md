# 연세솔안과 드림렌즈/RGP 피팅 가이드

정적 웹앱입니다. GitHub Pages로 배포하면 브라우저에서 바로 사용할 수 있습니다.

## 사용 방법

- 메인 앱: https://totenhaft.github.io/lens-fitting-guide/
- 보유 렌즈 추천 페이지: https://totenhaft.github.io/lens-fitting-guide/inventory.html
- 검사값을 입력하면 드림렌즈, LK 드림렌즈, Paragon CRT, RGP, 공막렌즈 피팅 가이드가 표시됩니다.
- `K5M 붙여넣기` 탭에서 topography 텍스트나 이미지를 붙여넣어 수치를 추출할 수 있습니다.

## 2026-06-26 자료 반영 v5

실제 병원 보유 렌즈 재고를 기준으로 추천 렌즈를 고르는 전용 페이지를 추가했습니다.

- `inventory.html` 추가
- 계산된 Final FK가 43.45D처럼 나오더라도 실제 렌즈 step에 맞춰 43.50D 등으로 반올림
- Google Sheet 범위 복사/붙여넣기 또는 CSV/TSV 붙여넣기 지원
- 재고표의 Lens, Model, FK, Power, Dia, Cyl, Qty 컬럼 자동 인식
- FK/A.C, Power, Dia, Cyl, 모델명을 점수화해 보유 렌즈 후보 순위 표시
- 재고표는 브라우저 localStorage에 저장되어 다음 방문 때도 유지

## 2026-06-26 자료 반영 v4

LK 드림렌즈 교육자료를 기반으로 다음 로직을 추가했습니다.

- LK CH2 / Premier / Premier Toric 전용 탭 추가
- LK 초기 처방: Flat-K 기반 A.C 후보, Target Power, B.C 후보, Dia 후보 계산
- Eccentricity 보정: Ecc 0.30-0.39 steep, 0.46-0.54 on K, 0.55 이상 flat 방향 보정
- HVID 기준 Dia 후보: 10.2 / 10.6 / 11.0mm 선택 보조
- Premier Toric 적용: 각막난시 1D 이상 또는 centration 불안정 시 고려
- LK troubleshooting: superior, inferior, lateral decentration, central island, chemical damage별 수정 방향
- Troubleshooting 탭에 `LK 드림렌즈` 렌즈군 추가

기존 v3 내용도 유지됩니다.

- Paragon CRT 전용 탭: BC, RZD, LZA, OAD, OR target, Dual Axis 후보 계산
- CRT troubleshooting: 상방/하방/측방 이탈, central island, fake central island, pooling별 수정 방향
- Onfit 공막렌즈 분기: central clearance, limbal clearance, scleral landing/haptic alignment 중심 안내
- OK 중심이탈 troubleshooting: 상측/이측, 하측/비측, lateral decentration, central island, staining/erosion별 수정 방향
- RGP 고난시: Supervision toric/back toric 후보와 spectacle cylinder 2/3 rule 표시

## OCR 참고

이미지 OCR은 브라우저 내장 OCR을 먼저 사용하고, 없으면 Tesseract.js를 CDN에서 불러옵니다. 인터넷이 차단된 환경에서는 OCR이 실패할 수 있으므로 수치를 직접 입력하거나 텍스트로 붙여넣어 사용하세요.

## 주의

이 도구는 렌즈 피팅 의사결정을 돕는 내부 참고용 가이드입니다. 최종 처방은 진료 소견, slit lamp/fluorescein 소견, 착용 시간, 환자 증상, over-refraction과 함께 판단하세요.
