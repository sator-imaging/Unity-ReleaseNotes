# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Upgrade Guide



*   A new asset versioning system has been introduced which will trigger a reimport of textures, models, substance, and audio when opening a project created in previous versions of Unity.
*   In 3.5 the behaviour of when to add an extra root node containing imported animation nodes has changed. Previously it was based on if there are multiple root nodes and in order to fix issues where character animation files had only one but the model had multiple, it was using the @ notation files to figure out when to add multiple root nodes. Now the logic is simply: if any of the root nodes have a rigged bone attached or if there are multiple root nodes. This fixes a lot of issues in animations. In some rare cases it might lead to animations not play when importing, they can be fixed by matching the number of bones in the animation fbx file to the fbx file that contains the model.
*   Prefabs with multiple root game objects are no longer supported. Unity will automatically create a root gameobject for you when such a deprecated prefab is encountered.
*   The Mac OS X Development Web Player now requires Mac OS X 10.6. The normal user web player will continue to work on 10.5.
*   Mac OS X 10.4 support is discontinued at this point. Existing pre 3.5 content still can be used with older webplayers.
*   Unity 3.5 removes support for PowerPC and Dashboard build options on Mac OS X.
*   Mac OS X web players now support IME input (using an input window) in Chrome and Firefox. If enabled, you will not receive events for each key stroke and no KeyUp events, but only KeyDown events for the characters input. By default, this is enabled whenever a text field has focus. Use Input.imeCompositionMode to change the behavior.
*   Unity 3.5 makes your existing shaders work with directional lightmaps automatically. Unfortunately, decoding directional lightmaps is slightly more expensive than calculating lighting for a directional light. If a shader written in Unity 3.4 was just below the arithmetic instruction count limit of shader model 2.0 (64 instructions), it might go over this limit during the conversion, and fail to compile. To solve this, you can either make the shader compile against shader model 3.0 [https://unity3d.com/support/documentation/Components/SL-ShaderPrograms.html](/support/documentation/Components/SL-ShaderPrograms.html) or disable directional lightmaps with the “nodirlightmap” keyword [https://unity3d.com/support/documentation/Components/SL-SurfaceShaders.html](/support/documentation/Components/SL-SurfaceShaders.html).