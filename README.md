# Designer's Ledger — サイト本体

海外アフィリエイト企画のサイト。手順書は ~/workspace/affiliate-drafts/00-site-setup-guide-free.md。

- 構築：Hugo（バイナリは ~/workspace/tools/hugo/hugo、v0.170.1 extended）
- ビルド：`cd ~/workspace/designers-ledger && ~/workspace/tools/hugo/hugo` → public/ に出力
- 公開先：Cloudflare Pages（designersledger.pages.dev、無料）。デプロイはヒロのCloudflareアカウント作成後に接続
- 状態（2026-11-21）：骨格＋固定ページ（About / Affiliate Disclosure / Privacy）完成。記事1本目（client-wont-pay）は draft: true で格納のみ。公開は裏取り（ツール3社の公式条件確認・Reddit引用現物確認・アフィリプログラム承認）が済んでから draft を外す
- Contact ページは draft のまま（連絡先が決まったら公開）
