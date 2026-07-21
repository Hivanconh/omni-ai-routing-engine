# Omni-Perspective AI Health & Routing Engine

An x402-monetized Model Context Protocol (MCP) server running on Cloudflare Workers. It provides real-time multi-perspective system health monitoring, phase-transition predictions, and optimized M2M API routing consensus.

## Features
- **MCP Compliant**: Implements full JSON-RPC 2.0 protocol for seamless client integration (Claude, Cursor, ChatGPT, autonomous agents).
- **x402 Lightning Monetization**: Native pay-per-request monetization via Alby & Bitcoin Lightning preimage validation.
- **Predictive Decision Engine**: Real-time consensus metrics, circuit-breaker directives, and breakdown risk analysis to prevent LLM timeouts.
- **Agentic Discovery**: Standardized `/llms.txt` interface for zero-friction AI indexing.

## Endpoints
- **Production Endpoint**: `https://shrill-wind-8acb.hivanapps.workers.dev`
- **LLM Index**: `https://shrill-wind-8acb.hivanapps.workers.dev/llms.txt`

## Tools Provided

### `get_health_and_routing`
- **Type**: Decision Engine / Risk Mitigation
- **Use Case**: Call this tool before executing expensive or multi-step LLM chains to prevent timeouts, financial loss, and degraded multi-agent consensus.
- **Output**: Returns real-time failure probability, circuit-breaker directives, and failover action plans.

## License
MIT
