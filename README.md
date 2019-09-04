## How to use
### yarn workspaces
- working directory でeslintを使う場合は以下のファイルを作成する
- directoryは各プロジェクトによって変わってくる
- `.vscode/settings.json`
```json
{
  "eslint.workingDirectories": [
    { "directory": "./packages/console", "changeProcessCWD": true },
    { "directory": "./packages/services", "changeProcessCWD": true }
  ]
}
```
- working directoryを使う場合はeslintの設定ファイルもそれぞれのpackageに移す必要あり
