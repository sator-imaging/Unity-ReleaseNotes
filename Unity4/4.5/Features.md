# Unity 4.5
https://unity3d.com/unity/whats-new/unity-4.5

## Features


### Graphics features:
<ul>
<li>Shader importing has been massively improved: 
<ul>
<li>Shaders are imported much faster, especially complex surface shaders. Instead of compiling all shader variants for all possible platforms at import time, now the needed shader variants for needed platforms are compiled on-demand. Shader compilation results are cached under Library folder, so identical compilations happen much faster.</li>
<li>Error reporting was improved. Errors are reported on correct lines (imagine that!), and errors in .cginc files report the filename.</li>
<li>Surface shader debugging was improved. No more "#pragma debug" nonsense; just click "Show generated code" in the inspector.</li>
</ul></li>
<li>Added Sparse Texture support (also known as "mega textures" or "tiled textures"). This is a low-level API feature, see SparseTexture class. Implemented on DirectX 11.2 (via tiled resources) and desktop OpenGL (via ARB_sparse_texture).</li>
<li>Added stereoscopic rendering on DX 11.1 (requires Windows 8.1 and compatible hardware).</li>
<li>Introduced support for OpenGL ES 3.0 on iOS devices (starting with A7 devices).</li>
<li>Graphics: Support for 3D textures in OpenGL ES 3.0.</li>
</ul>

### Module Manager:
<ul>
<li>Introduced Module Manager with updatable platform support.  iOS, Android, Windows Phone 8, Blackberry Unity add ons can be updated without downloading full editor installer. Accessed through Modules menu, next to Preferences menu.</li>
</ul>

### Editor features:
<ul>
<li>New Hierarchy Window  sorting - sorting of elements is now based on transform order instead of name.</li>
<li>Introduced new editor API AssetDatabase.FindAssets (string filter, string[] folders). Search the Asset Database for assets by filename, type and asset label. See documentation for more information.</li>
<li>Added Selection.assetGUIDs for getting the current selected assets in the Project Browser. It also returns the folder selection in the first column in the Project Browser (in Two Column mode) which is not part of the main selection.</li>
</ul>

### 2D Physics features:
<ul>
<li>Added 2D Joint Gizmos.</li>
<li>Added new 2D physics component: WheelJoint2D.</li>
</ul>

### Unity Remote upgrade:
<ul>
<li>Unity Remote 4 is our play testing solution for iOS and Android. As of Unity 4.5, there’ll be no more Wifi latency when playtesting your games on iOS devices. Plus, we’ve added support for the full range of iOS device inputs including accelerometers, gyroscopes and camera images. Unity Remote 4 is available free of charge from Google Play and the App Store.</li>
</ul>

### Mecanim features:
<ul>
<li>Added CanTransitionToSelf option on AnyState Transitions.</li>
<li>Added new scripting function Animator.Rebind(). You can use this function to manually rebind the animator data set to unity when you change something in your GameObject hierarchy.</li>
<li>For humanoid rigs, in the importer, you can specify a transform node that will be used as root motion for an animation clip.  The transform node will replace the automatically extracted root motion computed by Mecanim. (Pro Only).</li>
</ul>

### Windows Store apps features:
<ul>
<li>Added Compass API to check for compass accuracy.</li>
<li>AppCallbacks methods InvokeOnUIThread and InvokeOnAppThread will detect deadlock and throw exception. Added TryInvokeOnUIThread and TryInvokeOnAppThread, which return true or false instead.</li>
<li>Support for programmatically opening touch screen keyboard.</li>
<li>In Player Preferences added support for scaled resources: splash screen, medium and wide tile, store and small logos.</li>
<li>In Player Preferences added support for Windows 8.1 scaled resources and related settings.</li>
<li>New APIs for changing system cursor - AppCallbacks::SetCursor, AppCallbacks::SetCustomCursor, WSA.Cursor.SetCustomCursor.</li>
<li>Added support for changing screen resolution on Windows 8.1.</li>
</ul>

### Other features:
<ul>
<li>Scripting: Introduced DisallowMultipleComponentAttribute for disallowing multiple components of the same type being added to a single GameObject.</li>
<li>Scripting: Add UnityEngine.ISerializationCallbackReceiver interface, to get a callback right before serialisation and right after deserialization.</li>
<li>Scripting: Structs with System.Serializable attribute can now be serialized. Also, fields of AnimationCurve[] and double[] now get serialised.</li>
<li>WebPlugin: Added  Enhanced Protected Mode support for Internet Explorer. Supports IE 64 bit.</li>
</ul>
