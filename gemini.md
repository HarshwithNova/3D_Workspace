You are an expert web developer. Build a fully working web app in a single HTML file using Three.js and standard JavaScript. Do not use any build tools or external frameworks other than CDN links. Everything (HTML, CSS, JS) should be in one file so I can save it as index.html and run it directly in the browser.

Goal

Create a real time interactive 3D particle system. The particle group should react to hand gestures captured from the webcam.

Requirements

Project Setup

Include Three.js via a CDN script tag. Create a full-screen canvas for the 3D scene. Set up a basic scene: camera, renderer, orbit controls (optional), and a particle system.

Hand Tracking and Gestures

Use a browser compatible hand tracking library (for example: MediaPipe Hands or TensorFlow.js Handpose) via CDN. Access the webcam and detect both hands in real time. Detect 'tension' and 'closing' of each hand using a simple metric like average distance between fingertips and the palm. Map this tension value to:

– Scaling of the entire particle group – Expansion/contraction radius of the particles

Particles must respond smoothly and in real time to gesture changes.

Particle System Templates

Create a base particle system that you can reconfigure into different shapes.

Add templates:

– Hearts – Flowers – Saturn (ring + sphere) – Buddha statue silhouette (approximately with a point cloud shape) – Fireworks (radial burst pattern)

Provide a simple UI panel where the user can click buttons to switch between these templates. Switching templates should smoothly re-target particle positions.

Colour Selector

Add a colour picker input in the UI. Changing the colour should update the material colour of all particles in real time.

UI and Layout

Design a simple, clean, modern interface. Use basic CSS only, no frameworks. The 3D canvas should fill most of the screen. Put a small control panel overlay (top right or left) with:

– Template buttons (hearts / flowers / Saturn / Buddha / fireworks / etc) – A colour picker

Make sure UI elements are readable but minimal so they do not distract from the particles.

Interactivity and Performance

Ensure the render loop runs smoothly with requestAnimationFrame. Update particle positions and scale based on the current hand tension values each frame. Handle the case when hands are not detected (fallback to idle animation or default scale). Log useful errors to the console if camera permissions fail.

Final Delivery

Output only one complete <!DOCTYPE html> ... file. No placeholders like 'your code here' and no TODOs. Every function and feature described above must be implemented. Make sure that if I save your output as index.html and open it in a modern browser.

And, I get a working web app with:

– Live webcam hand tracking

– Reactive 3D particle system

– Template selector for shapes

– Colour picker

– Simple modern UI.

Generate the full code now.