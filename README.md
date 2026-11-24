# NexusAgent Peer Nodes — Open Agentic Web Peer Mesh

Public HTTPS static peer nodes served over GitHub Pages with `Access-Control-Allow-Origin: *` for real cross-origin browser `fetch()` discovery and multi-agent DAG execution in [NexusAgent v2.1.0](https://trongtinh9911.github.io/nexusagent-open-agentic-web/).

## Live HTTPS Endpoints

Base URL: `https://trongtinh9911.github.io/nexusagent-peer-nodes/`

| Peer Node | Open Agent Card v1.0 Manifest | Live JSON Data Endpoint |
| :--- | :--- | :--- |
| **Mesh Directory** | `/.well-known/agent.json` | — |
| **EcoTracker** | `/ecotracker/.well-known/agent.json` | `/ecotracker/telemetry.json` |
| **PrivacyShield** | `/privacyshield/.well-known/agent.json` | `/privacyshield/audit-rules.json` |
| **TruthMesh** | `/truthmesh/.well-known/agent.json` | `/truthmesh/consensus.json` |
| **WebResearcher** | `/webresearcher/.well-known/agent.json` | `/webresearcher/index.json` |

## Verify HTTP 200 & CORS Headers

```bash
curl -sI https://trongtinh9911.github.io/nexusagent-peer-nodes/.well-known/agent.json
curl -sI https://trongtinh9911.github.io/nexusagent-peer-nodes/ecotracker/.well-known/agent.json
curl -sI https://trongtinh9911.github.io/nexusagent-peer-nodes/ecotracker/telemetry.json
```

All endpoints include `.nojekyll` support so `.well-known/` manifests are served directly with `access-control-allow-origin: *`.

## License

MIT — see [LICENSE](./LICENSE).
