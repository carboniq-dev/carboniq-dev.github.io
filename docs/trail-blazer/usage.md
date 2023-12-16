# Usage

## Setup

To get started, open the actor you wish to have control over the pathfinding feature. Obtain a reference to the **TrailBlazerGrid_BP** previously placed in the world. Drag out from the output pin and bind the **On Path Calculated** event. Afterward, drag out again and search for the **Find Path Async** function.
Specify the start and end locations. Please note that the locations must be within the grid. 
Connect the nodes as illustrated below.

![Get Path Locations](../assets/images/trail-blazer/custom-setup-1.PNG){ width="800" }

## Recommended

!!! Warning

    Cameras and pawns hovering within the obstacle detection range on game start will also be detected as obstacles, potentially preventing a path from being found. In such cases, they should be explicitly excluded in the obstacles section to avoid this issue.

- Fine-tune the grid size and cell size based on your environment’s scale and complexity.
- Use appropriate heuristic calculations based on your game’s requirements.
- Regularly profile and monitor performance, especially in larger or more complex environments.

### Showcase

!!! Maze Example
    Showcases pathfinding through a rather complicated maze.

| Property                 | Value    |
| ------------------------ | ------- |
| Cell Size| 20 |
| Num Columns | 300 |
| Num Rows | 300 |
| Include Diagonals | True |
| Add Cell Buffer | True |
| Buffer Distance | 2 |

![Get Path Locations](../assets/images/trail-blazer/example.PNG)
