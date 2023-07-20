# Harvard-University-course-CS50-project-at-Scratch
Harvard University's online course CS50: Introduction to Computer Science offers an intellectual journey into the realms of computer science and the art of programming. Through creating my first project on Scratch, I discovered the boundless potential of technology. Join this magical programming experience and unleash your full potential with CS50!

A  step-by-step guide for creating the "Solar Adventure" project in Scratch, following the beginner's perspective:

Step 1: Open Scratch
- Open Scratch on your computer or visit the Scratch website (scratch.mit.edu).

Step 2: Create a New Project
- Click on "Create" to start a new Scratch project.

Step 3: Choose Sprites
- Remove the default cat sprite by right-clicking on it and selecting "Delete."
- Click on the "Choose a Sprite from Library" button below the stage.
- In the sprite library, select two sprites of your choice (not a cat or an astronaut sprite). You can use the search bar to find them easily.

Step 4: Customize the Sprites
- Click on each sprite to select it.
- In the sprite costume section, click on the "Costumes" tab.
- Choose a costume for each sprite from the options provided.

Step 5: Create a Custom Block
- Click on the "Make a Block" button in the Blocks palette.
- Name the block as "flyForward" and specify a single parameter, "distance."
- Drag and snap together the blocks to create the custom block:
   ```
   move (distance) steps
   ```

Step 6: Script for Spaceship Sprite - Script 1
- Select the spaceship sprite.
- Click on the "Events" category in the Blocks palette and drag the "when green flag clicked" block to the Scripts area.
- From the "Control" category, drag and snap the following blocks inside the "when green flag clicked" block:
   - `if <touching [Planet v]?> then`
      - `say "Mission Success!" for 2 seconds`
   - `else`
      - `if <key [up arrow] pressed?> then`
         - `flyForward(10)`
      - `end`
      - `if <key [right arrow] pressed?> then`
         - `turn cw (15) degrees`
      - `end`
      - `if <key [left arrow] pressed?> then`
         - `turn ccw (15) degrees`
      - `end`
   - `end`

Step 7: Script for Spaceship Sprite - Script 2
- Click on the spaceship sprite to select it.
- Drag and snap the following blocks below the existing script:
   - `when green flag clicked`
   - `set [x velocity v] to (0)`
   - `set [y velocity v] to (0)`
   - `set [speed v] to (3)`
   - `forever`
      - `if <key [up arrow] pressed?> then`
         - `change [y velocity v] by (speed)`
      - `end`
      - `if <key [down arrow] pressed?> then`
         - `change [y velocity v] by (-speed)`
      - `end`
      - `if <key [right arrow] pressed?> then`
         - `change [x velocity v] by (speed)`
      - `end`
      - `if <key [left arrow] pressed?> then`
         - `change [x velocity v] by (-speed)`
      - `end`
      - `glide [0.1] secs to x: (x position) + (x velocity) y: (y position) + (y velocity)`
   - `end`

Step 8: Script for Planet Sprite
- Click on the planet sprite to select it.
- Drag and snap the following blocks:
   - `when green flag clicked`
   - `forever`
      - `turn cw (1) degree`
   - `end`

Step 9: Run the Project
- Click on the green flag above the stage to run the project.
- Control the spaceship sprite using the arrow keys.
- If the spaceship sprite touches the planet sprite, it will display the "Mission Success!" message.

  My Project Link is as under:
  https://scratch.mit.edu/projects/875043608/editor/
  
