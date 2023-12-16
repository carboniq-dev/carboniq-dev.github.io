# Epilogue

**How does the performance of TrailBlazer compare to Unreal Engine's native pathfinding?**

- TrailBlazer is optimized for {~~~>grid-based pathfinding~~} with a focus on customization. It performs exceptionally well in smaller to medium-sized environments. For very large landscapes, performance may vary, and it's recommended to adjust parameters like grid size and cell size for optimal performance.

**Can TrailBlazer be used for large open-world games?**

- While possible, TrailBlazer is ideally suited for smaller, more controlled environments. For large open-world games, careful consideration of grid size and cell count is necessary to balance performance.


**How are round objects handled in the pathfinding process?**

- The plugin incorporates a specific flag named {~~~>Use Max Precision~~} to enhance the handling of circular objects during pathfinding calculations. When this flag is enabled, the plugin takes into consideration the spherical attributes of objects.
- It's essential to point out that, for this flag to operate effectively, circular objects in your game world should be equipped with a sphere collision component. This component is utilized to accurately define the object's boundaries and facilitate path adjustments as needed.

**Is TrailBlazer suitable for dynamic environments?**

- TrailBlazer is capable of adapting to dynamic environmental changes. However, it's important to note that the grid is initially calculated on game start, and using it during gameplay could lead to blocking unless combined with a loading screen. Frequent recalculations in highly dynamic environments may also impact performance. Therefore, it's advisable to employ TrailBlazer in scenarios where environmental changes are less frequent or can be predictably managed.

**How does the plugin handle different terrain elevations or 3D environments?**

- TrailBlazer can adjust path heights to match terrain elevations if the {~~~>Adjust Path to Landscape Height~~} option is enabled. However, its primary strength is in 2D grid-based pathfinding.

**Can I customize the pathfinding algorithm?**

- Yes, TrailBlazer offers various customization options, including different heuristic calculations and the ability to include or exclude diagonal movements, among others.

**Is there support for path smoothing or avoiding sharp turns?**

- Yes, the plugin includes options for path smoothing and setting thresholds for turn angles, which can create more natural and visually appealing movement patterns.

**How does TrailBlazer handle obstacles?**

- At the beginning of the game, the plugin automatically detects obstacles within the grid. You can specify obstacle types and individual actors to be excluded from path calculations.

**Are there any limitations I should be aware of?**

- TrailBlazer is primarily designed for 2D grid-based pathfinding. While it offers functionality to adjust to 3D terrain, its application in complex 3D environments or highly vertical spaces might be limited. Additionally, very large grids can impact performance, so careful planning and testing are advised.
