# Unity 2017.4.2f2
https://unity3d.com/unity/whatsnew/unity-2017.4.2

## Fixes

<ul>
<li>(1016640) - Android: Fixed apk signer v2 being used when building Oculus apps with gradle.</li>
<li>(1014623) - Android: Fixed incorrectly including files to noCompress when their extensions are already included by default.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/935077/">986780</a>) - Android: Disabled warnings in ProGuard by default; fixes build errors with 3rd party plugins.</li>
<li>(1009641) - Asset Bundles: Fixed crash when building Asset Bundles.</li>
<li>(1008371) 1006573 - Core: Fixed a regression in memory usage at startup in Editor and Player.</li>
<li>(975341) 956741 - DirectX 12: Fixed Standalone crashing when using DestroyImmediate on a Texture2D when graphics jobs are enabled.</li>
<li>(1014167) - Editor: Fixed starting Unity from the Unity Hub disables File menu and other key bindings.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/966404/">966404</a>) - Editor: Fixed Editor crashes in "RenderSelectionOutline" when using ImageEffectAllowedInSceneView and set camera's targetTexture to null.</li>
<li>(1016691) 978204 - Editor: Fixed opening project in editor causing newly spawn instance to get stalled/suspended.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/963576/">963576</a>) - Graphics: Fixed objects using HideAndDontSave being visible in preview windows, after being disabled and enabled.</li>
<li>(1009868) - Graphics: Fixed Tangents on the LineRenderer, which would cause Normal Maps to look incorrect.</li>
<li>(1021655) - Graphics: Fixed occasional graphical corruption when using marquee selection on dynamic geometry, such as Lines, Particles and Trails.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1017529/">1017529</a>) - Graphics: Fixed LineRenderer scripting bug where start/end width would sometimes not update correctly if set from script.</li>
<li>(1019586) - IL2CPP: Prevented an error during code conversion related to a missing RGCTX entry for type T that can occur with an unbox opcode for a nullable type.</li>
<li>(1021529) 1013634  iOS: Fixed showing both orientation custom Launch Images on Landscape orientation.</li>
<li>(1016731) 991204 - iOS: Fixed build failing with error "DXT1 compressed textures are not supported when publishing to iPhone".</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/967197/">967197</a>) - iOS: Fixed an audio crash when moving an app to the background, and back to the foreground.</li>
<li>(947049) - Linux: Fixed Linux touch input for mouse events.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/978602/">978602</a>) - Mobile: Fixed screen flicker when launching Handheld.PlayFullScreenMovie.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1008385/">1008385</a>) - Multiplayer: Fixed editor crashing in AddWebsocketHost on a second instance using the same port.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006947/">1006947</a>) - Particles: Improved Dynamic Batching when systems with 0 particles exist in the scene.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1013161/">1013161</a>) - Particles: Fixed Rate Over Distance script setter property.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006435/">1006435</a>) - Particles: Fixed crash in AnimationCurveTpl::Evaluate when setting XYZ curves to mismatched modes via script.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/994938/">994938</a>) - Particles: Fixed rare case where bounding boxes could be incorrect on procedural systems.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/998680/">998680</a>) - Particles: Fixed invalid bounding box errors when using scripted emission.</li>
<li>(976785) - PS Vita: Fixed video sample project so it correctly initialises the render texture before playing a video, and cleaned up some error and warning messages.</li>
<li>(991010) 981757 - Scripting: Fixed crash on the .NET backend when calling Unity APIs that take structs with with bool fields.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011626/">1011626</a>) - Scripting: Fixed crash when taking memory snapshot.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989777/">989777</a>) - Shaders: Fixed GLSL TranslateVariableNameWithMask() printing a swizzle on a wrong place.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/919351/">919351</a>) - Shaders: Fixed an issue with the Shader Compiler which would result in GLSL based platforms not being able to compiler certain shaders.</li>
<li>(1006986) - Timeline: Fixed Copy/Paste between Timelines causing Groups Tracks to have incorrect parent.</li>
<li>(986040) 972997 - Video: Fixed flickering video playback on iOS/Metal.</li>
<li>(1017468) 976010 - WebRequest: Fixed crash when aborting AssetBundle download using UnityWebRequest.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/998331/">998331</a>) - XR: Fixed XR.WSA.WorldManager.OnPositionalLocatorStateChanged() not getting called when state changes back to active.</li>
</ul>

#### Revision: 52d9cb89b362
