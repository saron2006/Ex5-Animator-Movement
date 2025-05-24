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

## Program :

### DEVELOPED BY : SARON XAVIER A
### REG NO : 212223230197

## PlayerController:


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

![image](https://github.com/user-attachments/assets/65882d4f-746f-480b-9962-d6f8cbe28191)

![image](https://github.com/user-attachments/assets/b7125da1-7842-42f7-a709-28ee8ff3925c)

![image](https://github.com/user-attachments/assets/029ebd15-4d9e-445b-b706-5437d5613ea4)



## Result :

Thus, An animator movement for a player using unity is developed successfully.
