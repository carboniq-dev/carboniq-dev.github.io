# Examples

=== "Showcases"

    !!! example "1. Pathfinding on a maze"
        ![example_1](../assets/images/trail-blazer/example_1.PNG){ width="200" }

    !!! example "2. Pathfinding on large maze (Maxed out)"
        Landscape settings

        ![example_8](../assets/images/trail-blazer/example_8_2.PNG){ width="100" }

        Grid settings

        ![example_8](../assets/images/trail-blazer/example_8_3.PNG){ width="100" }

        Maze

        ![example_8](../assets/images/trail-blazer/example_8.PNG){ width="200" }

    !!! example "3. Pathfinding on stairs"
        ![example_4](../assets/images/trail-blazer/example_4.PNG){ width="200" }

    !!! example "4. Handling multiple elevated landscapes"
        ![example_7](../assets/images/trail-blazer/example_7.PNG){ width="200" }

    !!! example "5. Ingoring specific obstacles for detection and/or height adjustments"
        ![example_3](../assets/images/trail-blazer/example_3.PNG){ width="200" }

=== "Edge cases"

    These scenarios go beyond what this plugin was originally designed for. However, with the options for spherical and rectangular precision, you can adapt it to handle some unique situations. But remember, these adjustments come with a trade-off: longer load times. It's particularly important to be mindful when you're expanding the grid size while also shrinking the cell size to a smaller dimension. Doing so can lead to significantly longer load times, especially when you're working with rectangular precision. The reason behind this is the complex way the system calculates obstructions. There's a noticeable difference in how it processes objects that are rotated versus those aligned with the grid's orientation. Each requires a specific method in their calculation, adding to the complexity and load time.

    !!! Note
        The current limitations are recognized, and there are plans for future optimization. This will aim to streamline these functionalities and incorporate them seamlessly as a feature of the plugin. Stay tuned for updates!

    !!! example "8. Obstacles rotation not aligned with grid"
        ![example_2](../assets/images/trail-blazer/example_2.PNG){ width="200" }

    !!! example "9. Spherical obstacles detection"
        ![example_5](../assets/images/trail-blazer/example_5.PNG){ width="200" }

=== "Heuristic Types"

    Chebyshev

    ![chebyshev](../assets/images/trail-blazer/heuristic/chebyshev.PNG){ width="200" }

    Euclidean

    ![euclidean](../assets/images/trail-blazer/heuristic/euclidean.PNG){ width="200" }

    Euclidean Weighted

    ![euclidean_weighted](../assets/images/trail-blazer/heuristic/euclidean_weighted.PNG){ width="200" }

    Manhatten

    ![manhatten](../assets/images/trail-blazer/heuristic/manhatten.PNG){ width="200" }

    Tie Breaking Euclidean

    ![tieBreakingEuclidean](../assets/images/trail-blazer/heuristic/tieBreakingEuclidean.PNG){ width="200" }

=== "Pathfinding Settings"

    90 Degrees Turns

    ![sharp_turns](../assets/images/trail-blazer/settings/sharp_turns.PNG){ width="200" }

    Diagonals

    ![diagonals](../assets/images/trail-blazer/settings/diagonals.PNG){ width="200" }

    No Buffer

    ![no_buffer](../assets/images/trail-blazer/settings/no_buffer.PNG){ width="200" }

    Buffer

    ![buffer](../assets/images/trail-blazer/settings/buffer.PNG){ width="200" }

    Sharp Turns

    ![no_smooth](../assets/images/trail-blazer/settings/no_smooth.PNG){ width="200" }

    Smooth Turns

    ![smooth](../assets/images/trail-blazer/settings/smooth.PNG){ width="200" }