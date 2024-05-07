# Uploading Splatoon3 battle logs to stat.ink with Github Actions
- Using Github Actions to automatically upload battle logs from Splatoon 3 to stat.ink.

## How to use
- Check s3s [Setup instructions](https://github.com/frozenpandaman/s3s#setup-instructions-) and create a config.txt file.
- After signing up and logging in to Github, click `Use this template` -> `Create a new repository` at the top.
- Give your repository a name (preferably your character name to avoid confusion - but it's only in English, so you can change it as you see fit).
- Click the `Create repository` button at the bottom.
- Tap Settings -> Secrets and Variables -> Actions.
- Click the `New repository secret` button and enter `CONFIG_TXT` as `Name`, and `Secret` as the full contents of the config.txt file you created in the first guide.
- Done. It will upload battle logs automatically about every 5 minutes (sometimes delayed to 10 minutes due to Github limitations). You can manually upload by clicking `Actions` -> `Splatoon3 Battlelog Uploader` -> `Run workflow` button.
