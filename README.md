# 동작 안함 / Not working / 不動作
- 닌텐도측 보안 강화로 f generation api가 동작하지 않으므로 자동 업로드도 현재는 불가능합니다.
- Since the f generation app does not work due to Nintendo's increased security, automatic uploading is not possible at this time.
- 任天堂側のセキュリティ強化により、fgeneration apiが動作しないため、自動アップロードも現在はできません。

# Github Actions를 사용하여 Splatoon3의 배틀 전적을 stat.ink에 업로드하기
- Github Actions를 이용, 스플래툰 3의 배틀 전적을 자동으로 stat.ink에 업로드하도록 설정
- [日本語の使い方リンク](./README.ja.md)
- [English README](./README.en.md)

## 사용 방법
- [한국어 가이드](https://github.com/cake-monotone/s3s)를 참고하여 config.txt 파일을 생성합니다.
- Github 가입 및 로그인 후 상단 `Use this template` -> `Create a new repository`를 클릭합니다.
- `Repository name`은 적당히 정해줍니다.(헷갈리지 않으려면 캐릭터 이름으로 하는것이 좋습니다 - 단 영어만 가능하니 적당히 바꿔서 넣는게 좋겠죠?)
- 최하단 `Create repository` 버튼을 누릅니다.
- `Settings` -> `Secrets and variables` -> `Actions`를 누릅니다.
- `New repository secret` 버튼을 누르고 `Name`은 `CONFIG_TXT`로, `Secret`은 첫번째 가이드를 따라해 만든 config.txt 파일 내용을 통째로 넣습니다.
- 끝. 약 30분마다(Github 한계상 가끔 지연되기도 함) 자동으로 업로드됩니다. 수동 업로드는 `Actions` -> `Splatoon3 Battlelog Uploader` -> `Run workflow` 버튼 클릭으로 가능합니다.
