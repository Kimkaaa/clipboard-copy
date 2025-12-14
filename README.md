# Clipboard Copy Example

버튼 클릭 시 현재 URL을 클립보드에 복사하는 기능을 구현한 간단한 예제입니다.

<br>

## ✨ 주요 기능

- **Clipboard API 우선 사용**: 최신 브라우저 환경에서 표준 API 활용
- **Fallback 지원**: 제한된 환경을 위한 `execCommand('copy')` 방식 구현
- **다양한 브라우저 환경 고려**: 모바일 Safari 등 예외적인 동작 환경 대응

<br>

## 🛠️ 기술 스택

- 순수 HTML5
- Vanilla JavaScript (ES6+)
- No dependencies

<br>

## 🚀 실행 방법

1. 프로젝트 폴더를 VS Code에서 엽니다
2. Live Server 확장을 실행합니다
3. 브라우저에서 열린 페이지의 **URL 복사** 버튼을 클릭
4. 현재 페이지 주소가 클립보드에 복사됩니다

<br>

## 📸 실행 화면

<p align="center">
  <img src="./assets/clipboard-copy-test-img.png" alt="실행 화면" />
</p>

<br>

## 📝 참고사항

- **HTTPS 환경**: Clipboard API는 일반적으로 보안 컨텍스트(HTTPS)에서 동작합니다
- **localhost 예외**: `http://localhost`는 보안 컨텍스트로 간주되어 Clipboard API가 정상 동작합니다
- **file:// 프로토콜**: HTML 파일을 직접 열어 실행할 경우(`file://`), 브라우저 정책에 따라 복사 동작이 달라질 수 있습니다