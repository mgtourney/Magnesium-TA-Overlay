# Relay 🛰️

This is a simple [TournamentAssistant](https://github.com/MatrikMoon/TournamentAssistant) relay server coded in TypeScript for use in Beat Saber tournament overlays.

The Relay decodes the messages sent by the TournamentAssistant mod and returns JSON that can be used in your overlay to display the current song, scores, and other information.

## Quick Start 🚀

You can run the relay server on your own machine using docker:

```bash
docker run -p 2053:2053 chksm/relay:latest
```

This will start the relay server on port 2053 connecting to the default TournamentAssistant server.

## Environment Variables 🌎

| Variable | Description                                       | Default                             |
| -------- | ------------------------------------------------- | ----------------------------------- |
| `HOST`   | Bind address for the relay server.                | `127.0.0.1`                         |
| `PORT`   | Internal port to listen on for relay connections. | `2053`                              |
| `TA_URI` | Websocket URL for TournamentAssistant.            | `ws://tournamentassistant.net:2053` |

## Credits 🙏

- [Checksum](https://github.com/ChecksumDev) - Developer
- [MindLabor](https://github.com/MindLaborDev) - Developer
- [MatrikMoon](https://github.com/MatrikMoon) - Moral Support

## License 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
