# **Neon Snake & Apple Game**
Neon Snake &amp; Apple reimagines the classic game for both nostalgic players and a new generation. 

# **Executive Summary**

"Neon Snake & Apple" reimagines the classic game for both nostalgic players and a new generation. This vibrant HTML5 game offers addictive gameplay with a stunning neon design. Players navigate a growing snake through a grid, consuming apples to score while avoiding collisions. With multiple game modes, adjustable difficulty, and various power-ups, it provides a polished and engaging experience. The game features responsive design, intuitive controls, and persistent high-score tracking, making it highly replayable.

# **Technical Summary**

"Neon Snake & Apple" is a well-organised, single-file web application developed using vanilla HTML, CSS, and JavaScript. It employs the HTML5 Canvas API for rendering all gameplay elements and uses local storage for data persistence. The codebase is structured in a clear, class-based format that encapsulates game logic and state management, making it both maintainable and scalable.

#### 

## **Core Features**

* **Dual Game Modes:** Players can choose between "Classic" mode, where colliding with walls ends the game, and "Wrapping" mode, where the snake teleports from one edge of the screen to the other.  
* **Adjustable Difficulty:** Three difficulty settings (Easy, Medium, Hard) modify the game's speed and the probability of special items appearing, catering to players of all skill levels.  
* **Dynamic Power-Up System:** The game includes a variety of apples beyond the standard red one:  
  * **Golden Apples:** Grant an extra life.  
  * **Special Apples:** Provide a temporary speed boost and bonus points.  
  * **Poison Apples:** Decrease the player's score, reduce speed, and cost a life.  
* **Progressive Levelling:** The game features a level-up system tied to the number of apples eaten, which progressively increases the snake's speed and the game's challenge.  
* **Persistent High Scores:** A local high-score board tracks the top 10 scores, prompting users for their initials and saving the data using the browser's localStorage API.  
* **Responsive & Accessible Controls:** The game is fully playable on both desktop and mobile devices, featuring on-screen touch buttons for mobile and keyboard arrow keys for desktop users.  
* **Comprehensive UI:** The interface includes a start screen, rules display, pause menu, level-up notifications, and a game-over screen, providing a complete and user-friendly experience.

#### 

## **Technical Highlights**

* **Object-Oriented Design:** The core game logic is encapsulated within a SnakeGame JavaScript class, which manages state variables such as the snake's position, score, lives, level, and game-over status. This approach promotes clean, organised, and reusable code.  
* **Canvas Rendering Engine:** All game graphics, including the grid, snake, and various apples, are dynamically drawn on an HTML5 \<canvas\> element. The rendering loop is efficiently managed to produce smooth animations.  
* **Stateful Game Loop:** The game's progression is controlled by an setInterval function that serves as the main game loop. The interval's timing is dynamically adjusted based on the game's current speed, which changes with difficulty and level progression.  
* **Collision Detection Logic:** The game implements robust collision detection algorithms to check for interactions between the snake's head and the canvas boundaries, its body segments, and all types of apple objects.  
* **DOM Manipulation for UI:** The user interface elements (score display, lives, menus) are standard HTML elements that are dynamically updated via JavaScript to reflect the current game state in real-time.  
* **Responsive CSS:** The user interface is styled with CSS that includes media queries and flexible box layouts to ensure a consistent and playable experience across various screen sizes, from mobile phones to desktop monitors.  
* **Event-Driven Controls:** Player input is handled through keydown event listeners for keyboard controls and touchstart/click listeners for the on-screen buttons, ensuring immediate and responsive control over the snake's movement.

