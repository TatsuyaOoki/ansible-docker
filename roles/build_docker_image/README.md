# build_docker_image

## 処理内容

1. 実行環境にPythonのdockerパッケージがインストールされているか確認

    **後続のタスクで必要なため、インストールされていない場合は異常終了とする**

2. 一時作業ディレクトリの作成
3. イメージ作成に必要な資材を一時作業ディレクトリに作成
4. Dockerfileを一時作業ディレクトリにコピー
5. dockerイメージのビルド
6. 一時作業ディレクトリの削除

    **途中でタスクが失敗しても一時ディレクトリの削除は実施**

## 変数

| 変数名 | 説明 | 備考 |
| ----- | ----- | ----- |
| build_docker_image_path | Dockerfileのcopy元のパス | |
| build_docker_image_name | 作成するDocker imageの名前 | |
| build_docker_image_tag | 作成するDocker imageのタグ名 | |
| build_docker_image_context_files | ビルドコンテキストに含めるファイル群 | |

## 注記

なし
