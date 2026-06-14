# Unity Gaming Services GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Unity Gaming Services (UGS) platform, covering the full breadth of cloud services available to game developers. Unity Gaming Services provides a suite of REST APIs for authentication, cloud code, cloud save, economy, leaderboards, matchmaking, multiplayer, analytics, remote configuration, and more. This schema models those services as a unified GraphQL type system, enabling unified querying and mutation of game backend resources.

## Source APIs

- **Player Authentication API** — https://services.docs.unity.com/player-auth-admin/v1/
- **Cloud Code API** — https://services.docs.unity.com/cloud-code-admin/v1/
- **Cloud Save API** — https://services.docs.unity.com/cloud-save-admin/v1/
- **Economy API** — https://services.docs.unity.com/economy-admin/v2/
- **Leaderboards API** — https://services.docs.unity.com/leaderboards-admin/v1/
- **Remote Config API** — https://services.docs.unity.com/remote-config-admin/v1/
- **Analytics API** — https://services.docs.unity.com/analytics/v1/
- **Lobby API** — https://docs.unity.com/ugs/en-us/manual/lobby/manual/lobby-apis
- **Matchmaker API** — https://services.docs.unity.com/matchmaker-admin/v3/
- **Relay API** — https://services.docs.unity.com/relay-allocations/v1/
- **Multiplay Game Server Hosting API** — https://services.docs.unity.com/multiplay-config/v1/
- **Friends API** — https://services.docs.unity.com/friends/v1/
- **Push Notifications API** — https://docs.unity.com/ugs/en-us/manual/push-notifications/manual/overview
- **Build Automation API** — https://build-api.cloud.unity3d.com/docs/

## Schema Source

- **File**: `unity-schema.graphql`
- **Types**: 65+
- **Schema Style**: Conceptual (derived from REST API surface, not a native GraphQL implementation)

## Type Categories

### Project and Environment Management
- `Project` — top-level organizational unit containing all UGS resources
- `Environment` — isolated runtime context (production, staging, development) within a project

### Build and DevOps
- `Build` — a compiled game artifact produced by the Build Automation service
- `BuildConfiguration` — platform target and settings that drive a build job

### Cloud Code (Serverless Functions)
- `CloudCode` — aggregate representation of the Cloud Code service for a project
- `CloudCodeModule` — compiled C# module deployed to the serverless runtime
- `CloudCodeScript` — JavaScript script deployed to the serverless runtime
- `Function` — callable unit within a cloud code module or script
- `FunctionInvocation` — a single execution record of a cloud code function

### Cloud Save (Persistent Storage)
- `CloudSave` — service-level aggregate for player and game data persistence
- `CloudSaveData` — a key-value data item stored for a player or shared game state

### Economy
- `Economy` — aggregate for in-game economy configuration
- `EconomyCurrency` — virtual currency definition (type, initial balance, limits)
- `EconomyResource` — abstract base for purchasable or grantable economy resources
- `EconomyVirtualPurchase` — exchange of virtual currency for items or other currency
- `EconomyRealMoneyPurchase` — in-app purchase configuration backed by store receipts
- `EconomyInventoryItem` — a player's instance of a resource in their inventory

### Social / Friends
- `Friends` — service aggregate for the social graph
- `FriendRequest` — pending or resolved friend request between two players
- `Presence` — real-time online/activity status for a player

### Lobby
- `Lobby` — a pre-match gathering space for players with custom data and filters

### Players and Identity
- `Player` — a registered game player with profile, authentication, and service data

### Leaderboards and Scores
- `Leaderboard` — ranked list configuration with scoring rules and reset schedules
- `LeaderboardEntry` — a single player's ranked record in a leaderboard
- `Score` — a numeric score value submitted to a leaderboard

### Matchmaking
- `Match` — a completed match result linking players to a game server
- `MatchmakerTicket` — a request submitted to the matchmaker for player grouping
- `Ticket` — alias/variant representation of a matchmaking ticket state

### Multiplay / Game Server Hosting
- `Multiplay` — service aggregate for dedicated game server infrastructure
- `Server` — a physical or virtual machine running game server processes
- `ServerAllocation` — a reservation of a server for an active game session
- `Fleet` — a managed pool of servers with auto-scaling rules
- `FleetRegion` — geographic deployment region within a fleet
- `GameServer` — a running game server process with lifecycle state

### Analytics
- `Analytics` — service aggregate for event ingestion and reporting
- `Event` — a single player or game telemetry event
- `EventBatch` — a collection of events submitted together for efficiency
- `UserAttribute` — a custom attribute segment applied to a player

### Remote Config
- `RemoteConfig` — service aggregate for runtime configuration delivery
- `GameOverride` — a conditional rule that overrides default config values for a segment
- `ConfigValue` — a typed key-value configuration entry

### Authentication and Tokens
- `Authentication` — service aggregate for player identity and session management
- `AccessToken` — a short-lived JWT granting access to UGS services
- `SignIn` — a completed sign-in session record
- `GuestSignIn` — an anonymous/guest sign-in session
- `UnityToken` — a Unity-issued token encapsulating player session identity

### Notifications
- `Notification` — a push notification definition targeted at player devices

### Relay (Peer-to-Peer Networking)
- `Relay` — service aggregate for relay-based multiplayer networking
- `RelayAllocation` — a relay server slot allocated for a host player
- `RelayAllocationJoin` — a relay join token allowing a client to connect to a relay allocation

### Subscriptions / Real-Time
- `Subscription` — a real-time event subscription for live data updates

## Queries

The schema exposes queries for:
- Fetching projects and environments
- Retrieving cloud code scripts and modules
- Reading player cloud save data
- Querying economy currencies and inventory
- Reading leaderboard rankings
- Inspecting matchmaker queues and tickets
- Listing game server fleets and allocations
- Fetching analytics event history
- Reading remote configuration values
- Retrieving authentication tokens and sessions
- Listing friend relationships and presence
- Querying lobby rooms

## Mutations

The schema exposes mutations for:
- Creating and deploying cloud code scripts/modules
- Writing and deleting cloud save data
- Granting currency and processing purchases
- Submitting leaderboard scores
- Creating and joining lobbies
- Submitting matchmaking tickets
- Allocating game server resources
- Ingesting analytics events
- Updating remote config values
- Signing players in and refreshing tokens
- Sending friend requests and managing relationships
- Scheduling push notifications

## References

- Unity Gaming Services Documentation: https://docs.unity.com/ugs
- Unity Services API Reference: https://services.docs.unity.com/
- Unity Technologies GitHub: https://github.com/Unity-Technologies
