# Unity 2017.4.1f1
https://unity3d.com/unity/whatsnew/unity-2017.4.1

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1008942/">1008942</a>) - 2D: Fixed Tilemap not setting Tiles with the correct data in players with code stripping.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970038/">970038</a>) - Android: Fixed performance regression caused by compiler optimizing for size.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/978599/">978599</a>) - Android: Fixed unity pause during Android Handheld.PlayFullScreenMovie start.</li>
<li>(1013173 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970945">970945</a>)) - Android: Fixed Time.deltaTime sometimes returning negative value on certain devices/Android versions.</li>
<li>(1011573 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991127">991127</a>)) - Android: Fixed Cardboard VR fails to initialize on certain Android devices.</li>
<li>(992130 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/983938">983938</a>)) - Android: Fixed terrain shader to avoid crashing when calling glLinkProgram on Adreno 3xx.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970038/">970038</a>) - Android: Fixed performance regression of Render.Mesh in apps built with Gradle.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985786/">985786</a>) - Animation: Fixed an issue where scrubbing in the Animation Window would spam warning messages if some properties could not be found.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003190/">1003190</a>) - Animation: Fixed an issue where importing additional curves in a Legacy clip would crash.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1012200/">1012200</a>) - Asset Importing: Fixed ScriptedImporters such that SerializedProperty.objectReferenceValue can be set in the inspector.</li>
<li>(1013472 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1013071">1013071</a>)) - Asset Importing: Fixed crash when importing FBX with animated user properties in multiple animation clips.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991034/">991034</a>) - Audio: Fixed a bug where the matrices passed to spatializer and ambisonic audio plugins could be set to the identity matrix briefly when a sound starts playing.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/905161/">905161</a>) - Editor: Fixed various UnityEditor.VersionControl.Provider APIs when used with newly created VersionControl.Assets.</li>
<li>(1009686) - Editor: Fixed vsync not always off in scene view on macOS.</li>
<li>(None) - Editor: Fixed license activation issue when losing the network.</li>
<li>(1008764 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/921915">921915</a>)) - Editor: Fixed errors related to temp TLS allocations.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/952517/">952517</a>) - Editor: Fixed rare startup crash in BaseHierarchyProperty.</li>
<li>(None) - Editor: Fixed performance regression when Game View is visible while in play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/909987/">909987</a>) - Editor: Fixed m_CurrentEntriesPtr != NULL &amp;&amp; m_IsGettingEntries error thrown when double clicking on a specific warning.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/913869/">913869</a>) - GI: Fixed for LightingData.asset for multiple scenes baked together being vastly bigger than the sum of the sizes of those assets for scenes being baked separately. Enlighten probeset data was included multiple times.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996127/">996127</a>) - GI: Fixed realtime probes going black when unloading a scene that was a part of a multi-scene bake.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/957736/">957736</a>) - GI: Fixed realtime probes not working when loading scenes (that were baked together) additively.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980811/">980811</a>) - GI: Fixed errors on loading Enlighten probesets in the Editor after clearing the GI cache.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1000692/">1000692</a>) - GI: Fixed LoadDataTimeSliced working on the wrong scene mapping in the Editor.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/949117/">949117</a>) - GI: Fixed the "m_ProbeSetHashes.empty()" error occuring in certain projects when clearing the GI cache or when quitting the standalone.</li>
<li>(971907) - GI: Fixed duplicate GI light probe data in the player build with scenes that were part of a multi-scene bake.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/990626/">990626</a>) - GI: Fixed harmless "Lighting data asset [...] is inconsistent" errors when moving those assets between projects.</li>
<li>(1011232) - Graphics: Fixed for Android/OpenGLES Cubemap native texture not being registered correctly causing cubemap CopyTexture to native texture to fail.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989654/">989654</a>) - Graphics: Fixed black screen on devices that do not support RGBA16F rendering to texture.</li>
<li>(None) - Il2CPP: Improve Android build size.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005019/">1005019</a>) - IL2CPP: Fixed an error in the managed linker which can occur when the Vurforia plugin is used on iOS.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011133/">1011133</a>) - IL2CPP: Fixed delegate invocation of a virtual method that is passed directly to an action.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/999803/">999803</a>) - IL2CPP: Fixed method parameter attributes not being handled for methods on generic types.</li>
<li>(1009701 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/953606">953606</a>)) - iOS: Fixed Standard shader specular highlights on mobiles.</li>
<li>(1005678) - iOS: Fixed possible crash in UnityWebRequest.</li>
<li>(1016613 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1013198">1013198</a>)) - iOS: Fixed crash when creating texture from PNG image when cardboard VR is enabled.</li>
<li>(None) - iOS: Improved robustness of second stage splash screen setup to work correctly on both ancient and current iOS versions.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/972995/">972995</a>) - iOS: Added support for iPhone X second stage splash screen.</li>
<li>(None) - Multiplayer: Fixed server active disconnect client for web sockets.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/946958/">946958</a>) - OSX: Fixed crash in UnitcodeInputView during editor shutdown.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985049/">985049</a>) - Particles: Fixed Particle Collision not being detected when System uses negative scale.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/983677/">983677</a>) - Particles: Fixed performance drop with Size over Lifetime or Size over Speed modules enabled when emitting particles from script.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/990696/">990696</a>) - Particles: Fixed case where ParticleSystem's EmitParams.velocity was ignored when 'Shape' was checked.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989631/">989631</a>) - Particles: Fixed prefabs with a ParticleSystem no longer keeps creating duplicate entries into its serialization after each modification.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/967476/">967476</a>) - Particles: Particles/Alpha Blended material inverted colors of other blended objects when using HDR.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/988854/">988854</a>) - Particles: Fixed Editor crashing after two Emit() waves with UpdateSizeTpl&lt;0&gt; when Noise module's Size Amount parameter was more than zero.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970414/">970414</a>) - Particles: Fixed ParticlesStandardUnlit shader causing MissingReferenceException when Particle System StopAction was set to Destroy.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/967752/">967752</a>) - Particles: Fixed preview of Rate over Distance emission, during Edit Mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1001875/">1001875</a>) - Physics: Fixed an issue where auto-simulation is off but 2D collider shapes that are destroyed do not get removed from the internal shape changes queue resulting in shape destruction time increasing.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006679/">1006679</a>) - Physics: Ensured that recursive 2D physics callbacks do not causes a crash when reparenting/disabling with existing contacts.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/983374/">983374</a>) - Physics: Ensured that a Kinematic Rigidbody2D created in script stays in a relative position to any parent Rigidbody2D when reparented.</li>
<li>(1012718 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/987943">987943</a>)) - Profiler: Fixed missing format extension for binary logging, added .raw extension to our binary format.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/919769/">919769</a>) - Scene Management: Fixed crash in SplatMaterials::FindMaterialProperties when opening a scene with specific Material and Terrain combination.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/986215/">986215</a>) - Scripting: Fixed crash when SocketException is encountered.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/911661/">911661</a>) - Scripting: Fixed memory leak when entering play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/952292/">952292</a>) - Scripting Upgrade: Fixed crashes when exiting via alt+f4 when using new scripting runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/943047/">943047</a>) - Scripting Upgrade: Fixed DateTime.Now on scripting runtime upgrade.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/990979/">990979</a>) - Scripting Upgrade: Fixed random error when using UDPClient.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/977917/">977917</a>) - Scripting Upgrade: Fixed exception when binding delegate with Enum value to method with int parameter.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002004/">1002004</a>) - Sprite Packer: Fixed specific set of sprites are packed non-optimaly.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005779/">1005779</a>) - Substance: Fixed a memory leak when using cloned ProceduralMaterials.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/979587/">979587</a>) - Timeline: Fixed tracks and clips copied across timelines retaining links to original.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010354/">1010354</a>) - Universal Windows Platform: Fixed player getting stuck on a white screen when a fatal error (such as unable to load files or system doesn't meet minimum requirements) occurs during startup.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/997876/">997876</a>) - Universal Windows Platform: Fixed build failing on IL2CPP scripting backend if class library from Mono directory was copied into the project (like System.Data.dll).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991154/">991154</a>) - Universal Windows Platform: Fixed a crash in .NET native compiler ("RHB0011: Internal error: 'pchTypeNameEnd[0] == L'&gt;"at'f:\dd\ndp\rh\src\tools\rhbind\makepdb.cpp:998") in certain scenarios involving plugins.</li>
<li>(1004327 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1001438">1001438</a>)) - Web: Fixed abort on iOS on UnityWebRequest timeout.</li>
<li>(None) - Web: Switched UnityWebRequest default to chunkedTransfer=false.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996015/">996015</a>) - Windows: Fixed resolution dialog not showing monitor list and crashing on pressing 'Play' button on some weird monitor setups.</li>
<li>(948559) - Windows MR: Fixed GestureRecognizer is not returning grip data.</li>
<li>(976378) - Windows MR: Fixed GetureRecognizer stops working after HMD loses tracking.</li>
<li>(989909) - Windows MR: Fixed Gesture manipulation horizontal movement appears to operate on X/Z plane.</li>
<li>(964836) - Windows MR: Fixed GestureRecognizer callbacks returning InteractionSourceKind Other for hand gestures.</li>
<li>(956509) - Windows MR: Fixed incorrect grip position in Gesture Recognizer event handlers.</li>
<li>(1008179 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/950796">950796</a>)) - Windows MR: Fixed plugging a HMD with a running MR app causes performance to drop from a warning spam.</li>
<li>(971384) - Windows MR: Fixed Manipulation axes are not matching controller axes.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/976544/">976544</a>) - Windows MR: Fixed Manipulation Event Data is wonky after resuming from sleep.</li>
<li>(None) - XR: Fixed incorrect thread affinity setting on Gear VR.</li>
<li>(1008179 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/950796">950796</a>)) - XR: Fixed log spam when app starts disconnected from Windows MR HMD and crash when HMD is reconnected.</li>
<li>(None - XR: Updated warning issued when a VR SDK is not supported in the Editor.</li>
<li>(1011573 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991127">991127</a>)) - XR: Updated Google VR NDK to 1.130 for Android, 1.120 for iOS.</li>
<li>(None) - XR: Updated Vuforia to version 7.0.50.</li>
</ul>

#### Revision: 9231f953d9d3
