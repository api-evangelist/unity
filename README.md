# Unity

Unity is a cross-platform real-time development platform that provides a comprehensive suite of APIs and services for game development, interactive 3D content creation, and live game operations. Unity Gaming Services (UGS) delivers cloud-hosted services covering multiplayer networking, live operations, player economy, analytics, authentication, DevOps automation, and social features.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/unity/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Game Development
- Real-Time 3D
- Multiplayer
- Game Services
- Cloud Gaming

## Timestamps

- **Created:** 2025-01-08
- **Modified:** 2026-05-03

## APIs

| API | Description | Reference |
|-----|-------------|-----------|
| Player Authentication | Anonymous, platform, and custom identity sign-in | [Docs](https://docs.unity.com/ugs/en-us/manual/authentication/manual/rest-api) |
| Economy | Virtual currencies, inventory, and purchases | [Docs](https://docs.unity.com/ugs/en-us/manual/economy/manual/write-configuration/rest-api) |
| Leaderboards | Competitive player rankings and scores | [Docs](https://docs.unity.com/ugs/en-us/manual/leaderboards/manual/write-configuration/rest-api) |
| Remote Config | Feature flags and game configuration delivery | [Docs](https://docs.unity.com/ugs/en-us/manual/remote-config/manual/write-configuration/rest-api) |
| Cloud Save | Player data and game state persistence | [Docs](https://docs.unity.com/ugs/en-us/manual/cloud-save/manual/reference/rest-api) |
| Cloud Code | Serverless JavaScript and C# game logic | [Docs](https://docs.unity.com/ugs/en-us/manual/cloud-code/manual) |
| Analytics | Custom event ingestion and behavior tracking | [Docs](https://docs.unity.com/ugs/en-us/manual/analytics/manual/rest-api) |
| Lobby | Multiplayer lobby creation and management | [Docs](https://docs.unity.com/ugs/en-us/manual/lobby/manual/lobby-apis) |
| Matchmaker | Skill-based player matchmaking | [Docs](https://docs.unity.com/ugs/en-us/manual/matchmaker/manual/matchmaker-api) |
| Relay | Secure peer-to-peer relay networking | [Docs](https://docs.unity.com/ugs/en-us/manual/relay/manual/rest-api) |
| Multiplay Game Server Hosting | Dedicated game server fleet management | [Docs](https://docs.unity.com/ugs/en-us/manual/game-server-hosting/manual/api/rest-api) |
| Cloud Content Delivery | CDN-backed game asset and update delivery | [Docs](https://docs.unity.com/ugs/manual/ccd/manual/ccd-rest-api) |
| Triggers | Event-driven Cloud Code execution | [Docs](https://docs.unity.com/ugs/en-us/manual/cloud-code/manual/triggers) |
| Scheduler | Cron-based Cloud Code scheduling | [Docs](https://docs.unity.com/ugs/en-us/manual/cloud-code/manual/triggers) |
| Friends | Player social connections and presence | [Docs](https://docs.unity.com/ugs/en-us/manual/friends/manual/overview) |
| Vivox Voice and Text Chat | Real-time voice and text communication | [Docs](https://docs.unity.com/ugs/en-us/manual/vivox-unity/manual/Unity/Unity) |
| Moderation | Player behavior and content moderation | [Docs](https://docs.unity.com/ugs/en-us/manual/moderation/manual/overview) |
| Build Automation | Cloud CI/CD for automated game builds | [Docs](https://docs.unity.com/ugs/manual/devops/manual/build-automation/build-automation-api) |
| Version Control | Source control (Unity Version Control) | [Docs](https://docs.unity.com/ugs/en-us/manual/devops/manual/unity-version-control) |
| Access | Resource-level access control and permissions | [Docs](https://docs.unity.com/ugs/manual/overview/manual/access-control) |
| SCIM | Cross-domain identity management | [Docs](https://support.unity.com/hc/en-us/articles/38766626849684-How-do-I-configure-SCIM-provisioning) |
| Asset Manager | 3D asset management and sharing | [Docs](https://docs.unity.com/ugs/en-us/manual/asset-manager/manual) |
| Monetize | Ad placement and revenue management | [Docs](https://docs.unity.com/ads/en-us/manual/MonetizationResourceCenter) |
| Safe Text | AI-powered text chat moderation | [Docs](https://docs.unity.com/ugs/en-us/manual/safe-text/manual/overview) |
| Distributed Authority | Decentralized multiplayer state management | [Docs](https://unity.com/products/distributed-authority) |
| Push Notifications | Mobile push notifications for iOS and Android | [Docs](https://docs.unity.com/ugs/en-us/manual/push-notifications/manual/overview) |

## OpenAPI Specifications

| Specification | Path |
|---|---|
| Player Authentication | [openapi/unity-player-authentication-openapi.yml](openapi/unity-player-authentication-openapi.yml) |
| Economy | [openapi/unity-economy-openapi.yml](openapi/unity-economy-openapi.yml) |
| Leaderboards | [openapi/unity-leaderboards-openapi.yml](openapi/unity-leaderboards-openapi.yml) |
| Remote Config | [openapi/unity-remote-config-openapi.yml](openapi/unity-remote-config-openapi.yml) |
| Cloud Save | [openapi/unity-cloud-save-openapi.yml](openapi/unity-cloud-save-openapi.yml) |
| Cloud Code | [openapi/unity-cloud-code-openapi.yml](openapi/unity-cloud-code-openapi.yml) |
| Analytics | [openapi/unity-analytics-openapi.yml](openapi/unity-analytics-openapi.yml) |
| Lobby | [openapi/unity-lobby-openapi.yml](openapi/unity-lobby-openapi.yml) |
| Matchmaker | [openapi/unity-matchmaker-openapi.yml](openapi/unity-matchmaker-openapi.yml) |
| Multiplay | [openapi/unity-multiplay-openapi.yml](openapi/unity-multiplay-openapi.yml) |
| Build Automation | [openapi/unity-build-automation-openapi.yml](openapi/unity-build-automation-openapi.yml) |
| Friends | [openapi/unity-friends-openapi.yml](openapi/unity-friends-openapi.yml) |

## Capabilities

### Workflow Capabilities

| Capability | Description |
|---|---|
| [Live Game Operations](capabilities/live-game-operations.yaml) | Economy, Cloud Save, and Leaderboards for live service games |
| [Multiplayer Services](capabilities/multiplayer-services.yaml) | Lobby creation, matchmaking, and server management |
| [Player Identity](capabilities/player-identity.yaml) | Authentication, account management, and data persistence |

### Shared Capability Definitions

| Shared Capability | API |
|---|---|
| [capabilities/shared/authentication.yaml](capabilities/shared/authentication.yaml) | Player Authentication API |
| [capabilities/shared/economy.yaml](capabilities/shared/economy.yaml) | Economy API |
| [capabilities/shared/leaderboards.yaml](capabilities/shared/leaderboards.yaml) | Leaderboards API |
| [capabilities/shared/lobby.yaml](capabilities/shared/lobby.yaml) | Lobby API |
| [capabilities/shared/matchmaker.yaml](capabilities/shared/matchmaker.yaml) | Matchmaker API |
| [capabilities/shared/cloud-save.yaml](capabilities/shared/cloud-save.yaml) | Cloud Save API |

## JSON Schemas

| Schema | Path |
|---|---|
| Player | [json-schema/unity-player-schema.json](json-schema/unity-player-schema.json) |
| Leaderboard | [json-schema/unity-leaderboard-schema.json](json-schema/unity-leaderboard-schema.json) |
| Economy Config | [json-schema/unity-economy-config-schema.json](json-schema/unity-economy-config-schema.json) |

## JSON Structures

| Structure | Path |
|---|---|
| Player | [json-structure/unity-player-structure.json](json-structure/unity-player-structure.json) |
| Lobby | [json-structure/unity-lobby-structure.json](json-structure/unity-lobby-structure.json) |

## Examples

| Example | Path |
|---|---|
| Submit Leaderboard Score | [examples/unity-leaderboards-add-player-score-example.json](examples/unity-leaderboards-add-player-score-example.json) |
| Make Virtual Purchase | [examples/unity-economy-make-virtual-purchase-example.json](examples/unity-economy-make-virtual-purchase-example.json) |
| Anonymous Sign-In | [examples/unity-player-authentication-sign-in-anonymously-example.json](examples/unity-player-authentication-sign-in-anonymously-example.json) |
| Create Lobby | [examples/unity-lobby-create-lobby-example.json](examples/unity-lobby-create-lobby-example.json) |
| Create Matchmaking Ticket | [examples/unity-matchmaker-create-ticket-example.json](examples/unity-matchmaker-create-ticket-example.json) |
| Save Player Data | [examples/unity-cloud-save-set-player-data-example.json](examples/unity-cloud-save-set-player-data-example.json) |

## Rules

| Ruleset | Path |
|---|---|
| Unity Spectral Rules | [rules/unity-spectral-rules.yml](rules/unity-spectral-rules.yml) |

## Vocabulary

| Vocabulary | Path |
|---|---|
| Unity Vocabulary | [vocabulary/unity-vocabulary.yml](vocabulary/unity-vocabulary.yml) |

## JSON-LD

| Context | Path |
|---|---|
| Unity Context | [json-ld/unity-context.jsonld](json-ld/unity-context.jsonld) |

## Common Properties

- [Portal](https://cloud.unity.com)
- [Dashboard](https://dashboard.unity3d.com)
- [Sign Up](https://id.unity.com)
- [Status](https://status.unity.com)
- [Support](https://support.unity.com)
- [Terms of Service](https://unity.com/legal/terms-of-service)
- [Privacy Policy](https://unity.com/legal/privacy-policy)
- [Blog](https://blog.unity.com)
- [GitHub Organization](https://github.com/Unity-Technologies)
- [API Reference](https://services.docs.unity.com/)
- [Documentation](https://docs.unity.com/ugs)
- [Pricing](https://unity.com/products/gaming-services/pricing)
- [Forum](https://discussions.unity.com/)
- [Marketplace](https://assetstore.unity.com)
- [Learning](https://learn.unity.com)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

**FN:** Unity Technologies
**Email:** support@unity.com
**URL:** https://unity.com
