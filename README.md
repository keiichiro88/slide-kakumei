# スライド革命 - Google Slides Generator

Google Apps Script (GAS) を使用してGoogle Slidesを自動生成するツールです。

## 概要

このプロジェクトは、テキストやデータからプロフェッショナルなGoogle Slidesプレゼンテーションを自動生成するためのGoogle Apps Scriptアプリケーションです。

## ファイル構成

```
GAS/
├── Code.gs      - メインのGASコード（サーバーサイドロジック）
├── gs.code      - GASコードのバックアップ
├── index.html   - WebアプリのフロントエンドUI
└── Gem.plompt   - Geminiカスタム指示（JSONデータ生成用プロンプト）
```

## 機能

- 🎨 カラーユーティリティ（HEX/RGB/HSL変換）
- 📊 20種類以上のスライドパターン対応
- 🎯 カスタマイズ可能なスライドテーマ
- 📱 レスポンシブなWebインターフェース
- 🤖 Gemini AIによるスライド構成自動生成

## 使用方法（ワークフロー）

```
┌─────────────────────────────────────────────────────────────────┐
│  1. GASアプリで「ジェミニを開く」ボタンをクリック                    │
│                    ↓                                            │
│  2. Gemini（カスタムジェム）が開く                                 │
│     - Gem.plompt のカスタム指示が設定済み                         │
│     - スライドの内容を会話形式で伝える                             │
│                    ↓                                            │
│  3. GeminiがslideData JSONを生成                                │
│                    ↓                                            │
│  4. 生成されたJSONをコピー                                       │
│                    ↓                                            │
│  5. GASアプリの「スライド構成データ入力」欄にペースト               │
│                    ↓                                            │
│  6. スライド生成ボタンをクリック → Google Slides完成！             │
└─────────────────────────────────────────────────────────────────┘
```

## 対応スライドパターン

| カテゴリ | パターン |
|---------|---------|
| 基本 | title, section, closing, content |
| リスト | agenda, cards, headerCards, bulletCards |
| 比較 | compare, statsCompare, barCompare |
| プロセス | process, processList, timeline, flowChart |
| 図解 | pyramid, triangle, stepUp, cycle, diagram |
| データ | table, kpi, progress |
| その他 | quote, faq, imageText |

## セットアップ

1. [Google Apps Script](https://script.google.com/) にアクセス
2. 新しいプロジェクトを作成
3. `Code.gs` の内容をスクリプトエディタにコピー
4. `index.html` をHTMLファイルとして追加
5. デプロイしてWebアプリとして公開
6. Geminiでカスタムジェムを作成し、`Gem.plompt` の内容をカスタム指示に設定

## 技術スタック

- Google Apps Script
- HTML/CSS/JavaScript
- Google Slides API
- PDF.js（PDFプレビュー用）
- Google Gemini（AI構成生成）

## ライセンス

MIT License

## 作者

Hayashi Keiichiro
