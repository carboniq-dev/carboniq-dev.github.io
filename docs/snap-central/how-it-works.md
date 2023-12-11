# How it works

To use the plugin, simply search the <mark>CentralGrid</mark> actor in the _Place Actors_ tab, add it to your world and obtain a reference to it. The actor provides a function called <mark>GetSnapParameters</mark>, which can be called to handle line tracing, finding the closest snap location, and handling visualizations. To use the function, pass an actor or camera component to it, and the plugin will take care of the rest.

If necessary, you can also pass a vector to the TargetLocation pin and handle the logic yourself. This may be required in cases where complex character movements or actions are involved, such as jumping off cliffs while snap dragging along floating planes.

Overall, the CentralGrid actor and its associated function provide a convenient and efficient way to implement snapping and grid-based movement in your Unreal project, while also offering flexibility and control for more complex scenarios.
