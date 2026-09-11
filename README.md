# Ryosei Morisawa

大学院では機械学習を用いた医用画像解析を研究しています。
チーム開発では、バックエンドを中心にプロダクトの設計・実装に取り組んでいます。

## 研究

脳MRIを対象に、現在の画像から将来の脳の変化を予測・生成する深層学習モデルの研究に取り組んでいます。
加齢や認知症に伴う脳の経年変化に着目し、脳領域の体積や形状の変化を捉えることを目指しています。

## 最近の開発（チーム）

### [オキタ！（Okita!）](https://github.com/takefussa/wake-hack) — 明日の朝を、誰かの声で。

誰かが録音した「おはよう」をアラームとして届け、起きたらお礼のボイスメッセージを返せるアプリです。
学生向けハッカソン [Tornado2026](https://2026.tornado-official.jp/) で、**PM1人・デザイナー1人・エンジニア4人の計6人**で開発しました。

🏆 **Tornado2026 大阪拠点にて最優秀賞と企業賞を受賞しました！**

**担当：エンジニア／バックエンドリーダー**

チームで制作したプロダクトのうち、用件定義及び、バックエンド全般と、音声の送受信から端末のアラームにつなぐ処理を担当しました。

- **データ基盤**：Supabaseの認証・DB・Storageを使った、プロフィール・朝リクエスト・音声・お礼などのデータ連携。
- **音声配送**：録音ファイルの保存、送信先と朝リクエストへの紐付け、受信側での取得・受け取り状態の管理。
- **アラーム連携**：Personal VoiceをAlarmKitの音声として準備・登録し、未到着時にはCommunity Voiceや標準音を使う処理。
- **統合・検証**：フロントエンドとの接続、不具合の原因調査、iPhone・iPadでの動作確認。

特に注力したのは、**録音された音声を保存・管理し、適切なユーザーへ届け、指定時刻にアラームとして再生するまでの一連のバックエンド設計・実装**です。

使用技術：TypeScript / Supabase（Auth・PostgreSQL・Storage）/ Expo・React Native / Swift・AlarmKit

→ [チームのリポジトリ・プロダクト紹介を見る](https://github.com/takefussa/wake-hack)

## 過去の個人開発

### 大学3年次PBL タスク管理Webアプリ

研究・学習などのタスクをプロジェクトごとに整理するアプリを、フロントエンドとバックエンドに分けて開発しました。
タスクの追加・削除、クリックによる **Todo → In Progress → Done** の更新、プロジェクト別の進捗一覧を実装しています。

- **フロントエンド**：Next.js / React / TypeScript / Chakra UI。画面と操作を実装し、メイン画面のデータをSupabaseへ保存。
- **バックエンド**：Python / FastAPI / SQLAlchemy / PostgreSQL。プロジェクト・タスクの作成・取得・更新・削除を行うREST APIを実装。

[フロントエンド](https://github.com/takefussa/take-project) · [バックエンド](https://github.com/takefussa/FastAPI)

<details>
<summary>タスク管理画面を見る</summary>

![プロジェクトごとのタスクをTodo・In Progress・Doneに分けて管理する画面](https://raw.githubusercontent.com/takefussa/take-project/main/docs/images/task-board.png)

</details>
