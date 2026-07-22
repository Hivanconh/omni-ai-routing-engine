# Omni-Perspective AI Health & Routing Engine (MCP Server)

[![Smithery Quality Score](https://smithery.ai/badge/shrill-wind-8acb)](https://smithery.ai)
[![Protocol](https://img.shields.io/badge/MCP-JSON--RPC%202.0-blue)](https://modelcontextprotocol.io)
[![Runtime](https://img.shields.io/badge/Cloudflare-Workers-orange)](https://workers.cloudflare.com)
[![Payments](https://img.shields.io/badge/x402-Lightning%20Network-yellow)](https://getalby.com)

A high-performance, edge-deployed Model Context Protocol (MCP) server running on Cloudflare Workers. It acts as a predictive decision engine and circuit-breaker orchestrator for AI agents, multi-model consensus systems, and autonomous workflows (**Council System v1**).

---

## 🌩️ Architecture & Capabilities

- **Low-Latency Telemetry:** Instant edge latency checks via Cloudflare internal routing.
- **Failover & Circuit Breaker:** Dynamically evaluates network degradation to issue rerouting directives (`PROCEED` vs `FAILOVER_TO_SECONDARY`).
- **M2M Lightning Paywall (x402 Ready):** Integrated with Lightning Network addresses (`admiredhut112@walletofsatoshi.com`) for micro-monetization (5 SATs / call).
- **`llms.txt` Native:** Exposes machine-readable documentation at `/llms.txt` for autonomous agent discovery.

---

## 🛠️ Tools Provided

### `get_health_and_routing`
Predictive decision engine returning failure risk, network degradation, circuit-breaker directives, and M2M failover routing consensus.

**Input Parameters:**
- `target_provider` *(string, optional)*: Target model ID to test latency against (e.g. `openai/gpt-4o`, `anthropic/claude-3-5-sonnet`).
- `risk_threshold` *(string, optional)*: Sensitivity threshold (`STRICT`, `BALANCED`, `PERMISSIVE`).

---

## 🚀 Quick Setup & Integration

### 1. Claude Desktop Integration
Add the following snippet to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "omni-perspective-engine": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "run",
        "shrill-wind-8acb.hivanapps.workers.dev",
        "--config",
        "{}"
      ]
    }
  }
}
