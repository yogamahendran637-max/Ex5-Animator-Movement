# Ex5-Animator-Movement

## Aim:
To develop a animator movement for a player using unity.

## Algorithm:

Step 1:

Import necessary models.

Step 2:

Right-click -> Create -> Animator Controller.

Step 3:

Open Animator window, define states (Idle, Run, Jump, etc.).

Step 4:

Use keyframes or Unity's Animation tools to animate transitions between states.

Step 5:

Drag Animator Controller to the GameObject in the Inspector.


# Program:
```
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputX", InputX);
        animator.SetFloat("InputY", InputY);
    }
}

```



## Output:





<img width="1919" height="1070" alt="571718162-d25c8736-af78-4235-a8c2-299e292a7164" src="https://github.com/user-attachments/assets/e2c9001d-1bc0-49df-9565-510eb9c44f91" />


# Result:

An animator movement for a player using unity is developed successfully.







## Result:
