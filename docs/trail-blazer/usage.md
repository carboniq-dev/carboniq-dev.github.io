# Usage

!!! Tip
    If you don't see the plugin content described in the documentation, be sure to either enable the option to display plugin content or navigate to the TrailBlazer plugin folder itself.

## Quickstart

I've prepared an initial blueprint setup that demonstrates the intended usage of the TrailBlazer plugin. Begin by adding the **TrailBlazerGrid_BP**, **TrailBlazerStarter_BP**, and two **TrailBlazer_Debug_StartEndIndicator_BP** blueprints to your world. Next, select the placed TrailBlazerStarter_BP and configure either the start/end actor or the start/end location. To initiate the pathfinding process, press the play button and left-click in your world.

## Custom Setup

To get started, open the actor you wish to have control over the pathfinding feature. Obtain a reference to the **TrailBlazerGrid_BP** previously placed in the world. Drag out from the output pin and bind the **On Path Calculated** event. Afterward, drag out again and search for the **Find Path Async** function.
Specify the start and end locations. Please note that the locations must be within the grid.
Connect the nodes as illustrated below.

![Get Path Locations](../assets/images/trail-blazer/custom-setup-1.PNG){ width="800" }

## Guidelines

The plugin's pathfinding settings offer a wide range of customization options that can significantly impact the calculation of paths. In edge cases or scenarios beyond the recommended usage, it becomes crucial to carefully adjust and experiment with these settings. It's important to note that these settings can have interdependencies, meaning changes to one setting may affect others.

- Fine-tune the grid size and cell size based on your environment’s scale and complexity.
- Use appropriate heuristic calculations based on your game’s requirements.
- In case a path is not detected, consider utilizing the precision options.

!!! Warning

    Cameras and pawns hovering within the obstacle detection range on game start will be detected as obstacles, potentially preventing a path from being found. In such cases, they should be explicitly excluded in the obstacles section to avoid this issue.


### Showcase

#### Maze

| Property                 | Value    |
| ------------------------ | ------- |
| Cell Size| 20 |
| Num Columns | 300 |
| Num Rows | 300 |
| Include Diagonals | True |
| Add Cell Buffer | True |
| Buffer Distance | 2 |

![Get Path Locations](../assets/images/trail-blazer/example.PNG)
