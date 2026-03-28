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