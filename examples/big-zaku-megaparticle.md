# プロジェクト指示書（サイコーミュ方式：ビッグザク・メガ粒子砲）

## 1. プロジェクト名
ビッグザク・メガ粒子砲 (Big Zaku Mega Particle Cannon)

## 2. ゴール
- 情報を効率よく多方面へ一斉拡散する自動ワークフローを構築する。
- すべての拡散文面に BuyMeACoffee（BMC）リンクを自然に織り込む。
- 投稿→計測→最適化を継続し、拡散率とCV（支援率）を上げる。

## 3. 作業の進め方
1. **投稿ペイロード定義**（YAML/JSON）
   - `title` / `summary` / `image` / `tags` / `cta` を統一
   - `bmc`: `https://buymeacoffee.com/kgninja?utm_source={platform}&utm_medium=social&utm_campaign=psycommu`
2. **テンプレート生成（Markdown→各プラットフォーム）**
   - X（140字）：短文＋#KGNINJA＋短縮（必要なら）＋BMC
   - Telegra.ph/Blog：長文＋画像＋BMCを上部と末尾に
   - Discord：要点3行＋BMC＋画像URL
3. **自動発射ワークフロー**
   - a) GitHub Actions（`on: workflow_dispatch`）で一斉投稿
   - b) または n8n フロー（Cron/Manual→各SNSノード）
4. **ログ＆計測**
   - 送信レスポンスを `logs/` に保存
   - `utm_source` でクリック計測（BMC側・アナリティクス）
5. **最適化**
   - クリック率/支援CVを週次で比較→文面テンプレAB

## 4. 出力テンプレート
### 4.1 X（短文）
