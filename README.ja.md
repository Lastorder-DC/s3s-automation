# Github Actionsを使用してSplatoon3のバトル履歴をstat.inkにアップロードする
- Github Actionsを利用して、スプラトゥーン3のバトル履歴を自動的にstat.inkにアップロードするように設定します。

## 使用方法
- [日本語ガイド1](https://nerune-jp.com/splatoon3-statink/)や[日本語ガイド2](https://vanillasalt.net/2022/10/10/how-to-use-s3s/)を参考にconfig.txtファイルを作成します。
- Github登録やログイン後、上部の`Use this template` -> `Create a new repository`を押します。
- `Repository name`は適当に決めます。(紛らわしくないように文字名ですることをお勧めします - ただし、英語だけなので、適当に変えて入れることをお勧めします)
- 一番下の`Create repository`ボタンを押します。
- `Settings` -> `Secrets and variables` -> `Actions`を押します。
- New repository secretボタンを押して`Name`は`CONFIG_TXT`で、`Secret`は最初のガイドで作ったconfig.txtファイルの内容を全部入れます。
- 終わり。約5分ごとに(Githubの制限上、たまに10分まで遅延することもあります)自動でアップロードされます。手動アップロードは`Actions` -> `Splatoon3 Battlelog Uploader` -> `Run workflow`ボタンをクリックすることで可能です。
