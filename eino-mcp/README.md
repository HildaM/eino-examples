# Eino MCP

基于 Eino 框架开发的 MCP (Message Control Protocol) 示例项目。

A MCP (Message Control Protocol) example project built on Eino framework.

## 项目简介 | Introduction

本项目展示了如何使用 Eino 框架实现 MCP 协议，包括：
- MCP 代理实现
- 配置管理
- 工具集成
- 协议扩展示例
- RAG (Retrieval Augmented Generation) 功能集成

This project demonstrates how to implement MCP protocol using Eino framework, including:
- MCP agent implementation
- Configuration management
- Tool integration
- Protocol extension examples
- RAG (Retrieval Augmented Generation) integration

## 项目结构 | Project Structure

```
eino-mcp/
├── agent/          # MCP agent implementation
├── conf/           # Configuration management
├── tools/          # Tool implementations
├── rag/            # RAG functionality (integrated from github.com/HildaM/eino-rag)
├── main.go         # Entry point
├── config.yaml     # Configuration file
└── go.mod          # Go module definition
```

## 快速开始 | Quick Start

### 安装依赖 | Install Dependencies

```bash
go mod tidy
```

### 配置设置 | Configuration

1. 复制配置文件示例：
   ```bash
   cp config.yaml.example config.yaml
   ```

2. 编辑 `config.yaml` 文件，配置必要的参数：
   ```yaml
   mcp:
     host: "localhost"
     port: 8080
     # 其他配置项...
   
   rag:
     # RAG相关配置
     embedding_model: "text-embedding-ada-002"
     vector_store: "local"
   ```

### 运行项目 | Run Project

```bash
go run main.go
```

## 功能特性 | Features

- MCP 协议实现
- 配置热加载
- 工具集成支持
- 代理服务
- RAG 知识库检索增强生成

## 外部依赖 | External Dependencies

本项目集成了以下外部仓库：
- [HildaM/eino-rag](https://github.com/HildaM/eino-rag) - Eino框架的RAG实现

## 开发计划 | Development Plan

- [ ] 完善错误处理机制
- [ ] 添加更多工具支持
- [ ] 优化配置管理
- [ ] 添加单元测试
- [ ] 完善RAG功能集成

## 贡献指南 | Contributing

欢迎提交 Pull Request 或 Issue 来完善项目。

Feel free to submit Pull Requests or Issues to improve the project. 