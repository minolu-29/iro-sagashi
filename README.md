# ちがう色さがし

1マスだけ色がちがうタイルを60秒で探し続けるゲーム。到達レベルで「ねむい目」〜「神の目」のランクが決まり、結果画像をXやストーリーにシェアできます。

## ファイル

| ファイル | 役割 |
|---|---|
| `index.html` | ゲーム本体（HTML・CSS・JSを1ファイルに収録） |
| `og.png` | SNSでリンクを貼ったときに出るプレビュー画像 |
| `icon.svg` / `icon-*.png` | ブラウザのタブとホーム画面のアイコン |
| `manifest.webmanifest` | スマホの「ホーム画面に追加」用の設定 |
| `.nojekyll` | GitHub Pagesでそのまま公開するための空ファイル |

## GitHub Pagesで公開する

1. GitHubで新しいリポジトリ `iro-sagashi` を **Public** で作る
2. 「uploading an existing file」から、このフォルダのファイルを全部ドラッグして Commit
3. リポジトリの **Settings → Pages** で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save
4. 1〜2分後、`https://ユーザー名.github.io/iro-sagashi/` で公開される

## 公開後に1か所だけ直す

`index.html` の中にある `USERNAME`（2か所）を自分のGitHubユーザー名に書き換えると、XやLINEでリンクを貼ったときにプレビュー画像が表示されます。

## 遊び方

- スタートを押すと60秒のカウントが始まる
- 色がちがう1マスをタップするとレベルアップ。まちがえると3秒へる
- 盤面は2×2から最大9×9まで細かくなり、色の差もだんだん小さくなる
- ベスト記録はその端末のブラウザに保存される
