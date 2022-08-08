# Unity 4.6.1

https://unity3d.com/unity/whats-new/unity-4.6.1

## Improvements



*   AssetBundles: Added additional information about WWW.LoadFromCacheOrDownload.
*   Graphics: Improved performance when allocating memory for large numbers of temporary objects.
*   Graphics: Optimized culling of lights in a mostly deferred scene with a few forward-rendered objects.
*   Physics 2D: Added 'Static Collider Shapes' to profiler for 2D physics.
*   Physics 2D: Renamed Physics2D.deleteStopsCallbacks to Physics.changeStopsCallbacks to better represent its purpose (old property is now obsolete).
*   Serialization: Randomize fileIDs for objects in prefabs to lower the chance of merge conflicts.
*   UI: Encapsulate children mesh bounds when calculating Root Bounds. Also cache the value so we don't calculate every time we draw.
*   UI: Performance optimizations. Optimized UI batching, text rendering and reduced amount of editor-only allocations.
*   UI: Standalone input module now leaves keyboard selected object selected. Mouse and Keyboard input are now orthogonal. Clicking with the mouse will move selection to the clicked element.
*   Windows Phone/Store Apps: Profiler shows managed memory usage.
*   Windows Phone/Store Apps: Provide ArrayList.BinarySearch implementation.
*   Windows Standalone: You can now embed windows standalone player into another application, simply pass -parentHWND and windows standalone application's window will be created with specified parent. See Command line arguments documentation for more information.