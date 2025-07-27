# Dlocker関連のAnsible Playbook

## セットアップ

1. インベントリの修正

    - `inventory.yml`にRHELサーバの情報を追記
    - マネージドノード側でansibleuserの作成及び公開鍵の登録
    - マネージドノード側でrootのパスワード設定
        - パスワードはansible-vaultで暗号化して登録

2. 必要ファイルの配置

    - `private/ansible.pem`を配置しパーミッションを600に設定
    - `private/ansible_vault_pass.txt`にvaultのパスワードを記載したファイルを配置
