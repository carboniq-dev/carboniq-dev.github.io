# Epilogue

**How does the performance of TrailBlazer compare to Unreal Engine's native pathfinding?**

- TrailBlazer is optimized for {==grid-based pathfinding==} with a focus on customization. It performs exceptionally well in smaller to medium-sized environments. For very large landscapes, performance may vary, and it's recommended to adjust parameters like grid size and cell size for optimal performance.

**Why do I sometimes not receive path locations on certain maps and configurations?**

!!! Note
    There can be several reasons for this issue. It's important to note that the availability of a path can be influenced by various settings. To address this, consider the following steps.

- {==Adjust Cell Size==}: In tight or constrained spaces, the default cell size might not be suitable for generating paths. Try changing the cell size to better fit the specific environment.

- {==Heuristic Calculation==}: Experiment with different heuristic calculation methods. The choice of heuristic can impact the pathfinding results significantly, so finding the right one for your scenario is important.

- {==Use Sperical Precision / Use Rotation Precision==}: If you encounter difficulties navigating around circular or rotated objects within confined spaces, you may want to consider enabling these parameters, which incorporate spherical and rotated objects into the object detection process.

- {==Explore Plugin Options==}: Explore additional options exposed by the plugin that can affect pathfinding behavior.

**Is TrailBlazer suitable for dynamic environments?**

- While TrailBlazer is not primarily intended for dynamic environments, it can be utilized in specific scenarios where dynamic elements are involved, but it's important to use it at your own discretion and risk. The plugin's optimal performance is typically seen in more static or contained environments, so implementing it in highly dynamic settings may require additional considerations and testing to ensure desired results.

- Additionally, when dealing with dynamic environments, one will need to facilitate the **Initialize Grid** function to reinitialize the grid as needed. It's worth noting that debug functions are wrapped in the TrailBlazerGrid_BP blueprint, so you will need to reconstruct it or copy-paste the existing functionality.

**How does the plugin handle different terrain elevations or 3D environments?**

- TrailBlazer can adjust path heights to match terrain elevations if the {==Adjust Path to Landscape Height==} option is enabled. However, its primary strength is in 2D grid-based pathfinding.

**Can I customize the pathfinding algorithm?**

- Yes, TrailBlazer offers various customization options, including different heuristic calculations and the ability to include or exclude diagonal movements, among others.

**Is there support for path smoothing or avoiding sharp turns?**

- Yes, the plugin includes options for path smoothing and setting thresholds for turn angles, which can create more natural and visually appealing movement patterns.

**How does TrailBlazer handle obstacles?**

- At the beginning of the game, the plugin automatically detects obstacles within the grid. You can specify obstacle types and individual actors to be excluded from path calculations.

**Are there any limitations I should be aware of?**

- TrailBlazer is primarily designed for 2D grid-based pathfinding. While it offers functionality to adjust to 3D terrain, its application in complex 3D environments or highly vertical spaces might be limited. Additionally, very large grids can impact performance, so careful planning and testing are advised.
