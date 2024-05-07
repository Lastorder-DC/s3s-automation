# Github Actions를 사용하여 Splatoon3의 배틀 전적을 stat.ink에 업로드하기
- Github Actions를 이용, 스플래툰 3의 배틀 전적을 자동으로 stat.ink에 업로드하도록 설정

## 사용 방법
- [한국어 가이드](https://github.com/cake-monotone/s3s)를 참고하여 config.txt 파일을 생성합니다.
- Github 가입 및 로그인 후 상단 Use this template -> Create a new repository를 누릅니다.
- Repository name은 적당히 정해줍니다.(헷갈리지 않으려면 캐릭터 이름으로 하는것이 좋습니다 - 단 영어만 가능하니 적당히 바꿔서 넣는게 좋겠죠?)
- 최하단 Create repository 버튼을 누릅니다.
- Settings -> Secrets and variables -> Actions를 누릅니다.
- New repository secret 버튼을 누르고 Name은 `CONFIG_TXT`로, Secret은 첫번째 가이드를 따라해 만든 config.txt 파일 내용을 통째로 넣습니다.
- 끝. 약 5분마다(Github 한계상 가끔 10분까지 지연되기도 함) 자동으로 업로드됩니다. 수동 업로드는 Actions -> Splatoon3 Battlelog Uploader -> Run workflow 버튼 클릭으로 가능합니다.
