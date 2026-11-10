# Linktown — Pocket Arena

A tiny static multiplayer arena shooter built for GitHub Pages and low-power Chromebooks.

## Play locally
Open `index.html` in a modern browser. Multiplayer requires an internet connection for PeerJS signaling.

## Multiplayer
One player selects **Host a room** and shares the room code shown on screen. Friends paste the code and select **Join**. The room uses PeerJS's public signaling service; game traffic is peer-to-peer. On GitHub Pages, HTTPS is provided automatically.

## Controls
- WASD: move
- Space or left Shift: jump; hold to bunny-hop continuously
- Mouse: look and fire
- R: reload (17 rounds per magazine, unlimited reserve)
- Esc: pause

The arena is an open baseplate with a perimeter barrier. A top-left minimap shows all connected players. The game intentionally uses a simple canvas renderer and no 3D engine or downloaded assets to keep CPU/GPU use low.

## Publish with GitHub Pages
Upload the contents of this folder to a GitHub repository, then in **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save. GitHub Pages is static hosting, so a new multiplayer room is created by a player each session.
