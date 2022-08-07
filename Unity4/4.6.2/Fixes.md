# Unity 4.6.2
https://unity3d.com/unity/whats-new/unity-4.6.2

## Fixes

<ul>
<li>2D: Custom sprites are now forced to have unique name when created through Sprite Editor.</li>
<li>2D: Fixed PolygonCollider2D mesh generation on Android.</li>
<li>2D: Hotkey for sprite Trim 'T' doesn't intervene with sprite naming anymore.</li>
<li>2D: Single sprite pivot will be now properly saved in Sprite Editor.</li>
<li>2D: Sprite importer multi-editing now works for packing tag, pixels per unit and extrude fields.</li>
<li>2D: Sprite Packer page list is now refreshed after packing.</li>
<li>Android: Android TV - do not strictly require accelerometer and microphone.</li>
<li>Android: Fix for NullReferenceException causing a crash.</li>
<li>Android: Fixed a file-loading problem which occasionally caused 'Inflate Error' messages &amp; freezes or crashes when loading resources on Android.</li>
<li>Android: Fixed broken texture upload from OnApplicationPause(false).</li>
<li>Android: Fixed build failure on x86 Java on Windows.</li>
<li>Android: Fixed CJK fonts on Android Lollipop.</li>
<li>Android: Fixed possible crash in hardware stats code.</li>
<li>Android: Fixed deadlock when calling UnityPlayer.pause() too early.</li>
<li>Android: Fixed freeze during startup on some Amazon Kindle devices.</li>
<li>Android: Fixed freeze on focus change when app is not paused (e.g. keyboard input).</li>
<li>Android: Fixed Japanese Kana fonts on Android Lollipop.</li>
<li>Android: Fixed lights-out mode on Android Lollipop.</li>
<li>Android: Fixed possible lost wakeup in UnityPlayer when rapidly calling pause/resume.</li>
<li>Android: Fixed theme attribute in default manifest to hide title bar during startup.</li>
<li>Android: Increase maximum memory available to Java when building for Android.</li>
<li>Animation: Animation window no longer shows 'Function not supported' for events on secondary MonoBehaviours.</li>
<li>Animation: Don't expose multiple entries for a source clip in AnimatorOverrideController.</li>
<li>Animation: Optimize and DeoptimizeTransformHierarchy are available in runtime as well as editor.</li>
<li>Asset Import: Imported assets now update the project label database correctly.</li>
<li>Asset Import: Restored previous behaviour of AssetModificationProcessor.OnWillSaveAssets to ignore null or void return values.</li>
<li>Asset Import: Reserialize imported .unitypackage assets to comply with project's Force Binary / Force Text serialization setting.</li>
<li>Core: Fixed incorrect error message when RectTransform.GetWorldCorners is called with incorrect parameters.</li>
<li>Core: PPtr animations now properly trigger the OnDidApplyAnimationProperties callback.</li>
<li>Editor: Allow viewing of all ModelImporter tabs when the model is not open for edit.</li>
<li>Editor: Fixed importing of .DDS textures with XRGB color formats.</li>
<li>Editor: Fixed a bug where driven RectTransform would incorrectly mark the scene dirty if it had a Vector2 where one coord was driven and the other not. Such a setup is common with the ContentSizeFitter UI component.</li>
<li>Editor: Fixed a small memory leak related to FormerlySerializedAs attribute.</li>
<li>Editor: Fixed bugs that caused UnityEvent object references to change by themselves with no user action when selecting multiple objects.</li>
<li>Editor: Fixed lagginess in editor when destroying multiple elements.</li>
<li>Editor: Fixed navigation to next / previous animation keyframes when there are subframe keyframes.</li>
<li>Graphics: Worked around some GPU driver bugs that were causing crashes when using OpenGL ES 3.0.</li>
<li>Graphics: Fixed possible memory corruption when using dynamic batching on platforms that support NEON.</li>
<li>Graphics: Fixed D3D9 handling of unsupported BGRA32 texture format to fall back properly to ARGB32.</li>
<li>Graphics: Texture2D.PackTextures will produce an ARGB4444-format atlas if all input textures are ARGB4444/RGBA4444.</li>
<li>iOS: Do not rotate splash view on non 6+ iPhones.</li>
<li>iOS: Ensure that Input.touches is not changed during the frame.</li>
<li>iOS: Fixed 2nd stage splash orientation on iOS 8.0+ landscape.</li>
<li>iOS: Fixed crash when text field contents are modified via script and undo is used.</li>
<li>iOS: Fixed OpenGL ES backbuffer size determination (fixes iPhone6+ zoomed mode).</li>
<li>iOS: Fixed local notifications for iOS 8.0. You should call NotificationServices.RegisterForLocalNotificationTypes before scheduling first notification.</li>
<li>iOS: Fixed messed up terminal settings if building for iOS from console.</li>
<li>iOS: Fixed skewed image on secondary display (AirPlay).</li>
<li>iOS: Fixed splash screen check on Xcode 5 when iPhone 6 splashes are present.</li>
<li>iOS: Fixed Xcode 6.2 support.</li>
<li>iOS: Increased stack allocator size on iOS.</li>
<li>iOS: On iOS set no backup flag on __info cache file. </li>
<li>iOS: Register SubstanceArchive when procedural materials are used.</li>
<li>iOS/IL2CPP: Correctly emit method, property, field, and event counts for array types</li>
<li>iOS/IL2CPP: Dramatically reduce the amount of warnings the generated code produces.</li>
<li>iOS/IL2CPP: Fixed Armv7 linker errors ("b/bl/blx ARM branch out of range").</li>
<li>iOS/IL2CPP: Fixed crash in reflecting over custom attributes.</li>
<li>iOS/IL2CPP: Gamecenter integration works now.</li>
<li>iOS/IL2CPP: Fixed incorrect code being generated for open generic types deriving from UnityEngine.Object.</li>
<li>iOS/IL2CPP: Fixed memory leak in reflection code.</li>
<li>iOS/IL2CPP: Fixed race condition in internal reflection implementation.</li>
<li>iOS/IL2CPP: Ignore managed types not in the UnityEngine namespace when the types which should not be stripped are discovered. </li>
<li>iOS/IL2CPP: BinaryFormatter serializer works now.</li>
<li>iOS/IL2CPP: Generated C++ code is a lot easier to read now.</li>
<li>iOS/IL2CPP: Treat arrays created with a lower bound of zero (via Array.CreateInstance) as SZARRAY types.</li>
<li>Linux: Make device unique identifier more consistent.</li>
<li>Mac OS X Standalone: Release player builds are now stripped off symbols again.</li>
<li>MonoDevelop: Generated solutions include 'indent size' directive to match tab size now.</li>
<li>Oculus Plugin: Fixed GearVR Unity Pro + Android Basic license issue.</li>
<li>Physics 2D: HingeJoint2D gizmo is displayed correctly with respect to any reference angle.</li>
<li>Physics 2D: Changes to the EdgeCollider2D points are now saved when used in prefabs.</li>
<li>Physics 2D: Setting the Rigidbody2D position or rotation directly now wakes the body.</li>
<li>Physics 2D: SliderJoint2D &amp; HingeJoint2D reference angles are now reset when connecting to another Rigidbody2D.</li>
<li>Physics 2D: Static 2D collider gizmos now render at the correct Transform Z position.</li>
<li>Scripting: Fixed a harmless but annoying error message when using StopCoroutine(Coroutine).</li>
<li>Scripting: Fixed issue with Console.InputEncoding and Console.OutputEncoding throwing an exception the first they were set on the .NET 2.0 Subset profile.</li>
<li>Shaders: Fixed editor memory leak in shader error reporting.</li>
<li>UI: Changing any Transition settings on a Selectable Component will now immediately reflect on the Scene and Game View.</li>
<li>UI: Don't apply AspectRatioFitter logic when component is inactive.</li>
<li>UI: Fixed a bug which caused wrong Y cursor alignment in TextField with custom fonts. </li>
<li>UI: Fixed division by zero if ScrollRect content size has zero width or height.</li>
<li>UI: Fixed issue where adding and removing a parent canvas wouldn't update parent canvas relationship of child objects.</li>
<li>UI: Fixed issue where keyboard would not display on mobile devices.</li>
<li>UI: Fixed regression with events being sent to wrong object in some cases when using multiple GraphicRaycasters.</li>
<li>UI: Make sure we copy the pointer enter for the right and middle mouse pointers when we fetch them.</li>
<li>UI: Moved EventSystemEditor from UnityEditor.UI namespace to UnityEditor.EventSystems namespace.</li>
<li>UI: Prevent the '/n' from appearing when reactivating an input-field in the disable call.</li>
<li>UI: Sliced image with transparent borders (padding) works correctly with non-default pixelsPerUnit.</li>
<li>UI: When activating the standaloneInputModule do not set selected element to NULL.</li>
<li>Version Control: Fixed drag-dropping assets between change lists only moving a single asset.</li>
<li>Windows Phone 8: It's now possible to specify plugins that should not be processed just like in Windows Store Apps.</li>
<li>Windows Phone 8.1/Store Apps: Fixed an issue which caused casting arrays in UnityScript sometimes throw MissingMethodException deep inside Boo.Lang.dll.</li>
<li>Windows Phone/Store Apps: Fixed a rare crash that was caused by skinned meshes.</li>
<li>WWW: Fixed bug in WWW Caching when WWW.LoadFromCacheOrDownload is canceled using WWW.Dispose.</li>
</ul>
