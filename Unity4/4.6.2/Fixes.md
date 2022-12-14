# Unity 4.6.2

https://unity3d.com/unity/whats-new/unity-4.6.2

## Fixes



*   2D: Custom sprites are now forced to have unique name when created through Sprite Editor.
*   2D: Fixed PolygonCollider2D mesh generation on Android.
*   2D: Hotkey for sprite Trim 'T' doesn't intervene with sprite naming anymore.
*   2D: Single sprite pivot will be now properly saved in Sprite Editor.
*   2D: Sprite importer multi-editing now works for packing tag, pixels per unit and extrude fields.
*   2D: Sprite Packer page list is now refreshed after packing.
*   Android: Android TV - do not strictly require accelerometer and microphone.
*   Android: Fix for NullReferenceException causing a crash.
*   Android: Fixed a file-loading problem which occasionally caused 'Inflate Error' messages & freezes or crashes when loading resources on Android.
*   Android: Fixed broken texture upload from OnApplicationPause(false).
*   Android: Fixed build failure on x86 Java on Windows.
*   Android: Fixed CJK fonts on Android Lollipop.
*   Android: Fixed possible crash in hardware stats code.
*   Android: Fixed deadlock when calling UnityPlayer.pause() too early.
*   Android: Fixed freeze during startup on some Amazon Kindle devices.
*   Android: Fixed freeze on focus change when app is not paused (e.g. keyboard input).
*   Android: Fixed Japanese Kana fonts on Android Lollipop.
*   Android: Fixed lights-out mode on Android Lollipop.
*   Android: Fixed possible lost wakeup in UnityPlayer when rapidly calling pause/resume.
*   Android: Fixed theme attribute in default manifest to hide title bar during startup.
*   Android: Increase maximum memory available to Java when building for Android.
*   Animation: Animation window no longer shows 'Function not supported' for events on secondary MonoBehaviours.
*   Animation: Don't expose multiple entries for a source clip in AnimatorOverrideController.
*   Animation: Optimize and DeoptimizeTransformHierarchy are available in runtime as well as editor.
*   Asset Import: Imported assets now update the project label database correctly.
*   Asset Import: Restored previous behaviour of AssetModificationProcessor.OnWillSaveAssets to ignore null or void return values.
*   Asset Import: Reserialize imported .unitypackage assets to comply with project's Force Binary / Force Text serialization setting.
*   Core: Fixed incorrect error message when RectTransform.GetWorldCorners is called with incorrect parameters.
*   Core: PPtr animations now properly trigger the OnDidApplyAnimationProperties callback.
*   Editor: Allow viewing of all ModelImporter tabs when the model is not open for edit.
*   Editor: Fixed importing of .DDS textures with XRGB color formats.
*   Editor: Fixed a bug where driven RectTransform would incorrectly mark the scene dirty if it had a Vector2 where one coord was driven and the other not. Such a setup is common with the ContentSizeFitter UI component.
*   Editor: Fixed a small memory leak related to FormerlySerializedAs attribute.
*   Editor: Fixed bugs that caused UnityEvent object references to change by themselves with no user action when selecting multiple objects.
*   Editor: Fixed lagginess in editor when destroying multiple elements.
*   Editor: Fixed navigation to next / previous animation keyframes when there are subframe keyframes.
*   Graphics: Worked around some GPU driver bugs that were causing crashes when using OpenGL ES 3.0.
*   Graphics: Fixed possible memory corruption when using dynamic batching on platforms that support NEON.
*   Graphics: Fixed D3D9 handling of unsupported BGRA32 texture format to fall back properly to ARGB32.
*   Graphics: Texture2D.PackTextures will produce an ARGB4444-format atlas if all input textures are ARGB4444/RGBA4444.
*   iOS: Do not rotate splash view on non 6+ iPhones.
*   iOS: Ensure that Input.touches is not changed during the frame.
*   iOS: Fixed 2nd stage splash orientation on iOS 8.0+ landscape.
*   iOS: Fixed crash when text field contents are modified via script and undo is used.
*   iOS: Fixed OpenGL ES backbuffer size determination (fixes iPhone6+ zoomed mode).
*   iOS: Fixed local notifications for iOS 8.0. You should call NotificationServices.RegisterForLocalNotificationTypes before scheduling first notification.
*   iOS: Fixed messed up terminal settings if building for iOS from console.
*   iOS: Fixed skewed image on secondary display (AirPlay).
*   iOS: Fixed splash screen check on Xcode 5 when iPhone 6 splashes are present.
*   iOS: Fixed Xcode 6.2 support.
*   iOS: Increased stack allocator size on iOS.
*   iOS: On iOS set no backup flag on \_\_info cache file.
*   iOS: Register SubstanceArchive when procedural materials are used.
*   iOS/IL2CPP: Correctly emit method, property, field, and event counts for array types
*   iOS/IL2CPP: Dramatically reduce the amount of warnings the generated code produces.
*   iOS/IL2CPP: Fixed Armv7 linker errors ("b/bl/blx ARM branch out of range").
*   iOS/IL2CPP: Fixed crash in reflecting over custom attributes.
*   iOS/IL2CPP: Gamecenter integration works now.
*   iOS/IL2CPP: Fixed incorrect code being generated for open generic types deriving from UnityEngine.Object.
*   iOS/IL2CPP: Fixed memory leak in reflection code.
*   iOS/IL2CPP: Fixed race condition in internal reflection implementation.
*   iOS/IL2CPP: Ignore managed types not in the UnityEngine namespace when the types which should not be stripped are discovered.
*   iOS/IL2CPP: BinaryFormatter serializer works now.
*   iOS/IL2CPP: Generated C++ code is a lot easier to read now.
*   iOS/IL2CPP: Treat arrays created with a lower bound of zero (via Array.CreateInstance) as SZARRAY types.
*   Linux: Make device unique identifier more consistent.
*   Mac OS X Standalone: Release player builds are now stripped off symbols again.
*   MonoDevelop: Generated solutions include 'indent size' directive to match tab size now.
*   Oculus Plugin: Fixed GearVR Unity Pro + Android Basic license issue.
*   Physics 2D: HingeJoint2D gizmo is displayed correctly with respect to any reference angle.
*   Physics 2D: Changes to the EdgeCollider2D points are now saved when used in prefabs.
*   Physics 2D: Setting the Rigidbody2D position or rotation directly now wakes the body.
*   Physics 2D: SliderJoint2D & HingeJoint2D reference angles are now reset when connecting to another Rigidbody2D.
*   Physics 2D: Static 2D collider gizmos now render at the correct Transform Z position.
*   Scripting: Fixed a harmless but annoying error message when using StopCoroutine(Coroutine).
*   Scripting: Fixed issue with Console.InputEncoding and Console.OutputEncoding throwing an exception the first they were set on the .NET 2.0 Subset profile.
*   Shaders: Fixed editor memory leak in shader error reporting.
*   UI: Changing any Transition settings on a Selectable Component will now immediately reflect on the Scene and Game View.
*   UI: Don't apply AspectRatioFitter logic when component is inactive.
*   UI: Fixed a bug which caused wrong Y cursor alignment in TextField with custom fonts.
*   UI: Fixed division by zero if ScrollRect content size has zero width or height.
*   UI: Fixed issue where adding and removing a parent canvas wouldn't update parent canvas relationship of child objects.
*   UI: Fixed issue where keyboard would not display on mobile devices.
*   UI: Fixed regression with events being sent to wrong object in some cases when using multiple GraphicRaycasters.
*   UI: Make sure we copy the pointer enter for the right and middle mouse pointers when we fetch them.
*   UI: Moved EventSystemEditor from UnityEditor.UI namespace to UnityEditor.EventSystems namespace.
*   UI: Prevent the '/n' from appearing when reactivating an input-field in the disable call.
*   UI: Sliced image with transparent borders (padding) works correctly with non-default pixelsPerUnit.
*   UI: When activating the standaloneInputModule do not set selected element to NULL.
*   Version Control: Fixed drag-dropping assets between change lists only moving a single asset.
*   Windows Phone 8: It's now possible to specify plugins that should not be processed just like in Windows Store Apps.
*   Windows Phone 8.1/Store Apps: Fixed an issue which caused casting arrays in UnityScript sometimes throw MissingMethodException deep inside Boo.Lang.dll.
*   Windows Phone/Store Apps: Fixed a rare crash that was caused by skinned meshes.
*   WWW: Fixed bug in WWW Caching when WWW.LoadFromCacheOrDownload is canceled using WWW.Dispose.