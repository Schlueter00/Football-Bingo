# Football-Bingo

This code provides a complete, single-file web application for a real-time, multiplayer NFL Bingo game. It uses Peer-to-Peer (P2P) technology, meaning no dedicated backend server is required to sync game boards between friends.

🏈 NFL Bingo 2026
A modern, mobile-responsive web application designed for interactive football viewing parties. Players can join a shared session, track each other's progress in real-time, and compete for the most Bingo wins.

🚀 Key Features
Real-Time Multiplayer: Powered by PeerJS, players connect directly to a host. When a player marks a square on their board, their "mini-map" updates on everyone else's screen instantly.
Dynamic Team Themes: Includes a comprehensive CSS theme engine with primary/secondary colors and official logos for all 32 NFL teams.
Anti-Cheat Countdown: To prevent accidental clicks from triggering a win, the app features a 5-second "Broadcasting" countdown. Players can cancel the win broadcast if they misclicked.
Live Leaderboard: A "Live Board Tracker" shows every participant’s name, their total win count, and a miniature real-time preview of their current bingo card.
Smart Persistence: Uses localStorage to remember your player name, selected team, and current board state even if you refresh the page.
Host Controls: The game creator can force a "Next Round" reset for all players, reset the entire leaderboard, or generate new invite links.
Visual Flair: Integrated with canvas-confetti for a celebratory burst when a player achieves Bingo.

🛠️ Technical Stack
Component
Technology
Frontend
HTML5, CSS3 (Flexbox/Grid), Vanilla JavaScript
P2P Networking
PeerJS
Visual Effects
Canvas-Confetti
Icons/Logos
SVG-based logos via Wikimedia Commons

🎮 How to Use
Host a Game: Simply open the HTML file in any modern browser. You are automatically assigned a unique Game ID.
Invite Friends: Click the "Invite 🔗" button to copy a unique URL. Send this to your friends.
Join a Game: When friends open your link, they will automatically connect to your session.
Play: As events happen during the NFL game (e.g., "Sack," "Touchdown Dance," "Beer Commercial"), tap the corresponding cell on your board.
Win: Get five in a row (horizontal, vertical, or diagonal) to trigger a Bingo. The host can then reset the boards for the next round.

📝 Configuration
The game logic is easily customizable within the <script> tag:
Words: Modify the bingoWords array to change the events tracked (e.g., swap NFL events for Super Bowl-specific commercials).
Colors: The teamData object contains the hex codes and logo URLs for all branding.
