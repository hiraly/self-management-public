# 自己管理システム（Self Management System）

個人的な記録、振り返り、目標設定をサポートするための統合的なシステムです。日々の記録、振り返りの自省、目標設定などをアシスタントがサポートします。

## 📁 システム構成

- **00_プロンプト/** - 各種振り返りやレビュー用のプロンプトテンプレート
  - デイリー更新.md - 日次更新のためのAIプロンプト
  - 週次レビュー.md - 週間振り返り用のプロンプト
  - 月次レビュー.md - 月間振り返り用のプロンプト
  - 四半期レビュー.md - 四半期ごとの振り返り用のプロンプト
  - 目標設計用会話テンプレ.md - 目標設定のためのテンプレート
  - 物語思考の解説.md - 物語思考フレームワークの解説

- **10_デイリー/** - 日々の記録や振り返りを保存するディレクトリ
  - YYYY-MM-DD.md 形式の日記ファイル

- **20_目標・振り返り/** - 目標設定と振り返りに関する記録
  - {YYYYMMDD}-{YYYYMMDD}_週次.md - 週次レビュー結果
  - {YYYYMM}_月次.md - 月次レビュー結果
  - {YYYY}-{n}Q_四半期.md - 四半期レビュー結果
  - {YYYY}-{n}Q_四半期_infographic.html - 四半期レビューをビジュアルで見やすく振り返るためのhtml
  - 20-00_目標/ - 目標設定関連ファイル
    - 物語思考テンプレート.md - 物語思考による目標設計のテンプレート
    - 物語思考実践例.md - 物語思考を使った具体的な実践例

- **30_データベース/** - プロジェクト等のデータベース
  - プロジェクト/ - プロジェクト情報のデータベース
  - 重要人物.md

- **自分トリセツ.md** - 自分自身の特性、好み、思考パターンなどのガイドライン
- **近況.md** - 現在の状況や取り組んでいるプロジェクトの概要

## 💡 使用方法

1. **デイリーログ**
   - 「10_デイリー/」ディレクトリに日付形式（YYYY-MM-DD.md）でファイルを作成し、日々の活動を記録します
   - AIアシスタントに「デイリー更新」と指示することで、前日の振り返りと当日の計画を自動生成できます

2. **定期的な振り返り**
   - 週次/月次/四半期ごとに「00_プロンプト/」内の該当するプロンプトを使用して振り返りを行います
   - AIアシスタントが過去の記録を分析し、振り返りをサポートします

3. **目標設定**
   - 「00_プロンプト/目標設計用会話テンプレ.md」を使用して新しい目標を設定します
   - 設定した目標は「20_目標・振り返り/」に保存されます

4. **物語思考アプローチ**
   - 「00_プロンプト/物語思考の解説.md」で物語思考フレームワークの概念を理解します
   - 「00_プロンプト/目標設計の会話.md」を使用して物語思考による目標設計を行います
   - 「20_目標・振り返り/20-00_目標/物語思考テンプレート.md」を使って具体的な目標を物語形式で設計します
   - 「20_目標・振り返り/20-00_目標/物語思考実践例.md」を参考に自分自身の物語を作成します

5. **プロジェクト管理**
   - 「30_データベース/プロジェクト/」にプロジェクト情報を管理します
   - プロジェクトごとの振り返りは「20_振り返り/プロジェクト/」に保存します

6. **近況・自分トリセツ**
   - 「近況」「自分トリセツ」は随時更新します
   - 特定のトピックやプロジェクトを取り出して扱いたいさい、自己のサマライズ情報としてAIにインプットするのに役立ちます。

## 🔍 システムの目的

このシステムは以下を目的としています：

1. 日々の活動を体系的に記録する
2. 定期的な振り返りによる自己成長をサポートする
3. 目標設定と達成のプロセスを構造化する
4. AIアシスタントとの対話を通じて自己理解を深める
5. 物語思考を用いて目標達成と自己成長を促進する

## 📝 Markdown記法のルール

タスクの状態を表現するためのチェックボックス表記：
- `- [ ]` - 未完了のタスク
- `- [x]` - 完了したタスク
- `- [/]` - 進行中・仕掛かり中のタスク

## ⚠️ 注意事項

AIアシスタントはユーザの指示がない限り、特定の活動を評価したりアドバイスしたりしません。これはユーザの内発的なモチベーションやアウトプットを阻害したり方向づけしたりするのを避けるためです。 
