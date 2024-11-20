# Firebase Functions プロジェクト

## 概要
このリポジトリはFirebase Functionsを使用したPythonバックエンドサービスです。HTTPリクエストとFirestoreトリガーを使用して、メッセージの保存と大文字変換機能を提供します。

## 機能
1. **メッセージ追加 API** (`addmessage`):
   - HTTPリクエストでテキストメッセージを受け取り、Firestoreに保存
   - クエリパラメータ `text` でメッセージを送信

2. **自動大文字変換** (`makeuppercase`):
   - Firestoreの`messages`コレクションに新規ドキュメントが作成されると自動実行
   - 元のテキスト（`original`フィールド）を大文字に変換し、`uppercase`フィールドとして保存

## 必要条件
- Python 3.7以上
- Firebase CLI
- Firebase プロジェクト

## 依存関係