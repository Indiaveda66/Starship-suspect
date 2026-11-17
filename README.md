Starship Suspect
A browser-based spaceship mystery game. Play offline with bots, or try the beta online room mode with a friend.
Play the game
1. Open starship-suspect-updated.html in a modern browser.
2. Choose your role and colour.
3. Select PLAY OFFLINE to play with bots, or use the online room controls.
For online play, host the HTML file on an HTTPS website (for example, a static-site host). Both players should open the same hosted page and have an internet connection.
Online multiplayer (beta)
Host:
1. Click CREATE ONLINE ROOM.
2. Wait for the connection status to confirm that the room was created.
3. Share the six-digit room code with your friend.
Join:
1. Enter the host's six-digit code.
2. Click JOIN and wait for the connection.
The host runs the match and the bots remain in the game. Online play uses PeerJS 1.5.4, loaded from the unpkg CDN. The browser must be able to reach that service and the PeerJS signalling service. Room creation and joining have connection timeouts; if a connection fails, check the internet connection and try again.
Online multiplayer is a beta feature. Test it with two browsers/devices before relying on it. Not every game action or meeting feature is guaranteed to be synchronized perfectly.

Controls
Action	Keyboard	Touch
Move	W A S D or arrow keys	On-screen joystick
Use task / interact / fix reactor	E	USE button
Report a body	R	REPORT button
Kill (when playing as an eligible impostor role)	Q	KILL button
Vent	V	VENT button
Special ability	F	ABILITY button


Some actions are only available when you are close enough to the relevant object or player.
How to play
- Crewmates: Complete tasks and identify the impostor. Report bodies or call the emergency meeting in the Cafeteria. The crew can win by completing tasks or removing the impostor.
- Impostor: Eliminate crewmates without being caught. Use sabotage to disrupt the crew.
- Sabotage: The impostor's SABOTAGE button cycles through Lights, Communications, and Reactor. During a reactor meltdown, a crewmate must reach the Reactor and press FIX before the countdown ends.
- Special roles: The game includes additional crew and impostor roles. Read the role description shown before starting a match.
- Bots: Bots move around the ship, perform tasks, and participate in the match.
Requirements
- A modern desktop or mobile browser with JavaScript enabled.
- Internet access is needed to load the PeerJS library and use online multiplayer.
- Offline mode can be played without joining an online room after the game file has loaded.
Files
- starship-suspect-updated.html — the game. Open this file directly or host it as a static website.
- README.md — these instructions.
Troubleshooting
- PeerJS did not load: Check your internet connection, then reload the page. The PeerJS script is loaded from unpkg.com.
- Room creation times out: Try again after a short wait. Check that the site is served over HTTPS and that your network allows access to PeerJS services.
- Cannot join: Check the six-digit code and make sure the host still has the room open.
- Friend disconnects: The host can continue the match with bots; the guest should rejoin using a newly created room if needed.
Credits and networking
Online room connections are provided by the PeerJS JavaScript library (version 1.5.4), loaded from the unpkg CDN. This project uses PeerJS for peer connection/signalling; it does not include a dedicated game server that guarantees uptime or authoritative anti-cheat validation.
