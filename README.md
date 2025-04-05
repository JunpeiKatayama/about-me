# 職務経歴書 (Web 版)

<br/>

**このリポジトリは、私の職務経歴書を Web ページとして公開するためのものです。**

最新の内容は、GitHub Pages で公開されている以下の URL からご覧いただけます。

[https://JunpeiKatayama.github.io/about-me/](https://JunpeiKatayama.github.io/about-me/)

---

## このページについて

この Web ページは、`resume.md` という Markdown ファイルに記述された職務経歴の内容を、クライアントサイドの JavaScript ライブラリ (`marked.js`) を使用して動的に HTML へ変換し、表示しています。

これにより、職務経歴の内容更新は `resume.md` ファイルの編集のみで行えるようになっています。

- **表示内容の原本:** [`resume.md`](./resume.md)
- **Web ページの骨格:** [`index.html`](./index.html)
- **スタイル定義:** [`style.css`](./style.css)

---

## 開発者向けメモ: ローカルでのプレビュー方法

開発・編集時にローカル環境で表示を確認するための手順です。

`index.html` ファイルを直接ブラウザで開いても、`resume.md` の読み込みがセキュリティ制限 (CORS) により失敗します。
以下のいずれかの方法でローカル HTTP サーバーを起動し、指定された URL にアクセスしてください。

### Python 3 を使う場合

```bash
cd <プロジェクトディレクトリ>
python3 -m http.server
```

ブラウザで `http://localhost:8000` を開きます。

### Node.js (live-server) を使う場合

`live-server` はファイルの変更を検知して自動でブラウザをリロードしてくれるため便利です。

```bash
cd <プロジェクトディレクトリ>
npx live-server
```

自動でブラウザが開くか、ターミナルに表示される URL (`http://127.0.0.1:8080` など) を開きます。
