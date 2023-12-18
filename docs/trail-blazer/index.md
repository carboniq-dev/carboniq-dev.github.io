# Introduction

!!! Note
    This plugin is currently undergoing the review process by Epic Games.

![Get Snap Parameters](../assets/images/trail-blazer/trail-blazer-cover.png){ width="200" }

TrailBlazer is a dedicated plugin crafted for {==grid-based pathfinding==}, offering a valuable option for projects requiring accurate and adaptable navigation solutions {==where objects are aligned with the grid cells rotation==}. While its primary strength lies in {==2D grid-based pathfinding==}, it also offers an option to consider landscape height along the z-axis. This plugin is particularly well-suited for puzzle games, mazes, and game environments of small to medium size.

TrailBlazer is focused on specific scenarios where grid-based navigation is the preferred approach. While it does provide capabilities for larger landscapes, it performs optimally in more contained environments. You can take advantage of various adjustable settings such as grid size, cell dimensions, obstacle detection options and heuristic methods to fine-tune navigation and tailor it to the unique requirements of your game.

!!! Info "Trailblazer vs UE pathfinding tools"
    This {==grid-based==} plugin is {==not==} intended to replace Unreal Engine's built-in pathfinding tools. It is tailored for developers who require complete control over all path locations and intricate navigation scenarios within a grid-based environment. It is not ideally suited for highly complex landscapes and environments.

!!! Warning "Handling complex environments"
    To enhance the flexibility of pathfinding in unusual situations, I've introduced additional settings that influence obstacle detection. These settings allow for the detection of circular objects (provided they have a sphere collision) and rotated rectangular objects that don't align with the grid.

    {==It's important to note that these settings should primarily be reserved for edge cases, confined spaces, or complex scenarios where no path is found.==}
