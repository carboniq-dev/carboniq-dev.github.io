# Usage

## Quickstart

I've prepared an initial blueprint setup that demonstrates the intended usage of the TrailBlazer plugin. Begin by adding the **TrailBlazerGrid_BP**, **TrailBlazerStarter_BP**, and two **TrailBlazer_Debug_StartEndIndicator_BP** blueprints to your world. Next, select the placed TrailBlazerStarter_BP and configure either the start/end actor or the start/end location. To initiate the pathfinding process, press the play button and left-click in your world.

## Custom Setup

To get started, open the actor you wish to have control over the pathfinding feature. Obtain a reference to the **TrailBlazerGrid_BP** previously placed in the world. Drag out from the output pin and bind the **On Path Calculated** event. Afterward, drag out again and search for the **Find Path Async** function.
Specify the start and end locations. Please note that the locations must be within the grid.
Connect the nodes as illustrated below.

![Get Path Locations](../assets/images/trail-blazer/custom-setup-1.PNG){ width="800" }
