# Rust 시작하기

Rust를 시작하는 것은 매우 간단합니다. 이 가이드에서는 Rust 개발 환경을 설정하고 첫 번째 Rust 프로그램을 작성하는 방법을 안내합니다.

## Rust 설치

Rust는 `rustup`이라는 도구를 통해 설치하는 것을 권장합니다. `rustup`은 Rust 버전 관리 및 관련 도구를 쉽게 설치하고 관리할 수 있도록 도와줍니다.

터미널을 열고 다음 명령어를 실행하여 `rustup`을 설치합니다:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

설치가 완료되면, Rust 환경 변수를 현재 셸에 적용해야 합니다. 대부분의 경우 설치 스크립트가 자동으로 처리하지만, 수동으로 적용해야 할 수도 있습니다:

```bash
source $HOME/.cargo/env
```

설치가 제대로 되었는지 확인하려면 다음 명령어를 실행합니다:

```bash
rustc --version
cargo --version
```

Rust 컴파일러(`rustc`)와 빌드 시스템 및 패키지 매니저(`cargo`)의 버전 정보가 출력되면 성공적으로 설치된 것입니다.

## 첫 번째 Rust 프로그램 작성하기

이제 Rust 개발 환경이 설정되었으니, 첫 번째 Rust 프로그램을 작성해 봅시다.

1.  새로운 프로젝트 디렉토리를 생성합니다:
    ```bash
    mkdir hello_rust
    cd hello_rust
    ```
2.  `main.rs` 파일을 생성하고 다음 코드를 작성합니다:
    ```rust
    fn main() {
        println!("Hello, Rust!");
    }
    ```
3.  터미널에서 다음 명령어를 실행하여 프로그램을 컴파일하고 실행합니다:
    ```bash
    rustc main.rs
    ./main
    ```

화면에 "Hello, Rust!"가 출력되면 성공입니다!

## Cargo를 이용한 프로젝트 생성

실제 Rust 프로젝트에서는 `cargo`를 사용하여 프로젝트를 관리하는 것이 일반적입니다. `cargo`는 빌드, 테스트, 의존성 관리 등 다양한 기능을 제공합니다.

1.  새로운 Cargo 프로젝트를 생성합니다:
    ```bash
    cargo new my_project
    cd my_project
    ```
2.  `my_project` 디렉토리 안에는 `src/main.rs` 파일과 `Cargo.toml` 파일이 생성됩니다. `src/main.rs` 파일에는 기본 "Hello, world!" 코드가 포함되어 있습니다.
3.  프로젝트를 빌드하고 실행합니다:
    ```bash
    cargo run
    ```

`cargo run` 명령어는 코드를 컴파일하고 실행까지 한 번에 처리해 줍니다.
