# PNG → SVG 변환기

PNG / JPG 이미지를 SVG로 바꿔 주는 웹 프로그램입니다. 브라우저에서 바로 쓸 수 있고, 이미지는 서버로 올라가지 않고 내 기기 안에서만 처리됩니다.

## 변환 방식

- **벡터로 다시 그리기**: 도형으로 다시 그려서 크게 키워도 깨지지 않음 (로고·아이콘·일러스트에 적합)
- **픽셀 그대로**: 픽셀을 네모 도형으로 바꿔 원본과 똑같이 (픽셀아트·작은 아이콘용)
- **원본 그대로 넣기**: PNG를 SVG 안에 그대로 담음 (100% 동일, 벡터 아님)

## 사용한 오픈소스

- [VTracer](https://github.com/visioncortex/vtracer) 1.0.0-alpha.4 — 변환 엔진 (MIT OR Apache-2.0). `vtracer.js`는 npm `@visioncortex/vtracer`의 WebAssembly를 브라우저용으로 감싼 파일입니다.
- [SVGO](https://github.com/svg/svgo) 4.1.0 — SVG 압축 (MIT). `svgo.js`는 공식 브라우저 빌드를 감싼 파일입니다.
