# soneki-release

部門損益 可視化（DeptProfitVis）の GitHub Pages 配信リポジトリ。開発は ../soneki-gas。
https://acoop-ai.github.io/soneki-release/

## 🔴 このリポは「公開」＝実データを置かない（絶対規則）

GitHub Pages で誰でも閲覧できる。**業務の実データ（実店舗名・実損益）を置いてはならない。**

- `index.html` … アプリのガワのみ。実データは持たない
- `demo/` … **作り物のモックだけ**（架空エリア「デモ東/西エリア」・架空店名「サンプル店○○」）。
  見せ方確認用。生成器＝`scratchpad/gen_soneki_demo_mock.py` 相当（実データ変換器を流用しない）
- **実データは GAS＋4ドメインOAuth 経由のみ**で表示する（Drive の outbox を認証済みユーザーだけが読む）

> 経緯: 2026-07-26、GAS接続前のプレビュー目的で `demo/` に実データ（5エリア55店・15ヶ月）を投入し公開してしまう事故が発生。
> 実データを撤去しモックへ置換、履歴も clean 化して封じ込め済み。同じ理由で「一時的だから」を認めない。
