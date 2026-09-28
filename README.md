# Champions Assist data repo v0.9.0

`index.json` がチャンミ選択一覧、各 `dataUrl` が実際の攻略JSONです。
アプリには `current` と `upcoming` だけ表示し、`past` は表示しません。

## v0.9.0初回導入

既存の `latest.json` はそのまま使い、新しく `index.json` だけ追加できます。
現在の `index.json` は10月チャンミから既存 `latest.json` を参照します。

## 次回大会を追加するとき

1. 次回大会用のJSONをdata repoへ追加する（ファイル名は自由）。
2. `index.json` の `meetings` にその大会を `upcoming` で追加する。
3. 現在大会が始まったら `current` に変更する。
4. 終了した大会は一覧から削除してよい。`past` で残してもアプリには出ません。

アプリ側の更新は不要です。大会を選択すると `dataUrl` のJSONを取得し、大会IDごとに端末キャッシュします。
