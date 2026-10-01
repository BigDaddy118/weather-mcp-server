# Weather MCP Server

真实天气查询 MCP 服务器（**Streamable HTTP**），可填入 Smithery 的 MCP Server URL。

## 本地运行

```bash
pip install -r requirements.txt
python server.py
# 默认: http://0.0.0.0:8081/mcp
```

## Smithery 表单怎么填

1. **Namespace / Server ID**: `BigDaddy118` / `weather-mcp-server`
2. **MCP Server URL**: 填部署后的公网地址，例如 `https://你的域名/mcp`（不能填 GitHub 仓库地址）

## Docker

```bash
docker build -t weather-mcp-server .
docker run -p 8081:8081 weather-mcp-server
```

## 工具

- `get_weather(city)`
- `list_supported_cities()`
- `get_server_info()`

## 许可证

MIT
