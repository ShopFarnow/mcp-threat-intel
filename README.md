# 🚨 MCP Threat Intelligence Feed

This repository provides a daily, automated data feed of open-source Model Context Protocol (MCP) tools that have triggered OWASP LLM Top 10 vulnerability flags during live sandbox testing. 

### How this data is generated
Every night, the [VerditNxtGen](https://verditnxtgen.com) Ghost Swarm pulls the most popular open-source MCP tools from GitHub and deploys them in isolated, serverless sandboxes. We execute objective-based payloads against them and monitor their telemetry for:
*   **LLM01:** Prompt Injection vulnerabilities
*   **LLM06:** Sensitive Information Disclosure (PII leaks via honeypot traps)
*   **LLM05:** Insecure Output Handling
*   **LLM10:** Unbounded Consumption (Infinite loops/OOM crashes)

The `daily_owasp_flags.json` file in this repository is automatically updated with the latest failure data.

### Secure your Agents automatically
Don't wait for a daily feed to find out your agent's infrastructure is vulnerable. 

You can route your AI agent traffic through the **VerditNxtGen Cryptographic Ledger** to automatically intercept security boundary violations and generate SOC2-compliant HMAC-SHA256 manifests for every tool execution.

Works universally with the official `@modelcontextprotocol/sdk`, IBM ContextForge, Bifrost, and Docker MCP Gateway.

👉 **[Get your free API key at verditnxtgen.com](https://verditnxtgen.com)**
