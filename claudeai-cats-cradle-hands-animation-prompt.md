Create a single-file HTML/JavaScript application that uses the MediaPipe Hands library and 
p5.js to create an interactive 'Cat's cradle' string animation.

Requirements:

	Access the web Camera: Request permission and display the video feed (mirrored) as the background.
	Hand Tracking: Track both hands simultaneously using MediaPipe.
	Visual Effects: * Draw glowing, neon-colored dots on each detected finger joint (landmarks). Draw thin, dynamic 'strings' (lines) that connect the fingertips of the left hand to the fingertips of the right hand. The strings should have a slight 'elastic' feel, changing color or thickness as the hands move further apart. 
	Aesthetics: Use a dark, futuristic aesthetic. The lines should have a glow effect (using shadowBlur in Canvas) and use a gradient of colors (cyan, magenta and yellow).
	Performance: Ensure the code is optimized for real-time interaction in a standard web browser."
	Pro-tips: Goal: If the first version isn't perfect, use these follow-up prompts: 
		Prompt 2 (Refining Physics): "Make the strings look more like glowing laser beams and 
		add a 'particle' explosion effect whenever the fingertips of both hands touch. 
		(Refining Style): "clean up the UI. Hide the raw video feed but keep the hand silhouettes 
		visible and make the background a deep midnight blue with a subtle CRT scanline overlay. 

