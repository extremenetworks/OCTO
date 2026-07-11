# OCTO — Office of the CTO

**Extreme Networks — Office of the CTO (OCTO)**

This repository is a directory of public projects maintained by the Office of the CTO at Extreme Networks. Each project below groups its related repositories and releases with a short description.

## Table of Contents

- [MCP XCO+ Community Server](#mcp-xco-community-server)
- [MCP SoNiC Community Server](#mcp-sonic-community-server)

---

## MCP XCO+ Community Server

A community [Model Context Protocol (MCP)](https://modelcontextprotocol.io) project for Extreme Networks **XCO+ (IP Fabric)**. It lets MCP-compatible AI assistants query and interact with an IP Fabric environment through natural language, and ships with a demo client so you can try the full workflow end to end.

The project has two components:

- **MCP XCO+ Community Server** — the MCP server itself. It exposes XCO+ (IP Fabric) operations and data as MCP tools so any MCP-compatible assistant can drive the fabric.
- **MCP XCO+ Community Demo Client** — a reference client that connects to the server and demonstrates a working end-to-end setup, useful as a starting point for your own integration.

**Links**

| Component | Repository | Releases |
|---|---|---|
| MCP XCO+ Community Server | [Repo](https://github.com/YuryOstrovsky/xco-mcp-community-server) | [Releases](https://github.com/YuryOstrovsky/xco-mcp-community-server/releases) |
| MCP XCO+ Community Demo Client | [Repo](https://github.com/YuryOstrovsky/xco-mcp-community-client-demo) | [Releases](https://github.com/YuryOstrovsky/xco-mcp-community-client-demo/releases) |

---

## MCP SoNiC Community Server

A community [Model Context Protocol (MCP)](https://modelcontextprotocol.io) project for **SoNiC**, the open-source network operating system for the software switch. It lets MCP-compatible AI assistants query and interact with a SoNiC switch through natural language, and ships with a client to try the full workflow end to end. This is a purely community effort — Extreme Networks switches do not run SoNiC at this time.

The project has two components:

- **MCP SoNiC Community Server** — the MCP server. It exposes SoNiC operations and data as MCP tools so any MCP-compatible assistant can drive the switch.
- **MCP SoNiC Community Client** — a reference client that connects to the server and demonstrates a working end-to-end setup, useful as a starting point for your own integration.

**Source & releases**

| Component | Version | Repository | Releases |
|---|---|---|---|
| MCP SoNiC Community Server | v0.2.0 | [Repo](https://github.com/YuryOstrovsky/sonic-mcp-community-server) | [v0.2.0](https://github.com/YuryOstrovsky/sonic-mcp-community-server/releases/tag/v0.2.0) · [all](https://github.com/YuryOstrovsky/sonic-mcp-community-server/releases) |
| MCP SoNiC Community Client | v0.1.1 | [Repo](https://github.com/YuryOstrovsky/sonic-mcp-community-client) | [v0.1.1](https://github.com/YuryOstrovsky/sonic-mcp-community-client/releases/tag/v0.1.1) · [all](https://github.com/YuryOstrovsky/sonic-mcp-community-client/releases) |

**Container images**

| Component | Docker Hub | GHCR |
|---|---|---|
| Server | [extremecanada/sonic-mcp-community-server](https://hub.docker.com/r/extremecanada/sonic-mcp-community-server) | [package](https://github.com/users/YuryOstrovsky/packages/container/package/sonic-mcp-community-server) |
| Client | [extremecanada/sonic-mcp-community-client](https://hub.docker.com/r/extremecanada/sonic-mcp-community-client) | [package](https://github.com/users/YuryOstrovsky/packages/container/package/sonic-mcp-community-client) |

```bash
# Server (v0.2.0 or latest)
docker pull extremecanada/sonic-mcp-community-server:0.2.0        # or :latest
docker pull ghcr.io/yuryostrovsky/sonic-mcp-community-server:0.2.0

# Client (v0.1.1 or latest)
docker pull extremecanada/sonic-mcp-community-client:0.1.1        # or :latest
docker pull ghcr.io/yuryostrovsky/sonic-mcp-community-client:0.1.1
```

**Server MCP endpoints**

- Streamable HTTP: `http://<host>:8000/mcp`
- stdio (Claude Desktop): `python -m mcp_runtime.mcp_stdio`

---

## About

The Office of the CTO drives technology strategy and innovation at Extreme Networks. This page serves as a central index to our public open-source work.

## Contact

For questions about the projects listed here, please open an issue or reach out through the relevant repository.
