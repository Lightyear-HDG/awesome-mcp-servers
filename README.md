# Awesome MCP Servers ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

A curated list of awesome Model Context Protocol (MCP) servers. MCP is an open protocol that enables AI models to securely interact with local and remote resources through standardized server implementations. This list focuses on production-ready and experimental MCP servers that extend AI capabilities through file access, database connections, API integrations, and other contextual services.

<br />

## ⚠️ Security Warning

> [!WARNING]
>  When running MCP servers without proper sandboxing, they can execute arbitrary code on your system with the same permissions as the host process. This creates significant security risks.
>
> **Security Risks:**
> - **System Access**: Full access to files, network, and system resources
> - **Code Execution**: Can run any command on your machine
> - **Prompt Injection**: Malicious prompts could trigger unintended server actions
> - **Data Exposure**: Sensitive data may be accessed or leaked
>
> **Best Practices:**
> - Use official implementations (marked with ⭐) when available
> - Run servers in VMs or isolated environments
> - Review code before installation
> - Limit permissions to minimum required
> - Monitor server activity

<br />

## Examples of Supported Clients

| | MCP Host | Documentation |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| [Claude Desktop](https://claude.ai/download) | Claude (Mac, Windows) | [Docs](https://modelcontextprotocol.io/clients/claude-desktop) |
| [Cline](https://github.com/cline/cline) | Cline (VSCode) | [Docs](https://github.com/cline/cline?tab=readme-ov-file#mcp-servers) |
| [Continue](https://www.continue.dev) | Continue (VSCode, JetBrains) | [Docs](https://docs.continue.dev/customize/deep-dives/mcp) |
| [Cursor](https://www.cursor.com) | Cursor | [Docs](https://docs.cursor.com/context/model-context-protocol) |
| [Zed](https://zed.dev) | Zed (Editor) | [Docs](https://zed.dev/docs/extensions/language-servers/language-server-overview) |

<br />

## Table of Contents

- [AI & LLM](#ai--llm)
- [Analytics & Data](#analytics--data)
- [Code Tools](#code-tools)
- [Crypto & Blockchain](#crypto--blockchain)
- [Customer Support](#customer-support)
- [Database](#database)
- [Developer Tools](#developer-tools)
- [Documentation](#documentation)
- [E-Commerce](#e-commerce)
- [Education](#education)
- [Email & Messaging](#email--messaging)
- [ERP & CRM](#erp--crm)
- [Finance](#finance)
- [Food & Nutrition](#food--nutrition)
- [Gaming](#gaming)
- [Healthcare](#healthcare)
- [Human Resources](#human-resources)
- [Knowledge & Learning](#knowledge--learning)
- [Local Utilities](#local-utilities)
- [Maps & Location](#maps--location)
- [Media & Creative](#media--creative)
- [News & Information](#news--information)
- [Personal Productivity](#personal-productivity)
- [Product Management](#product-management)
- [Project Management](#project-management)
- [Real Estate](#real-estate)
- [Research & Analysis](#research--analysis)
- [Sales & Marketing](#sales--marketing)
- [Scientific](#scientific)
- [Search](#search)
- [Social Media](#social-media)
- [Software Development](#software-development)
- [Utilities](#utilities)
- [Web & Browser](#web--browser)
- [Web3 & Blockchain](#web3--blockchain)

<br />

## AI & LLM

### Anthropic Prompt Caching

**[anthropic-prompt-caching](https://github.com/modelcontextprotocol/servers/tree/main/src/anthropic-prompt-caching)** - Enable claude to cache prompts for improved performance and cost efficiency.

- **Language**: Typescript
- **Availability**: Open source
- **Installation**: `npx -y @modelcontextprotocol/server-anthropic-prompt-caching`

### Bedrock Runtime

**[bedrock-runtime](https://github.com/modelcontextprotocol/servers/tree/main/src/bedrock-runtime)** - Provides access to various AWS Bedrock models through the Bedrock Runtime API.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[bedrock-runtime]`

### Claude Model Context Protocol

**[claude-api](https://github.com/modelcontextprotocol/servers/tree/main/src/Claude)** - Provides access to Claude models directly through MCP.

- **Language**: Typescript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-claude`

### Ollama Integration

**[ollama-mcp-server](https://github.com/yadPe/ollama_mcp_server)** - Server implementation that integrates with local Ollama instances, allowing you to use local LLMs through the MCP.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install ollama-mcp-server`

### OpenAI API

**[openai-api](https://github.com/modelcontextprotocol/servers/tree/main/src/openai)** - Access OpenAI models through the MCP protocol.

- **Language**: Typescript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-openai`

### xAI Grok

**[xai-grok](https://github.com/modelcontextprotocol/servers/tree/main/src/xai)** - Server for interacting with xAI's Grok models.

- **Language**: Typescript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-xai`

<br />

## Analytics & Data

### Census MCP Server

**[census](https://github.com/sutrolabs/census-mcp-server)** - Census provides an MCP server for accessing operational, reverse ETL, and activation capabilities of the Census platform.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install census-mcp-server`

### Coda MCP Server

**[coda-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/coda)** - Interact with Coda API and tables.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-coda`

### Datadog Integration

**[datadog-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/datadog)** - Provides access to Datadog API.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-datadog`

### DuckDB

**[duckdb](https://github.com/modelcontextprotocol/servers/tree/main/src/duckdb)** - Read-only access to DuckDB databases.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[duckdb]`

### Elasticsearch MCP Server

**[elasticsearch-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/elasticsearch)** - Query and search Elasticsearch indices.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-elasticsearch`

### Google Analytics MCP Server

**[google-analytics](https://github.com/modelcontextprotocol/servers/tree/main/src/google-analytics)** - Fetch Google Analytics data.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[google-analytics]`

### Grafana MCP Server

**[grafana-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/grafana)** - Access Grafana dashboards and data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-grafana`

### Metabase Integration

**[metabase-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/metabase)** - Provides access to Metabase for data analysis.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-metabase`

### MongoDB MCP Server

**[mongodb](https://github.com/modelcontextprotocol/servers/tree/main/src/mongodb)** - Query MongoDB databases.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-mongodb`

### Pandas Integration

**[pandas-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/pandas)** - Analyze data with Pandas through MCP.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[pandas]`

### Prometheus MCP Server

**[prometheus-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/prometheus)** - Access Prometheus metrics and data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-prometheus`

### SQLite MCP Server

**[sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite)** - Query SQLite databases (read-only or read-write).

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[sqlite]`

<br />

## Code Tools

### Bash Integration

**[bash-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/bash)** - Execute bash commands and shell operations.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-bash`

### Git Server

**[git-server](https://github.com/modelcontextprotocol/servers/tree/main/src/git)** - Access Git repositories with full version control integration.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[git]`

### Github Integration

**[github-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/github)** - Integration with GitHub repositories, issues, and pull requests.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-github`

### Gitlab Integration

**[gitlab-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab)** - Integration with GitLab repositories and APIs.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-gitlab`

### Python REPL

**[python-repl](https://github.com/modelcontextprotocol/servers/tree/main/src/python)** - Execute Python code with full standard library access.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[python]`

### Docker Integration

**[docker-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/docker)** - Manage and interact with Docker containers.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-docker`

<br />

## Crypto & Blockchain

### Alchemy

**[alchemy-mcp-server](https://github.com/alchemyplatform/alchemy-mcp-server)** ⭐ - Comprehensive Alchemy API integration with web3 capabilities.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g alchemy-mcp-server`
- **Endpoint**: https://alchemy.alchemyapi.io/

### Axiom

**[axiom-mcp-server](https://github.com/axiom-crypto/axiom-mcp-server)** - Integrate with Axiom for ZK-powered data infrastructure.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install axiom-mcp-server`
- **Endpoint**: https://axiom.xyz

### Coinbase Agentkit

**[coinbase-agentkit](https://github.com/coinbase/coinbase-agentkit)** ⭐ - CDPAgentKit MCP server for secure onchain interactions.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install coinbase-agentkit-core`
- **Endpoint**: https://cdp.coinbase.com

### Etherscan Integration

**[etherscan-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/etherscan)** - Query blockchain data through Etherscan API.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-etherscan`
- **Endpoint**: https://etherscan.io/apis

### EVMole

**[evmole](https://github.com/fomxgoq/evmole)** - Extract function and state variable names from EVM bytecode.

- **Language**: Rust
- **Availability**: Open source
- **Installation**: See [GitHub repository](https://github.com/fomxgoq/evmole)

### Helius

**[helius-mcp-server](https://github.com/helius-labs/helius-mcp-server)** ⭐ - Solana infrastructure with RPC, webhooks, and development tools.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install helius-mcp-server`
- **Endpoint**: https://helius.dev/

### Jupiter

**[jupiter-mcp-server](https://github.com/jup-ag/jupiter-mcp-server)** ⭐ - Access Jupiter swap aggregator for Solana token trading.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install jupiter-mcp-server`
- **Endpoint**: https://jup.ag/

### Magic Eden

**[magiceden-mcp-server](https://github.com/magiceden-io/magiceden-mcp-server)** ⭐ - Access Magic Eden NFT marketplace data and trading on Solana, Polygon, and Bitcoin.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install @magiceden-io/mcp-server`
- **Endpoint**: https://magiceden.io/

### Moonwell Finance

**[moonwell-mcp-server](https://github.com/moonwell-fi/moonwell-mcp-server)** - Access Moonwell Finance lending protocol.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install moonwell-mcp-server`
- **Endpoint**: https://moonwell.fi/

### Notional Finance

**[notional-mcp-server](https://github.com/notional-finance/notional-mcp-server)** - Interact with Notional Finance fixed-rate lending and structured products.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install notional-mcp-server`
- **Endpoint**: https://notional.finance/

### OKX Web3 MCP Server

**[okx-web3-mcp-server](https://github.com/okx/okx-web3-mcp-server)** ⭐ - Comprehensive Web3 infrastructure for 12+ blockchains.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install okx-web3-mcp-server`
- **Endpoint**: https://www.okx.com/web3

### Polymarket

**[polymarket-mcp-server](https://github.com/polymarket/polymarket-mcp-server)** ⭐ - Access Polymarket prediction market data and trading.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install polymarket-mcp-server`
- **Endpoint**: https://polymarket.com/

### Solana Toolkit

**[solana-toolkit-mcp-server](https://github.com/sendmecash/solana-toolkit)** - Comprehensive Solana blockchain interaction tools.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install solana-toolkit`
- **Endpoint**: https://api.mainnet-beta.solana.com/

### Stacks MCP Server

**[stacks-mcp-server](https://github.com/stacksgov/stacks-mcp-server)** - Interact with Stacks blockchain smart contracts and transactions.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install stacks-mcp-server`
- **Endpoint**: https://stacks.co/

### ZKSync Era

**[zksync-era-mcp-server](https://github.com/matter-labs/zksync-era-mcp-server)** - Access ZKSync Era Layer 2 blockchain.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install zksync-era-mcp-server`
- **Endpoint**: https://era.zksync.io/

<br />

## Customer Support

### Zendesk Integration

**[zendesk-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/zendesk)** - Manage Zendesk support tickets and customer interactions.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-zendesk`

<br />

## Database

### DuckDB

**[duckdb](https://github.com/modelcontextprotocol/servers/tree/main/src/duckdb)** - Read-only access to DuckDB databases.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[duckdb]`

### Google Firestore

**[firestore-mcp-server](https://github.com/gusio-ai/firestore-mcp-server)** - Query and manage Firestore databases.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install firestore-mcp-server`

### MongoDB MCP Server

**[mongodb](https://github.com/modelcontextprotocol/servers/tree/main/src/mongodb)** - Query MongoDB databases.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-mongodb`

### MySQL Server

**[mysql-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/mysql)** - Connect to and query MySQL databases.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[mysql]`

### PostgreSQL Server

**[postgres-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres)** - Query PostgreSQL databases with full SQL support.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-postgres`

### SQLite MCP Server

**[sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite)** - Query SQLite databases (read-only or read-write).

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[sqlite]`

<br />

## Developer Tools

### HTTP Server

**[http-server](https://github.com/modelcontextprotocol/servers/tree/main/src/http)** - Make HTTP requests and interact with APIs.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-http`

### Sentry Integration

**[sentry-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/sentry)** - Access Sentry error tracking and monitoring.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-sentry`

### Linear Integration

**[linear-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/linear)** - Manage Linear issues and projects.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-linear`

### Jira Server

**[jira-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/jira)** - Manage Jira issues and projects.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-jira`

### Slack Integration

**[slack-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/slack)** - Manage Slack messages and channels.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[slack]`

<br />

## Documentation

### Notion Integration

**[notion-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/notion)** - Query and create Notion pages and databases.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[notion]`

### Obsidian Vault

**[obsidian-mcp-server](https://github.com/obsidian-community/obsidian-mcp)** ⭐ - Query and create notes in Obsidian vaults.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g obsidian-mcp`
- **Endpoint**: https://obsidian.md/

<br />

## E-Commerce

### Shopify Integration

**[shopify-mcp-server](https://github.com/Shopify/mcp-server-shopify)** ⭐ - Access Shopify store data and perform operations.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @shopify/mcp-server-shopify`
- **Endpoint**: https://shopify.com/

<br />

## Education

### Eduflow Integration

**[eduflow-mcp-server](https://github.com/Eduflow/mcp-server)** - Integrate with Eduflow for learning and assessment.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g eduflow-mcp-server`

<br />

## Email & Messaging

### Gmail Integration

**[gmail-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/gmail)** - Access Gmail messages and send emails.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-gmail`

### Twilio Integration

**[twilio-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/twilio)** - Send SMS and manage Twilio communications.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-twilio`

<br />

## ERP & CRM

### Salesforce Integration

**[salesforce-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/salesforce)** - Interact with Salesforce CRM.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-salesforce`

### Hubspot Integration

**[hubspot-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/hubspot)** - Integrate with HubSpot CRM and marketing.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-hubspot`

<br />

## Finance

### Coinbase Agentkit

**[coinbase-agentkit](https://github.com/coinbase/coinbase-agentkit)** ⭐ - CDPAgentKit MCP server for secure onchain interactions.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install coinbase-agentkit-core`
- **Endpoint**: https://cdp.coinbase.com

### Lightyear CryptoPunks

**[lightyear-cryptopunks](https://github.com/Lightyear-HDG/awesome-mcp-servers)** - Free, open MCP server for CryptoPunks marketplace data.

- **Language**: REST API
- **Availability**: Open source
- **Installation**: Direct API access
- **Tools**: 11 tools including browse traits, filter punks, listings, bids, Merkle roots, bid recommendations
- **Endpoint**: https://punks.lightyear.build/api/mcp

### Moody's Integration

**[moodys-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/moodys)** - Access Moody's credit ratings and financial data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-moodys`

### SEC Filings (Edgar)

**[sec-filings-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/sec)** - Query SEC Edgar filings and financial reports.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install sec-filings-mcp-server`

### Stock Market Data

**[stock-market-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/stock-market)** - Real-time stock market data and trading information.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-stock-market`

### Yahoo Finance

**[yahoo-finance-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/yahoo-finance)** - Access Yahoo Finance market data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-yahoo-finance`

<br />

## Food & Nutrition

### Spoonacular

**[spoonacular-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/spoonacular)** - Access recipe and nutrition data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-spoonacular`

<br />

## Gaming

### Discord Integration

**[discord-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/discord)** - Manage Discord servers and messages.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-discord`

### Steam

**[steam-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/steam)** - Access Steam game library and store data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-steam`

<br />

## Healthcare

### FHIR Health Records

**[fhir-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/fhir)** - Access FHIR health records.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[fhir]`

<br />

## Human Resources

### Workday Integration

**[workday-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/workday)** - Integrate with Workday HCM system.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-workday`

<br />

## Knowledge & Learning

### Coursera

**[coursera-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/coursera)** - Access Coursera course data and learning resources.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-coursera`

<br />

## Local Utilities

### File System MCP Server

**[file-server](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)** - Read, write, and manage files and directories.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[filesystem]`

### Memory Manager

**[memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory)** - Persistent memory storage for long-term context.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-memory`

### Time Tracking

**[time-tracking-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/time-tracking)** - Track time and manage time entries.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-time-tracking`

<br />

## Maps & Location

### Google Maps

**[google-maps-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/google-maps)** - Access Google Maps API for location data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-google-maps`

<br />

## Media & Creative

### Adobe Creative Cloud

**[adobe-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/adobe)** - Integrate with Adobe Creative Cloud applications.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-adobe`

### Cloudinary

**[cloudinary-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/cloudinary)** - Manage images and media on Cloudinary.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-cloudinary`

### DALL-E 3 Image Generation

**[dall-e-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/dall-e)** - Generate images using DALL-E 3.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-dall-e`

### Figma Integration

**[figma-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/figma)** - Access Figma designs and components.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-figma`

### Midjourney

**[midjourney-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/midjourney)** - Generate images and manage Midjourney projects.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-midjourney`

### Spotify Integration

**[spotify-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/spotify)** - Access Spotify music and playlist data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-spotify`

### Unsplash

**[unsplash-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/unsplash)** - Access Unsplash free stock photos.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-unsplash`

<br />

## News & Information

### NewsAPI

**[newsapi-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/newsapi)** - Access news articles and headlines.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-newsapi`

### Wikipedia

**[wikipedia-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/wikipedia)** - Query Wikipedia articles and content.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-wikipedia`

<br />

## Personal Productivity

### Todoist Integration

**[todoist-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/todoist)** - Manage Todoist tasks and projects.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-todoist`

### Microsoft Teams

**[teams-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/teams)** - Integrate with Microsoft Teams.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-teams`

### Google Calendar

**[google-calendar-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/google-calendar)** - Access and manage Google Calendar events.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-google-calendar`

<br />

## Product Management

### Amplitude

**[amplitude-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/amplitude)** - Access Amplitude analytics and user data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-amplitude`

<br />

## Project Management

### Asana

**[asana-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/asana)** - Manage Asana projects and tasks.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-asana`

### Monday.com

**[monday-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/monday)** - Integrate with Monday.com work management.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-monday`

### Trello

**[trello-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/trello)** - Manage Trello boards and cards.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-trello`

### Microsoft Project

**[microsoft-project-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/project)** - Manage Microsoft Project files and timelines.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-project`

<br />

## Real Estate

### Zillow

**[zillow-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/zillow)** - Access Zillow real estate data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-zillow`

<br />

## Research & Analysis

### Brave Search

**[brave-search-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search)** - Access Brave Search API for web search.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-brave-search`

### Google Scholar

**[google-scholar-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/google-scholar)** - Search academic papers and citations.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-google-scholar`

### PubMed

**[pubmed-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/pubmed)** - Access PubMed medical research papers.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[pubmed]`

### Semantic Scholar

**[semantic-scholar-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/semantic-scholar)** - Access Semantic Scholar academic database.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-semantic-scholar`

<br />

## Sales & Marketing

### Marketo Integration

**[marketo-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/marketo)** - Access Marketo marketing automation.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-marketo`

<br />

## Scientific

### Arxiv Papers

**[arxiv-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/arxiv)** - Search and retrieve ArXiv papers.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[arxiv]`

<br />

## Search

### Brave Search

**[brave-search-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search)** - Access Brave Search API for web search.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-brave-search`

### Jina

**[jina-mcp-server](https://github.com/jina-ai/jina-mcp-server)** ⭐ - Advanced web search and retrieval powered by Jina.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install jina-mcp-server`
- **Endpoint**: https://jina.ai/

<br />

## Social Media

### Instagram Integration

**[instagram-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/instagram)** - Access Instagram API and manage posts.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-instagram`

### LinkedIn

**[linkedin-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/linkedin)** - Access LinkedIn posts and profile data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-linkedin`

### Reddit

**[reddit-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/reddit)** - Search and retrieve Reddit posts and comments.

- **Language**: Python
- **Availability**: Open source
- **Installation**: `pip install mcp[reddit]`

### Twitter/X

**[twitter-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/twitter)** - Access Twitter/X API and manage posts.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-twitter`

### Bluesky

**[bluesky-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/bluesky)** - Access Bluesky social network.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-bluesky`

<br />

## Software Development

### AWS CodeBuild

**[aws-codebuild-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/aws-codebuild)** - Integrate with AWS CodeBuild.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-aws-codebuild`

<br />

## Utilities

### QR Code Generator

**[qr-code-generator](https://github.com/modelcontextprotocol/servers/tree/main/src/qr-code)** - Generate QR codes.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-qr-code`

<br />

## Web & Browser

### Playwright Browser

**[playwright-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/playwright)** - Control and interact with web browsers using Playwright.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-playwright`

### Puppeteer Browser

**[puppeteer-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer)** - Browser automation with Puppeteer.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-puppeteer`

<br />

## Web3 & Blockchain

### Alchemy

**[alchemy-mcp-server](https://github.com/alchemyplatform/alchemy-mcp-server)** ⭐ - Comprehensive Alchemy API integration with web3 capabilities.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g alchemy-mcp-server`
- **Endpoint**: https://alchemy.alchemyapi.io/

### Axiom

**[axiom-mcp-server](https://github.com/axiom-crypto/axiom-mcp-server)** - Integrate with Axiom for ZK-powered data infrastructure.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install axiom-mcp-server`
- **Endpoint**: https://axiom.xyz

### Bitcoin Ordinals

**[bitcoin-ordinals-mcp-server](https://github.com/modelcontextprotocol/servers/tree/main/src/bitcoin-ordinals)** - Access Bitcoin Ordinals and inscriptions data.

- **Language**: TypeScript
- **Availability**: Open source
- **Installation**: `npm install -g @modelcontextprotocol/server-bitcoin-ordinals`

<br />

## Contributing

This is a community-driven list. To contribute, please follow the [Contribution Guidelines](CONTRIBUTING.md).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Stephen Akinyemi](https://github.com/appcypher) has waived all copyright and related or neighboring rights to this work.