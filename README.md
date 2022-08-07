# serverpodsample

## Get Started

[severpod.dev](https://docs.serverpod.dev/)

Serverpod is tested on Mac and Linux (Mac recommended), support for Windows is experimental. Before you can install Serverpod, you need to the following tools installed:

- Flutter and Dart. You will need Flutter version 2.10 or later. https://flutter.dev/docs/get-started/install
- Docker. Docker is used to manage Postgres and Redis. https://docs.docker.com/desktop/mac/install/

### Global
1. fvm のGlobalのパスを通しておく
2. serverpod_cliのインストール
    ```
    dart pub global activate serverpod_cli
    ```
3. severpod使えるか確認
    ```
    serverpod
    ```
4. project作成（ハイフン使えない）
    ```
    serverpod mypod
    ```
5. server の作成と起動
    ```
    docker-compose up -d --build
    serverpod run
    or
    dart bin/main.dart
    ```
6. アプリ側の起動（いつも通りにデバッグで良い）