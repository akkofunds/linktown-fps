# Linktown — Pocket Arena

A tiny static multiplayer arena shooter built for GitHub Pages and low-power Chromebooks.

## Play
Open the [live game](https://akkofunds.github.io/linktown-fps/). Click **Play Solo**, or one player selects **Host a Room** and shares the room code shown in the top right. Friends paste the code and select **Join**.

The game uses PeerJS 1.5.5 for WebRTC connections. Its browser bundle is included locally, so the game does not depend on an external CDN at play time. PeerJS uses its public signaling service to connect players; game traffic is peer-to-peer through the host. Rooms are temporary and last while the host's tab remains open.

## Controls
- WASD: move
- Space or left Shift: jump; hold to bunny-hop continuously
- Mouse: look and fire
- R: reload (17 rounds per magazine, unlimited reserve)
- Esc: pause

The arena is an open baseplate with an invisible perimeter barrier. A top-left minimap shows player locations. The game uses a simple canvas renderer and no 3D engine or downloaded artwork to keep CPU/GPU use low.

## Source and credits
- `index.html`: game and interface
- `peerjs.min.js`: PeerJS browser bundle (MIT License; see `PEERJS-LICENSE.txt`)
