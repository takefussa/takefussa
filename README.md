# takefussa

チーム開発では、バックエンドを中心に、ユーザーに届く体験を支える仕組みづくりに取り組んでいます。

## 最近の開発（チーム）

### [オキタ！（Okita!）](https://github.com/takefussa/wake-hack) — 明日の朝を、誰かの声で。

誰かが録音した「おはよう」をアラームとして届け、起きたらお礼のボイスメッセージを返せるアプリです。
学生向けハッカソン [Tornado2026](https://2026.tornado-official.jp/) で、**PM1人・デザイナー1人・エンジニア4人の計6人**で開発しました。

**担当：エンジニア／バックエンドリーダー**

チームで制作したプロダクトのうち、バックエンド全般と、音声の送受信から端末のアラームにつなぐ処理を担当しました。

- **データ基盤**：Supabaseの認証・DB・Storageを使った、プロフィール・朝リクエスト・音声・お礼などのデータ連携。
- **音声配送**：録音ファイルの保存、送信先と朝リクエストへの紐付け、受信側での取得・受け取り状態の管理。
- **アラーム連携**：Personal VoiceをAlarmKitの音声として準備・登録し、未到着時にはCommunity Voiceや標準音を使う処理。
- **統合・検証**：フロントエンドとの接続、不具合の原因調査、iPhone・iPadでの動作確認。

特に注力したのは、**録音を保存するだけでなく、相手の端末に届け、指定時刻のアラームとして鳴らすまでの流れをつなぐこと**です。

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
