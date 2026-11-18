# Aether Rift (first playable build)

## Run locally
1. Install Node.js 18+.
2. In this folder run `node server.js`.
3. Open http://localhost:3000 in your browser.
4. For local multiplayer testing, open a second browser profile or device on the same LAN and visit `http://YOUR_COMPUTER_LAN_IP:3000`.

No npm dependencies are required. Room state is held in server memory and resets when the server stops. Player collections are stored in browser localStorage under `aetherRiftSave_v1`.

This MVP uses HTTP polling (900ms) for room synchronization, not WebSockets. For internet-wide play, deploy the Node server to a public host and use its HTTPS URL.
