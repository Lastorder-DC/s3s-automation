# Github Actionsを使ってSplatoon3のバトル戦績をstat.inkにアップロードする
- Github Actionsのお勉強がてら、s3s.pyを自動実行してstat.inkにアップロードする設定
## やった手順
- Google Cloud Shell上で、誰かが作ってくれたdockerコンテナを起動
- そこでs3s.pyを実行してconfig.txtを取得
- Githubにpublicレポジトリをつくる
- config.txtの中身はシークレットにしたいので、レポジトリのSettingからSecrets and variablesで、各キーごとに値を保存
- ymlファイルを記述してアクションを設定
- 2時間毎に自動実行されるように記述してあるぽい
