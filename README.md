# test-esa-mcp

esa MCP サーバーの調査・検証用リポジトリ。

## 概要

[esa.io](https://esa.io) 公式の MCP サーバー ([esaio/esa-mcp-server](https://github.com/esaio/esa-mcp-server)) を VS Code + GitHub Copilot で利用するための設定をまとめています。

## 内容

- `.vscode/mcp.json` — VS Code 用の MCP サーバー設定（Docker版）
- `.github/copilot-instructions.md` — GitHub Copilot 向けの指示設定

## セットアップ

1. [esa の個人アクセストークン](https://docs.esa.io/posts/102) を発行する（PAT v2 推奨、read スコープのみ）
2. `.mcp-esa.env` を作成し、トークンを設定する

```
ESA_ACCESS_TOKEN=your_token_here
LANG=ja
```

3. VS Code で `.vscode/mcp.json` を開き、「起動」ボタンからサーバーを起動する
