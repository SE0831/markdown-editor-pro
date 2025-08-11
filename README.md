# MarkdownPro

## 📝 概要

リアルタイムプレビュー機能を備えた高機能マークダウンエディタです。直感的なUIと豊富な編集機能により、ドキュメント作成の生産性を大幅に向上させます。

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ 主な機能

### エディタ機能
- **📝 リアルタイムプレビュー** - 入力と同時に右側にプレビュー表示
- **🎨 シンタックスハイライト** - Prism.jsによるコードの色分け表示
- **⌨️ ショートカット対応** - Ctrl+B（太字）、Ctrl+I（斜体）など
- **💾 自動保存** - LocalStorageによる自動バックアップ

### 編集支援機能
- **🔧 ツールバー** - ワンクリックでマークダウン記法を挿入
- **📋 テンプレート** - README、ブログ、議事録など6種類のテンプレート
- **📊 ステータスバー** - 文字数、行数、単語数をリアルタイム表示
- **🌙 ダークモード** - 目に優しい暗色テーマへの切り替え

### ファイル操作
- **📂 ファイル読み込み** - .md、.txtファイルのインポート
- **💾 マークダウン保存** - 編集内容を.mdファイルとして保存
- **📄 HTML出力** - スタイル付きHTMLファイルとしてエクスポート
- **🔄 新規作成** - ワンクリックで新規ドキュメント作成

## 🛠️ 使用技術

| カテゴリ | 技術 | 用途 |
|---------|------|------|
| **パーサー** | Marked.js | マークダウンをHTMLに変換 |
| **ハイライト** | Prism.js | コードのシンタックスハイライト |
| **アイコン** | Font Awesome 6 | UIアイコン表示 |
| **フォント** | JetBrains Mono | コードエディタ用等幅フォント |
| **フォント** | Inter | UI用サンセリフフォント |
| **ストレージ** | LocalStorage | 自動保存機能 |

## 🚀 デモ

[🔗 ライブデモはこちら](https://se0831.github.io/markdown-editor-pro/)

## 📦 インストール & 使用方法

### オンライン版
1. 上記のデモリンクにアクセスするだけですぐに使用開始できます

### ローカル版
```bash
# リポジトリをクローン
git clone https://github.com/SE0831/markdown-editor-pro.git

# ディレクトリに移動
cd markdown-editor-pro

# ブラウザで開く（Macの場合）
open index.html

# ブラウザで開く（Windowsの場合）
start index.html

# またはローカルサーバーで実行
python -m http.server 8000
# http://localhost:8000 にアクセス
```

## 📝 基本的な使い方

### 1. テキスト編集
- 左側のエディタエリアにマークダウンを入力
- 右側のプレビューエリアでリアルタイムに結果を確認

### 2. ツールバーの活用
- **書式設定**: 太字、斜体、取り消し線
- **見出し**: H1、H2、H3の挿入
- **リスト**: 箇条書き、番号付き、チェックリスト
- **要素挿入**: リンク、画像、コード、引用、テーブル

### 3. キーボードショートカット
| ショートカット | 機能 |
|---------------|------|
| `Ctrl/Cmd + B` | 太字 |
| `Ctrl/Cmd + I` | 斜体 |
| `Ctrl/Cmd + K` | リンク挿入 |
| `Ctrl/Cmd + S` | ファイル保存 |
| `Ctrl/Cmd + O` | ファイルを開く |
| `Ctrl/Cmd + N` | 新規作成 |

## 📋 利用可能なテンプレート

1. **README** - GitHubプロジェクト用
2. **ブログ記事** - ブログ投稿用フォーマット
3. **ドキュメント** - 技術文書用
4. **議事録** - 会議記録用
5. **プロジェクト計画** - プロジェクト管理用
6. **チュートリアル** - 学習コンテンツ用

## 🎨 マークダウン記法サポート

### 基本記法
- 見出し（H1〜H6）
- 太字、斜体、取り消し線
- 箇条書き、番号付きリスト
- チェックリスト
- リンク、画像
- インラインコード、コードブロック
- 引用
- 水平線
- テーブル

### 拡張記法（GFM）
- テーブル
- タスクリスト
- 自動リンク
- 取り消し線

## ⚙️ カスタマイズ

### カラーテーマの変更
CSSの`:root`セクションで色を調整できます：
```css
:root {
    --accent: #007acc;  /* メインカラー */
    --bg-primary: #1e1e1e;  /* 背景色 */
    /* その他のカラー設定 */
}
```

### エディタフォントの変更
```css
#editor {
    font-family: 'お好みのフォント', monospace;
}
```

## 📂 プロジェクト構成

```
markdown-editor-pro/
├── index.html      # アプリケーション本体（HTML/CSS/JS統合）
├── README.md       # このファイル
└── LICENSE         # MITライセンス
```

## 🔄 今後の機能追加予定

- [ ] **Markdown拡張記法対応**
  - 数式（KaTeX/MathJax）
  - Mermaidダイアグラム
  - 絵文字ショートコード
- [ ] **エディタ機能強化**
  - 検索・置換機能
  - 複数ファイルのタブ管理
  - Vimキーバインド対応
- [ ] **同期・共有機能**
  - クラウド同期（Google Drive、Dropbox）
  - 共有リンク生成
  - コラボレーション編集
- [ ] **エクスポート拡張**
  - PDF出力
  - Word文書（.docx）出力
  - プレゼンテーション変換
- [ ] **UI/UX改善**
  - カスタムテーマ作成機能
  - プレビューのみモード
  - 全画面編集モード
  - モバイル対応の改善

## 🤝 コントリビューション

プルリクエストは大歓迎です！大きな変更の場合は、まずissueを開いて変更内容を議論してください。

1. このリポジトリをフォーク
2. フィーチャーブランチを作成 (`git checkout -b feature/AmazingFeature`)
3. 変更をコミット (`git commit -m 'Add some AmazingFeature'`)
4. ブランチにプッシュ (`git push origin feature/AmazingFeature`)
5. プルリクエストを作成

## 📄 ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE)ファイルをご覧ください。

## 👤 作者

**SE0831**

- GitHub: [@SE0831](https://github.com/SE0831)
- ポートフォリオ: [その他のプロジェクト](https://github.com/SE0831?tab=repositories)

## 🙏 謝辞

- [Marked.js](https://marked.js.org/) - 高速で軽量なマークダウンパーサー
- [Prism.js](https://prismjs.com/) - 美しいシンタックスハイライト
- [Font Awesome](https://fontawesome.com/) - アイコンセット
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) - プログラミング用フォント

## 🔗 関連プロジェクト

他のポートフォリオ作品もご覧ください：

- [📊 Sales Analytics Dashboard](https://github.com/SE0831/sales-analytics-dashboard)
- [🌤️ Weather Dashboard](https://github.com/SE0831/weather-dashboard)
- [💰 Expense Tracker App](https://github.com/SE0831/expense-tracker-app)
- [📋 Task Management App](https://github.com/SE0831/task-management-app)

---

⭐ このプロジェクトが役に立ったら、スターをお願いします！

*最終更新: 2024年8月*
