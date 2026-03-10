#Birkbeck Under Siege: The Drill (43 Gordon Square)

Play the game live here: [Insert your GitHub Pages link here, e.g., https://www.google.com/search?q=https://yourusername.github.io/birkbeck-fire-drill/]

📌 Project Overview

"The Drill" is a 3D web-based survival simulation game developed as a first-time Game Design project. Set in the historic 43 Gordon Square building of Birkbeck University, London, the game challenges players to navigate a claustrophobic, smoke-filled environment during a fire emergency.

The primary objective is to escape the starting room (G02), avoid environmental hazards, and successfully locate and deploy the reception's fire extinguisher within a strict 10-minute time limit.

🎯 Gameplay & Mechanics

Inclusive Avatar Selection: Players begin by selecting their student ID profile, altering camera height and representing inclusivity in the student body.

Oxygen & Hazard System: The building is filling with smoke. Players have a dynamic oxygen bar that depletes slowly over time. Entering highly hazardous zones (like the open lift shaft emitting thick black smoke) will drain oxygen rapidly, resulting in asphyxiation.

Level Design: A custom 3D environment modeled after the narrow, high-ceilinged Georgian architecture of Gordon Square. Players must navigate around physical obstacles (overturned desks, partition walls) to find the objective.

Win/Loss States: * Win: Locate the red CO2 extinguisher behind the reception desk and press ENTER within a 3-meter radius.

Loss: Run out of oxygen or fail to complete the objective within the 10-minute time limit.

⌨️ Controls

This game utilizes the Pointer Lock API for immersive first-person controls.

Start: Click anywhere on the game screen to lock the mouse and look around.

Movement: W A S D or Arrow Keys

Look: Mouse Movement

Interact: ENTER (When close to the fire extinguisher)

Pause/Free Mouse: ESC

🛠️ Technology Stack

This game was built from scratch without a traditional heavy game engine (like Unity or Unreal) to ensure instant, frictionless browser playback.

HTML5 / CSS3: For the UI, HUD overlays, and Start/End screens.

JavaScript (ES6): Core game logic, state management, and interaction scripting.

Three.js (WebGL): 3D rendering, lighting (Hemisphere & Point lights), volumetric fog (FogExp2), and basic particle systems for the smoke effects.

🚀 How to Run Locally

If you wish to run the code on your local machine rather than the live link:

Clone or download this repository.

Since the game uses ES6 Modules to import Three.js, it cannot be run simply by double-clicking the HTML file (due to CORS security restrictions in modern browsers).

You must run a local web server.

If using VS Code, install the "Live Server" extension and click "Go Live" on index.html.

Alternatively, using Python in your terminal: python -m http.server 8000 and visit http://localhost:8000.

