# FAQ

**Is it possible to use the plugin to snap to actors?**

- The short answer is no. The snap locations always refer to the grid. However, by selecting _HitLocation_ as the **Snap Type**, it is possible to snap along the Z-axis on any actor. With additional logic, achieving actor snapping should be feasible.

**Why is the snap location jumping when I try to snap underneath an actor like a bridge?**

- If this happens, it is likely that the line trace hit the above actor first, causing the plugin to take it as the reference for calculating the snap location. To avoid this issue, you can adjust the **Line Trace Height** property by decreasing its value, or add specific actors that should not be considered to the **Ignore Actors For Line Traces** array. In addition, you can enable debugging visuals to make it easier to spot issues.

**Why is the snap location elevated when I use the plugin on my custom landscape?**

- This issue can occur if the scale of the Z-axis doesn't match the original scale. To prevent any displacement issues, it's important to ensure that the scaling values in the software used for creating landscape geometry are accurate. In most cases, export information is displayed that shows the scaling values.

!!! Tip

    When exporting a height map for use in Unreal Engine, it's recommended to check the export options and ensure that the height map is exported as PNG 16-bit.

**Why are my custom materials not applied correctly?**

- The visuals for the grid are decal actors and require materials with their domain set to _Deferred Decal_.

!!! Tip

    It's important to note that if you want to reproduce the grid lines, you'll need to take the Tile Size into account. By doing so, you can ensure that the grid lines align properly with the rest of the grid.
