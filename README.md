# polariscreators-site

polariscreators.com の小さなサイト（GitHub Pages）。

- `app-ads.txt`：AdMob の広告枠の持ち主を示すファイル。アプリ『未読』の AdMob の確認に使う。ドメインのいちばん上（`https://polariscreators.com/app-ads.txt`）で読める必要がある。
- `index.html`：『未読』の紹介とサポートへのリンク。

## 注意：polariscreators.com にはすでに会社のサイトがある

2026-10-28 に確認したところ、`https://polariscreators.com` には「Polaris Creators」のサイト（AWS 上、DNS は Cloudflare）がすでにある。
**ドメインをこのリポジトリ（GitHub Pages）に向けると、そのサイトが置き換わってしまうので、向けないこと。**

app-ads.txt は、次のどちらかで `https://polariscreators.com/app-ads.txt` から読めるようにする。

1. 会社のサイトの管理者に、サイトのいちばん上に `app-ads.txt`（このリポジトリと同じ1行）を置いてもらう（いちばん簡単）。
2. Cloudflare で `polariscreators.com/app-ads.txt` だけを返す設定（Workers のルートなど）を足す。サーバーには触れない。

そのあと、App Store Connect のマーケティング URL を `https://polariscreators.com` にし（次のアップデートと一緒に）、AdMob の「アプリの設定」で「アップデートを確認」を押す。

このリポジトリの GitHub Pages（`https://miemasuda-web.github.io/polariscreators-site/`）は、app-ads.txt の中身の控えと『未読』の紹介ページとして残しておく。
