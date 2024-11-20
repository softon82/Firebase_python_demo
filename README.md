# Firebase Functions プロジェクト

## 概要
Firebaseを使用したPythonバックエンドサービスのサンプルです。
HTTPリクエストとFirestoreトリガーを使用して、メッセージの保存と大文字変換機能を提供するプログラムのデモを実施しました。

## 機能
1. **メッセージ追加 API** (`addmessage`):
   - HTTPリクエストでテキストメッセージを受け取り、Firestoreに保存
   - クエリパラメータ `text` でメッセージを送信

2. **自動大文字変換** (`makeuppercase`):
   - Firestoreの`messages`コレクションに新規ドキュメントが作成されると自動実行
   - 元のテキスト（`original`フィールド）を大文字に変換し、`uppercase`フィールドとして保存

## 参照
- [Firebase Functions demo](https://firebase.google.com/docs/functions/get-started)
- [Firebase CLI](https://firebase.google.com/docs/cli?hl=ja#install-cli-mac-linux)
