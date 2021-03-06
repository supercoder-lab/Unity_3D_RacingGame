### Day 3 Lesson Plan

Today we will be adding enemy players, enemy navigation, implementing a game menu, and writing scripts for a finish line.

### Steps

1. Adding a finish line to your track.
  - Create a new 3D game object **cube**
  - Move **cube** to one end of your track. Transform the cube so that its flat and spans the width of your finish line.
  
 ![](http://i.imgur.com/KyEA159.png)
 - In your **inpector** window under **Box Collider**, make sure that **is Trigger** is checked.
 - Edit your Collider perimeter **Instructor will show you this**.
 
2. Adding functionality to your finish line.
 - **Stop Here** 
 - Instructors live code **Finish line** script found in repo wiki. 
 - Test that script displays Debug Log when car passes through the finish line.
 
 3. Adding Enemy Cars.
    - In your **Hierarchy** window, right-click on player and select **duplicate**. Rename this car **Enemy**.
    - Create a new material and apply to enemy player.
    
 4. Adding Navigation for Enemy Cars.
  - **Instructors will live code NavBake** - refer to Wiki on how to nav bake.
  - With your Enemy player selected, navigate to **inspector** window and click **add Component**. Search for **nav mesh agent** and click ok.
  - **Instructors live-code Nav Script** - refer to wiki in repo for code.
  - Set **destination** on Nav Script to **FinishLine**. This will help the enemy player navigate towards the finish line.
  **Stop Here**- Run game and check that Nav script is working for enemy car.
  
 5. Adding a restart menu. 
    - Navigate to **file => new scene**, name this scene **restart**
    - Navigate to **GameObject => UI => Canvas**. This should add a **canvas** to your hierarchy window. In the same menu, add a **UI Button** and drop and drag button so that its a child element of **Canvas**.
    - Select **button** and in inspector window you should see some cross-hairs. Click on the icon, then press **shift** on your keyboard and look for the icon that will center the button on the UI.
    - Under **button** their is a child element **Text**, click this and change the text so that it says **Restart Game**.
    
    **KNOWN ISSUES TO CHECK IF DEBUG LOG NOT SHOWING UP IN CONSOLE**
      - Script Names must be camelCase and match the object name completely.
      - Make Collider Body on player object have the a tag of "player".
      - Make sure that box collider component on finishline object is selected.
      - Make sure mesh collider component on finishline object is deselected.
      - Check script for sytax/spelling errors.
 
 6. **Stop Here** - instructors live code restart script for button.
 
 7. Making the Game Menu Function.
    - Navigate to **file => build settings**, drag and drop **Scene1 & restart** into window. Then exit settings.
    - Open back up **Scene1** and run your game. Now when you cross the finish line, a game button will appear and start your game over again.
    
    **Note**
      - After restarting the game, the game lighting will appear to be darker than normal. This is okay, its a bug with the unity editor. When the game is actually built, the lighting issue will not be there.
 
 **END**
