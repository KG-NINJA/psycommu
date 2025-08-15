# プロジェクト指示書（サイコーミュ方式：自動翻訳システム）

## 1. プロジェクト名
自動翻訳システム (Auto-Translator)

## 2. ゴール
- 音声またはテキストを入力すると即座に翻訳結果を得られる。
- 最初は Python + Whisper ライブラリでデモを完成させる。
- 将来的に whisper.cpp で高速化し、Bot化を目指す。

## 3. 作業の進め方
1. Python版 Whisper をインストールして動作確認
   ```bash
   pip install openai-whisper
