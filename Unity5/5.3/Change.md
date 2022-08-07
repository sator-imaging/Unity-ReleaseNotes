# Unity 5.3
https://unity3d.com/unity/whats-new/unity-5.3

## Change

<ul>
<li>Android: Remove "Hide status bar" option in the Player Settings, now it is always hidden</li>
<li>Animation: Removed unsupported "Resample Rotation" options when importing animations in Legacy Mode</li>
<li>Deprecated: EditorApplication classNewScene,NewEmptyScene,OpenScene,OpenSceneAdditive, SaveScene,SaveCurrentSceneIfUserWantsTo,SaveCurrentSceneIfUserWantsToForce,currentScene,MarkSceneDirty,isSceneDirty and Application class levelCount,LoadLevel,LoadLevelAsync,LoadLevelAdditive,LoadLevelAdditiveAsync,loadedLevel, loadedLevelName APIs. They all redirect to equivalent APIs on EditorSceneManager or SceneManager but it is recommended to start using the new APIs instead.</li>
<li>Editor: Don't show disabled context button for assets without a context menu</li>
<li>Editor: EditorGUIUtility.RenderGameViewCameras() marked obsolete. It was poorly designed API, and it appears nobody uses it anyway. We'll give it at least one minor release until we remove it entirely, in order to see if anyone is actually using it.</li>
<li>Editor: Screen.lockCursor will not be reset when clicking with mouse</li>
<li>Graphics: OpenGL core (3.2 - 4.1) API is used by default on Mac OS X and Linux now.</li>
<li>iOS: Use launch screens as primary source for splash images</li>
<li>Particles: Enable dynamic collisions checkbox by default</li>
<li>Particles: Setting playOnAwake through script will now change all systems that are part of the emitter, matches the inspectors behaviour.</li>
<li>Physics: 2D physics (Box2D) now reports out-of-memory errors rather than simply crashing.</li>
<li>Physics: Added PlatformEffector2D.sideArc to replace PlatformEffector2D.sideAngleVariance as well as adding the missing gizmo for sides</li>
<li>Physics: Allow the PhysX CharacterController to consider the slope limit for Rigidbodies. This fixes bugs where the CharacterController could climb on very steep slopes on Rigidbodies. Restores Unity4 behavior.</li>
<li>Physics: Restore the Rigidbody2D linear-velocity after a Rigidbody2D.MovePosition has completed.</li>
<li>Physics: Setting Rigidbody.detectCollisions to false also affects queries now (e.g. Physics.RaycastAll)</li>
<li>Terrain: "SplatCount" tag is removed from terrain shaders as it doesn't serve any purpose..</li>
<li>UI: Updated function names to be more consistent with other classes</li>
<li>Windows Store Apps/Windows Phone 8: Removed support for Windows Phone 8.0 and Windows Store Apps 8.0</li>
<li>Windows Store Apps: Removed AppCallbacks.SetSwapChainBackgroundPanel function</li>
<li>Windows Store: all managed plugins and WinMD files always target AnyCPU architecture. This essentially means that you no longer need to have separate wrapper DLL and winmd files for each native plugin you have.</li>
</ul>
