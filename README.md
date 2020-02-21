## Docker Nginx

- 全てのパスに対して、jsonをレスポンスをします。
- 必ず200応答です。（全てのPATHを拾うようにしています）
- アクセスログは`log/access.log`に出力され、リクエストBodyも出力されます。

## Usage

```bash
docker-compose up

curl -X POST -H "Content-Type: application/json" \
-d '{"Name":"james", "Age":"100"}' \
http://127.0.0.1:8080/api/v1/users
```
