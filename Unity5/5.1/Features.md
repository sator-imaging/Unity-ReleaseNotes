# Unity 5.1
https://unity3d.com/unity/whats-new/unity-5.1

## Features

<ul>
<li>New multiplayer networking feature introduced, see the manual and UnityEngine.Networking namespace in the script reference for details. This includes low level API (transport layer) and a higher level API with many features to help implement multiplayer functionality in games. Cloud based relay service can be used to get past NAT restrictions, and a simple matchmaking service can be used for game/host discovery. To configure the services go to <a href="https://multiplayer.unity3d.com">https://multiplayer.unity3d.com</a>. The current RakNet based multiplayer system will be deprecated but still functional in this release.  </li>
<li>New network components and NetworkBehaviour base class for network aware scripts:</li>
</ul>

#### 
<ul>
<li>New NetworkManager to control and configure multiplayer games:</li>
</ul>

#### 
<ul>
<li>Added integrated support for Oculus Rift in Editor and Standalone Players, see the Manual and UnityEngine.VR namespace script reference for details  Once Virtual Reality is enabled in Player Settings, pressing play in the editor will show your game view on the Rift.  It is recommended to "Maximize on Play" the game view and run the Oculus Rift in Extended mode in order to achieve the smoothest rendering.  Be sure to remove any previous Oculus plugins and assets from your project, or update to the latest version that supports 5.1. 
<ul>
<li>VR optimization: Render shadows only once and share between eyes.</li>
<li>VR optimization: Cull once for both eyes.</li>
<li>Support for Oculus 0.6.0-beta runtime</li>
</ul></li>
</ul>

#### 
<ul>
<li>New HDR Color Picker 
<ul>
<li>Improves the Standard shader workflow for changing the emission color property.</li>
<li>The emission color can now be animated from the animation window.</li>
<li>Using scripting API to change emission will now be reflected in the shader gui.</li>
<li>Color Presets now also support HDR colors. Saving a HDR color will overlay a lowercase 'h' on the preset swatch.</li>
<li>Color property fields can now be customized with the ColorUsageAttribute (show/hide alpha value, is HDR)</li>
<li>Added Hex color field</li>
</ul></li>
</ul>

#### 
<ul>
<li>Graphics: Crunch texture compression format on platforms which support DXT. This is a lossy compression that is both small on disk/download and compressed (DXT1/DXT5) for the GPU.</li>
</ul>

#### 
<ul>
<li>Graphics: Experimental support for OpenGL 4.5 and ES 3.1 on Windows. Use -force-glcore, -force-gles(20|30|31|31aep) arguments to enable. This enables testing OpenGL ES 3.1 features on desktop. Note: no GL4 support on Mac or Linux yet.  
<ul>
<li>Graphics: OpenGL ES 3.1 support on Android</li>
<li>New graphics levels (OpenGL ES 3.1, OpenGL ES 3.1 + AEP)</li>
<li>Compute shaders</li>
<li>Geometry shaders</li>
<li>Tessellation shaders</li>
<li>Advanced blend modes</li>
<li>Note: OpenGL ES 3.0/3.1 uses a new shader compiler backend; see Changes below.</li>
</ul></li>
<li>New runtime assertion library under UnityEngine.Assertions namespace. The library provides a set of methods for setting assertions in your code. 
<ul>
<li>The method calls will be conditionally compiled out from non-developer’s builds.</li>
<li>The conditional compilation is controlled by UNITY_ASSERTION define.</li>
<li>Defines DEBUG and TRACE are now also defined for non-developer’s builds. </li>
<li>A wrapping library providing extension methods is also available under UnityEngine.Assertions.Must namespace. </li>
</ul></li>
<li>Unity Analytics: new, built-in Analytics functionality introduced (currently in “Preview”), under the UnityEngine.Analytics namespace. 
<ul>
<li>Basic Integration can be completed by inserting a unique ProjectId into “Cloud Project Id” in PlayerSettings.</li>
</ul></li>
</ul>

#### 
<ul>
<li>The ProjectId is a unique identifier that links your Editor project with the data on your Analytics dashboard, and is generated during the Basic Integration process. 
<ul>
<li>Go to http://analytics.unity3d.com to get started with Basic Integration, as well as access the relevant documentation and integration instructions. </li>
<li>Additionally, the library provides methods to track Monetization, Custom Events, and User Attributes (otherwise known as Advanced Integration options).</li>
</ul></li>
</ul>

#### 
<ul>
<li>Note: 4.x and 5.0 Editor users can still use Analytics by integrating the downloadable SDK package. For 5.1 users, adding the plug-in should not result in errors, nor will it result in duplicate data, but we still advise that you remove the old plug-in assets.</li>
<li>Home Window Login integration. You can now login or work offline using the home window or command-line arguments.</li>
</ul>

#### 
<ul>
<li>Home Window License integration. You can now validate your serial and activate your copy of Unity using the new 5.1 json licensing API through the home window.</li>
</ul>

#### 
