# Ex.No: 4  Create a player Movement Script in unity 
### DATE:17/03/2025                                                                            
### REGISTER NUMBER : 212224230057
### AIM: 
To write a program to create a player movement in unity.
### Algorithm:
1. Create a New Unity Project by Open the  Unity Hub and create a new 3D Project,Name the project (e.g., PlayerMovement).
2. Create the Moving Object
   In the Hierarchy, right-click → 3D Object → Capsule (or Sphere).
   Rename it to Player 
4. Adding the Player Movement Behavior Script
   Create the Script-In the Project Window, go to the Assets folder.
   Right-click → Create → C# Script.
5. Write a script for player behavior and save it
6. Attach the Script
   Select player in the Hierarchy - Drag & Drop the playerBehavior script onto the Inspector Panel.
7. Run the game 
8. Stop the program
    
### Program:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Player_movement : MonoBehaviour
{
    // Start is called before the first frame update
    public float speed;
    void Start()
    {
    }

    // Update is called once per frame
    void Update()
    {
       float xdir = Input.GetAxis("Horizontal") * speed;
      float zdir = Input.GetAxis("Vertical") * speed;
      transform.position+=new Vector3(xdir, zdir); 
    }
}

```
### Output:

![Screenshot 2025-03-17 143414](https://github.com/user-attachments/assets/4b176942-38d6-44e3-83b0-45fb2e34afa8)








### Result:
Thus the simple movement behavior was implemented successfully.
