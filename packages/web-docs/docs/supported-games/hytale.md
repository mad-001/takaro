# Hytale

Takaro supports Hytale servers through our generic connector and the Hytale-Takaro Integration mod. This integration enables real-time player event streaming, Discord integration, player management capabilities, and remote server control.

## Installation

To connect your Hytale server to Takaro, you'll need to install the Hytale-Takaro Integration mod on your existing Hytale server.

### Requirements

- Hytale dedicated server
- Administrative access to your server files
- [Takaro account](https://takaro.io)

### Getting a Takaro Account

1. Visit [Takaro](https://takaro.io) and complete the survey
2. Join the [Takaro Discord](https://discord.gg/pwenDRrtnA) and request an invite

### Mod Installation

1. Download the latest Hytale-Takaro Integration mod from the [GitHub releases page](https://github.com/gettakaro/Hytale-Takaro-Integration/releases)
2. Place the mod JAR file in your Hytale server's `mods` directory
3. Start your server to generate the configuration file
4. Stop the server to edit the configuration

## Configuration

After installation, you'll need to configure the mod with your Takaro authentication tokens.

Edit the configuration file at `\Hytale\Server\mods\dev.takaro_HytaleTakaroIntegration\config.properties`:

```properties
# Get these from your Takaro dashboard
IDENTITY_TOKEN=NAME-YOUR-SERVER-WHATEVER-YOU-WANT
REGISTRATION_TOKEN=GET_THIS_FROM_THE_DIRECTIONS_BELOW
```

### Getting Your Tokens

1. **Identity Token**: Use a unique identifier for your Hytale server
2. **Registration Token**: Obtain this from your Takaro dashboard:
   - Navigate to Settings → Game Servers
   - Click "Add Game Server"
   - Select "Generic" as the game type
   - Copy the Registration Token

After updating the configuration, start your Hytale server. The mod will automatically connect to Takaro.

## Features

### Events

- Player join/leave notifications
- Chat message relay
- Real-time player tracking

### Commands

- Execute console commands remotely
- Send messages to players
- Give items to players
- Teleport players
- Kick/ban/unban players

### Information

- Player list with real-time locations
- Server info and status
- Complete items database
- Player inventory viewing

## How Takaro Connects to Your Hytale Server

The Hytale-Takaro Integration mod establishes a connection to Takaro using the generic connector protocol. Once connected, the mod:

- Streams real-time events from your Hytale server to Takaro
- Receives and executes commands from Takaro
- Provides player and server information on demand
- Enables Discord integration and advanced automation features

## Support and Development

For the most up-to-date information about supported features, troubleshooting, and development status, visit the [Hytale-Takaro Integration GitHub repository](https://github.com/gettakaro/Hytale-Takaro-Integration).

If you encounter issues or need help:

- Report bugs on [GitHub Issues](https://github.com/gettakaro/Hytale-Takaro-Integration/issues)
- Join the [Takaro Discord](https://discord.gg/pwenDRrtnA) for community support
