# Unity 5.0

https://unity3d.com/unity/whats-new/unity-5.0

## Known issues



*   New Substance features introduced by Substance Designer 5.0 are not yet supported inside Unity.
*   On Windows 7, system dialog (File Open/File save) and homescreen/project launcher window, the editor in the background doesn't redraw properly when the window is dragged around
*   WebGL: If you set up a UI Event to trigger a method on a class which is not a MonoBehaviour, and that method is not invoked elsewhere from your code, then the method may be stripped, and the event will fail. The workaround is to explicitly call the method in some place in your code to make sure it won't be stripped.
*   Windows Player: -parentHWND doesn't work (will return in patch release).
*   Enabling GPU panel in profiler, and stopping or closing the profiler, will result in the editor almost stalling while printing many error messages. A workaround is to close the GPU panel before closing or stopping the profiler. Will be fixed in patch release
*   Animation :Copy/Pasting States or StateMachines will not copy it’s StateMachineBehaviours they will be shared between the copies. Will be fixed in patch release.
*   Animation: Panning with alt-click does not work in the BlendTree graph. Will be fixed in patch release.