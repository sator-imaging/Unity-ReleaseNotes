# Unity 2018.3

https://unity3d.com/unity/whats-new/unity-2018.3.0

## Changes



*   Android: Disabled Android TV by default for new projects.
    
*   Build Pipeline: If you call `BuildPipeline.BuildPlayer` while Unity is compiling scripts, Unity now completes compilation before beginning the build process, rather than aborting compilation.
    
*   Editor: Removed undocumented behavior where pressing the F key twice in rapid succession would execute **Edit** > **Lock View to Selected** instead of **Edit** > **Frame Selected**.
    
*   iOS: Marked Mono scripting backend as deprecated.
    
*   iOS: Unity now distributes iOS and tvOS Simulator players as dynamic libraries (dylib).
    
*   Particles: It is now possible to flip a percentage of mesh particles, in the same way that was previously only possible with billboards.
    
*   Particles: The Unlit Particle Standard Shader is now applied by default when creating new Particle Systems.
    
*   Windows: The Vulkan editor support on Windows and Linux is no longer experimental. Removed the "Enable Vulkan editor support" checkbox.