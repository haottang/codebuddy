# Gin Demo

一个简单的 Gin Web 框架示例项目。

## 运行

```bash
go mod tidy
go run main.go
```

## 接口

- `GET /ping` - 返回 {"message": "pong"}
- `GET /hello?name=xxx` - 返回问候语
- `POST /data` - 接收 JSON 数据

## 测试

```bash
# ping
curl http://localhost:8080/ping

# hello
curl http://localhost:8080/hello?name=Auto

# POST
curl -X POST http://localhost:8080/data -H "Content-Type: application/json" -d '{"name":"test","value":123}'
```
