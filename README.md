# Apex Apocalypse Multiplayer

Static GitHub Pages build.

## Deploy

1. Upload `index.html` to a GitHub repository.
2. Enable GitHub Pages for the repository branch/folder containing `index.html`.
3. Open the Pages URL in two or more browsers/devices.
4. Choose a username, optionally create a party and invite an online player, then press **Find Match**.
5. Once the match is found, press **Deploy**.

## Networking

The game uses PeerJS/WebRTC data channels. Player-facing peer IDs and room codes are hidden. One connected browser temporarily owns a known rendezvous peer that keeps the live lobby roster and assigns players to a match. The first player assigned becomes the game host. Human slots replace bots in a 30-combatant match.

The public PeerJS Cloud signalling service is used by default, so no server setup is required for basic testing. For a larger production deployment, use your own PeerServer/TURN infrastructure.
