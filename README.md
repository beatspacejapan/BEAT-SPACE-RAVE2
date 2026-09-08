# BEAT SPACE RAVE 登録サイト

## GitHub Pages での公開手順

1. GitHubで新しいリポジトリを作成する
   例: `beat-space-rave`
   (Public / Private どちらでも公開できますが、無料プランでPagesを使うなら Public 推奨)

2. このZIPに入っている `index.html` を、作成したリポジトリの一番上の階層（ルート）にアップロードする
   - GitHubのリポジトリ画面 →「Add file」→「Upload files」→ `index.html` をドラッグ＆ドロップ
   - ファイル名は必ず `index.html` のままにしてください

3. リポジトリの「Settings」タブ →左メニューの「Pages」を開く

4. 「Build and deployment」の「Source」を **Deploy from a branch** にし、
   Branch を **main**（または master）/ フォルダを **/(root)** に設定して「Save」

5. 数分待つと、ページ上部に
   `Your site is live at https://ユーザー名.github.io/リポジトリ名/`
   と表示されます。そのURLがゲスト登録サイトの本番URLです。

6. スマホでそのURLを開き、実際に登録テストを行い、Googleスプレッドシートに
   反映されることを確認してください。

## 注意点

- `index.html` は単体のファイルで完結しており、画像やロゴもすべて内部に
  埋め込まれています。他のファイルをアップロードする必要はありません。
- Googleスプレッドシートと連携するWebhook URLは既に `index.html` 内に
  設定済みです（Apps Scriptのデプロイ URL）。変更する場合はファイル内の
  `SHEET_WEBHOOK_URL` を書き換えてください。
- サイトの内容を修正したい場合は、GitHub上で `index.html` を直接編集する
  か、新しいファイルをアップロードして上書きしてください。
