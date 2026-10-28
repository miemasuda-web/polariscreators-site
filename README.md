# polariscreators-site

polariscreators.com の小さなサイト（GitHub Pages）。

- `app-ads.txt`：AdMob の広告枠の持ち主を示すファイル。アプリ『未読』の AdMob の確認に使う。ドメインのいちばん上（`https://polariscreators.com/app-ads.txt`）で読める必要がある。
- `index.html`：『未読』の紹介とサポートへのリンク。

## ドメインのつなぎ方

1. ドメインの管理画面で、`polariscreators.com`（@）に GitHub Pages の A レコード4つを足す（MX などメールの設定には触れない）。
   `185.199.108.153` / `185.199.109.153` / `185.199.110.153` / `185.199.111.153`
2. このリポジトリの Settings → Pages → Custom domain に `polariscreators.com` を入れて保存し、Enforce HTTPS をオンにする。
3. App Store Connect のマーケティング URL を `https://polariscreators.com` にする（次のアップデートと一緒に）。
4. AdMob の「アプリの設定」で「アップデートを確認」を押す。
