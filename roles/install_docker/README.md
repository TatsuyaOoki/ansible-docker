# install_docker

## 処理内容

1. 競合パッケージの削除
2. dnf-plugins-coreパッケージのインストール
3. Dockerのリポジトリファイル取得
4. Docker関連パッケージインストール
5. Dockerの起動及び自動起動有効化
6. サービス情報の取得
7. Dockerサービスの情報表示

## 変数

| 変数名 | 説明 | 備考 |
| ----- | ----- | ----- |
| install_docker_packages | install対象のDocker関連サービス | |
| install_docker_remove_conflicting_packages | 削除対象の強豪パッケージ | |
| install_docker_repo_url | DockerリポジトリファイルのURL | |
| install_docker_service_name | Dockerのサービス名 | |

## 注記

なし
