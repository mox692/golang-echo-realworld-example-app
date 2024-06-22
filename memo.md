起動

```sh
go run main.go
```

requestを投げる
```sh
# docs.goから適当にエンドポイントを選ぶ
repeat 10000 sleep 0.1 &&  curl 'http://127.0.0.1:8585/api/articles'
```

traceを分析
```bash
go tool trace trace.out
```
