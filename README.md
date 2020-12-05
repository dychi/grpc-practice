# WEB + DB PRESSのgRPC速習

## protoファイルからコードの生成
.protoファイルに定義したメッセージやサービスからGo用のサーバーインターフェースとRPCを実行するためのクライアントプログラムであるスタブのコードを生成する
```
protoc --proto_path ./echo/proto --go-grpc_out=./echo/proto/ ./echo/proto/echo.proto
```
### コマンドオプションについて
--proto_path: コンパイルする.protoファイルを検索するディレクトリの指定
--go-grpc_out: GoのgRPCのコードを出力するディレクトリ指定

