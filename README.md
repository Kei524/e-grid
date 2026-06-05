# イーグリッド コンサル基礎研修

新人コンサルタント向けの基礎研修コンテンツ（スライド資料）です。
Markdown ベースの [Marp](https://marp.app/) で作成しており、GitHub 上での編集・レビュー、PDF / PPTX / HTML への出力が可能です。

## 対象者

- 新卒・中途で入社したばかりの新人コンサルタント全般
- コンサルティングの基礎スキルを体系的に学び直したいメンバー

## ゴール（研修修了時の状態）

1. コンサルタントとしての役割・心構えを自分の言葉で説明できる
2. ロジカルシンキングの基本（MECE・ピラミッド構造・ロジックツリー）を使える
3. 問題解決の基本プロセスに沿って、課題を構造化し打ち手を導ける
4. 仮説思考でリサーチ・検証を効率的に進められる
5. ヒアリング・資料作成・プレゼンの型を理解し、実務で再現できる
6. プロジェクトの進め方（PM の基礎）をイメージできる

## カリキュラム構成

| No. | モジュール | ファイル | 目安時間 |
| --- | --- | --- | --- |
| 00 | 研修オリエンテーション | [slides/00_orientation.md](slides/00_orientation.md) | 30分 |
| 01 | コンサルタントとは／心構え | [slides/01_consultant_mindset.md](slides/01_consultant_mindset.md) | 60分 |
| 02 | ロジカルシンキング基礎 | [slides/02_logical_thinking.md](slides/02_logical_thinking.md) | 90分 |
| 03 | 問題解決の基本プロセス | [slides/03_problem_solving.md](slides/03_problem_solving.md) | 90分 |
| 04 | 仮説思考・リサーチ | [slides/04_hypothesis_research.md](slides/04_hypothesis_research.md) | 60分 |
| 05 | ヒアリング・コミュニケーション | [slides/05_communication.md](slides/05_communication.md) | 60分 |
| 06 | ドキュメンテーション（資料作成） | [slides/06_documentation.md](slides/06_documentation.md) | 90分 |
| 07 | プレゼンテーション | [slides/07_presentation.md](slides/07_presentation.md) | 60分 |
| 08 | プロジェクトマネジメント基礎 | [slides/08_project_management.md](slides/08_project_management.md) | 60分 |

> 各モジュールは独立して実施できます。1日完結ではなく、複数回に分けての実施を推奨します。

## スライドの見方・出力方法

### 1. VS Code で編集・プレビュー

1. VS Code 拡張機能「**Marp for VS Code**」をインストール
2. `slides/` 以下の `.md` を開くと、右上のプレビューアイコンからスライド表示できます

### 2. CLI で PDF / PPTX / HTML に変換

[Marp CLI](https://github.com/marp-team/marp-cli) を使用します。

```bash
# Marp CLI のインストール（要 Node.js）
npm install -g @marp-team/marp-cli

# 単一ファイルを PDF に変換
marp slides/02_logical_thinking.md --pdf --theme themes/egrid.css

# PPTX（PowerPoint）に変換
marp slides/02_logical_thinking.md --pptx --theme themes/egrid.css

# slides/ 配下をまとめて HTML に変換
marp slides/ --theme themes/egrid.css
```

## ディレクトリ構成

```
.
├── README.md                 # 本ファイル
├── slides/                   # 各モジュールのスライド（Marp Markdown）
│   ├── 00_orientation.md
│   ├── 01_consultant_mindset.md
│   ├── 02_logical_thinking.md
│   ├── 03_problem_solving.md
│   ├── 04_hypothesis_research.md
│   ├── 05_communication.md
│   ├── 06_documentation.md
│   ├── 07_presentation.md
│   └── 08_project_management.md
└── themes/
    └── egrid.css             # スライド共通テーマ
```

## 編集ガイドライン

- 1スライド＝1メッセージを基本とする（情報を詰め込みすぎない）
- 具体例・演習（💡 / ✏️ で表記）を各モジュールに必ず入れる
- 専門用語は初出時に必ず補足する
- 図解できる箇所は文章ではなく図・表で表現する

## ライセンス／取り扱い

社内研修用コンテンツです。社外への共有時は内容の取り扱いに注意してください。
