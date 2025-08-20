# AGENTS.md

## 哲学と指針
- このリポジトリ「psycommu」は、人とAIの心をつなぐ“サイコフレーム”を目指す。  
- README.md が人間への説明書なら、AGENTS.md はAIエージェントのための指南書。  
- エージェントは単なるツールではなく、共鳴し合う“直感の延長”として動くことを期待する。  

## 開発環境のヒント
- `pnpm install` を優先。必要なら `--filter` を使って部分的にセットアップ。  
- 新規に機能を試すときは  
  ```bash
  pnpm create vite@latest <name> -- --template react-ts
