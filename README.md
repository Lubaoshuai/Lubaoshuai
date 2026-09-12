# 你好，我是 Lubaoshuai 👋

**Java 后端 & AI Agent 开发 | Java Backend & AI Agent Engineering**

- 🔭 专注 **Java 企业级开发**与 **LLM Agent 工程化**：Spring / Spring AI / LangChain4j / MCP，兼写 Python、TypeScript
- 🌱 深入研究 Agent 编排、工具调用（Tool Calling）、RAG 与结构化输出的可靠性
- 📫 活跃在各大 AI 基建开源仓库：`langchain4j` · `spring-projects` · `langchain-ai` · `openclaw` · `modelcontextprotocol` · `google`

---

## 🚀 开源贡献 / Open Source Contributions

> 横跨 **10+ 个 AI 基建仓库**、**20+ 个在途 PR**；每个贡献都是：根因分析 → 最小改动 → 正反例单测 → 全量回归验证

### ✅ 已合并 / Merged

| 仓库 | PR | 说明 |
|------|----|------|
| ![Java](https://img.shields.io/badge/Java-007396?logo=openjdk&logoColor=white&label=%20) [langchain4j](https://github.com/langchain4j/langchain4j) ★13k | [#6243](https://github.com/langchain4j/langchain4j/pull/6243) | 修复 Agent Supervisor 参数描述丢失继承字段，让子 Agent 能力被 LLM 正确感知 |

### 🔍 In Review（CI 全绿，排队等 review）

| 仓库 | 代表 PR | 说明 |
|------|---------|------|
| [Spring AI](https://github.com/spring-projects/spring-ai) ★8k+ | [#6969](https://github.com/spring-projects/spring-ai/pull/6969) | 修复 Bedrock Converse 工具调用参数经 `Document.toString()` 序列化产生非法 JSON、工具执行 500 的问题，新增逆向 Document 转换器 + 回归测试 |
| [OpenClaw](https://github.com/openclaw/openclaw) ★389k | [#145242](https://github.com/openclaw/openclaw/pull/145242) | 修复心跳"设计内跳过"被记账为 failed：`tasks list --status failed` 每天误报 ~48 条 + 误触发失败告警 |
| [LangChain4j](https://github.com/langchain4j/langchain4j) | [#6373](https://github.com/langchain4j/langchain4j/pull/6373)–[#6378](https://github.com/langchain4j/langchain4j/pull/6378)、[#6220](https://github.com/langchain4j/langchain4j/pull/6220)–[#6225](https://github.com/langchain4j/langchain4j/pull/6225)、[#6293](https://github.com/langchain4j/langchain4j/pull/6293) | 图片 detailLevel 丢失、JSON Schema 继承字段/`@JsonIgnore`、Anthropic cache_control 去重、GPT-5 计数器、Infinispan Float 字面量、Kotlin pathMatcher、 refusal 流式透传、ExpandingQueryTransformer 上限、User-Agent 统一…… |
| [MCP Java SDK](https://github.com/modelcontextprotocol/java-sdk) | [#1132](https://github.com/modelcontextprotocol/java-sdk/pull/1132) | 修复 Streamable HTTP 会话在 SSE 写失败时被误丢弃的问题，保持会话存活 |
| [Google ADK Java](https://github.com/google/adk-java) | [#1505](https://github.com/google/adk-java/pull/1505) | 修复 Spring AI 自动配置加载顺序 |
| [LangChainJS](https://github.com/langchain-ai/langchainjs) ★15k | [#11613](https://github.com/langchain-ai/langchainjs/pull/11613) | 修复多模态消息 tracing 只转换首个 media block 的缺陷 |
| [Spring AI Alibaba](https://github.com/spring-ai-alibaba/spring-ai-extensions) | [#300](https://github.com/spring-ai-alibaba/spring-ai-extensions/pull/300) | AnalyticDB 向量库输出原生 jsonb 过滤语法替代 jsonpath |

<details>
<summary>📊 完整在途清单（点击展开）</summary>

| 仓库 | PR |
|------|-----|
| langchain4j/langchain4j | #6373 #6374 #6375 #6376 #6377 #6378 #6293 #6225 #6222 #6221 #6220 |
| spring-projects/spring-ai | #6969 #6956 |
| openclaw/openclaw | #145242 #144222 |
| langchain-ai/langgraph | [#8898](https://github.com/langchain-ai/langgraph/pull/8898)（等 issue 认领后自动重开） |
| modelcontextprotocol/java-sdk | #1132 |
| google/adk-java | #1505 |
| langchain-ai/langchainjs | #11613 |
| spring-ai-alibaba/spring-ai-extensions | #300 |
| langchain4j/langchain4j-spring | [#212](https://github.com/langchain4j/langchain4j-spring/pull/212) |

</details>

---

## 🧰 技术栈 / Tech Stack

![Java](https://img.shields.io/badge/Java-17-007396?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=springboot&logoColor=white)
![Spring AI](https://img.shields.io/badge/Spring_AI-6DB33F?logo=spring&logoColor=white)
![LangChain4j](https://img.shields.io/badge/LangChain4j-1C6EBC?style=flat)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat)
![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)

**Agent 方向**：Tool Calling · RAG · Guardrails · Streaming · Structured Output · Multi-Agent Orchestration · MCP

---

## 📦 自研项目 / Projects

- **[dsh-notify](https://github.com/Lubaoshuai/dsh-notify)** — DeepSeek Harness 通知插件：agent 可调用的 `notify_send` 工具 + 定时提醒外发（Telegram / Slack / Discord / 飞书 / 钉钉 / Bark / ntfy / webhook），TypeScript
