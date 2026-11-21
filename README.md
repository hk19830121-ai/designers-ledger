# Designer's Ledger — サイト本体

海外アフィリエイト企画のサイト。手順書は ~/workspace/affiliate-drafts/00-site-setup-guide-free.md。

- 構築：Hugo（バイナリは ~/workspace/tools/hugo/hugo、v0.170.1 extended）
- ビルド：`cd ~/workspace/designers-ledger && ~/workspace/tools/hugo/hugo` → public/ に出力
- 公開先：Cloudflare Workers（https://designers-ledger.akumu-channel-info.workers.dev、無料）。GitHubリポジトリ連携で push のたびに自動デプロイ（Build command なし／Deploy command `npx wrangler deploy`）
- 更新手順：ソースを編集 → `~/workspace/tools/hugo/hugo` でビルド → public/ の変化も含めて commit → push（public/ は .gitignore に入れない。Cloudflare側ビルドでは public が残らなかったための方式）
- 状態（2026-11-21）：**公開中**。骨格＋固定ページ（About / Affiliate Disclosure / Privacy）が表示されることを確認済み。記事1本目（client-wont-pay）は draft: true で格納のみ。ツール3社の公式条件は確認済みで本文に反映済み。残りは Reddit引用の現物確認とアフィリエイトプログラム確認が済んでから draft を外して公開
- Contact ページは draft のまま（連絡先が決まったら公開）
