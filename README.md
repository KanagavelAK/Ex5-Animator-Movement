# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

# Program :
```
DEVELOPED BY : Kanagavel A K
REG NO : 212223230096
```
# PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent <Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}


```
## Output :
![image](https://github.com/user-attachments/assets/b06d79eb-585c-4167-aa46-9edc1f18f592)
![image](https://github.com/user-attachments/assets/eabd0ebf-d100-4098-88e0-03dcaab69054)
![image](https://github.com/user-attachments/assets/c47727e5-b777-42ee-9826-174a4bf3ef44)



## Result :

Thus, An animator movement for a player using unity is developed successfully.
