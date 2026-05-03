# 기여 가이드라인

Rust 한국어 문서 프로젝트에 기여해주셔서 감사합니다! 여러분의 참여는 한국 Rust 커뮤니티에 큰 도움이 됩니다.

## 기여하기 전에

- 이 프로젝트는 [행동 강령](CODE_OF_CONDUCT.md)을 따릅니다. 모든 참여자는 서로 존중하고 협력해야 합니다.
- 기여하기 전에 기존 이슈를 확인하거나 새로운 이슈를 생성하여 어떤 작업을 할지 논의하는 것을 권장합니다.

## 문서 번역 및 작성

1.  **Fork 및 Clone**: 이 저장소를 개인 GitHub 계정으로 Fork한 후, 로컬 환경에 Clone합니다.
    ```bash
    git clone https://github.com/YOUR_USERNAME/rust-korean-docs.git
    cd rust-korean-docs
    ```
2.  **브랜치 생성**: 작업할 내용을 위한 새로운 브랜치를 생성합니다.
    ```bash
    git checkout -b feature/your-contribution-name
    ```
3.  **번역 또는 작성**: `docs/` 디렉토리 내에 Markdown 형식으로 문서를 번역하거나 작성합니다.
    - 파일명은 소문자로 작성하고, 단어는 하이픈(-)으로 연결합니다 (예: `getting-started.md`).
    - 번역 시 원문의 의미를 정확하게 전달하는 것을 최우선으로 합니다.
    - 새로운 내용을 작성할 경우, 기존 문서와의 일관성을 유지합니다.
4.  **변경 사항 커밋**: 작업한 내용을 커밋합니다.
    ```bash
    git add .
    git commit -m "feat: Add Korean translation for getting started guide"
    ```
5.  **Push 및 Pull Request**: 변경 사항을 Fork한 저장소에 Push하고, 이 저장소로 Pull Request를 생성합니다.
    ```bash
    git push origin feature/your-contribution-name
    ```
    Pull Request 설명에는 어떤 내용을 변경했는지, 왜 변경했는지 등을 상세하게 작성해주세요.

## 코드 스타일

- Markdown 문법을 준수합니다.
- 가독성을 위해 적절한 줄 바꿈과 공백을 사용합니다.

## 문의

궁금한 점이 있다면 언제든지 이슈를 생성하여 질문해주세요.
