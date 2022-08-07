# Unity 2019.1
https://unity3d.com/unity/whats-new/2019.1.0

## Features

<ul>
<li><p>Android: Added Android notch/cut-out support to <code>Screen.safeArea</code></p></li>
<li><p>Android: Added OpenGL ES 3.2 support</p></li>
<li><p>Android: Added Script Only Patching functionality, which sends only script-related changes to the device instead of repackaging the APK file.</p></li>
<li><p>Android: Added support for ASTC HDR texture formats</p></li>
<li><p>Android: Added <code>AndroidDevice.SetSustainedPerformanceMode</code> to the API to enable/disable sustained performance mode in runtime</p></li>
<li><p>Android: Enabled redistributing Android NDK and SDK components with Android Build Support</p></li>
<li><p>Editor: Added a new Scene view <strong>Camera settings</strong> menu to control field of view (FOV), Camera speed, and Camera easing while moving and zooming. In Flythrough mode, the mouse scroll wheel adjusts the Camera speed.</p></li>
<li><p>Editor: Added a new Shortcuts Manager window for managing keyboard shortcuts.</p></li>
<li><p>Editor: Added a search field to the Console for filtering output by keyword.</p></li>
<li><p>Editor: Added checkboxes to the Gizmos menu for selecting/deselecting all gizmos in a given section (<strong>Built-in Components</strong>, <strong>Scripts</strong>, and so on).</p></li>
<li><p>Editor: Added new <strong>EditorTools</strong> API for creating custom tools that behave like native tools. The <strong>Available Custom Editor Tools</strong> button in the Scene view toolbar opens a custom tools menu. The <strong>Component Editor Tools</strong> panel in the Scene view shows available custom tools for the current selection.</p></li>
<li><p>Editor: Added pre-checkout and pre-submit user-specified callbacks for VCS integration. Allows users to create callbacks that can modify Asset lists and changeset selections/descriptions at checkout and submit time.</p>

<p>Pre-checkout callback can:</p>

<ul>
<li>Add and remove assets from the list of those that will be checked out</li>
<li>Create a new changeset to check the specified asset list in</li>
<li>Nominate an existing changeset to check the specified asset list in</li>
<li>Return false from the callback to block checkout</li>
</ul>

<p>Pre-submit callback can:</p>

<ul>
<li>Add and remove assets from the list of those that will be submitted</li>
<li>Create a new changeset to submit specified asset list in</li>
<li>Nominate an existing changeset to submit the specified asset list in</li>
<li>Rename an existing changeset then submit it and</li>
<li>Return false from the callback to block submission</li>
</ul></li>
<li><p>Editor: Added Scene visibility controls to the Hierarchy window for controlling the visibility of GameObjects in the Scene view. Users can toggle visibility for individual GameObjects, or GameObjects and their children. A global visibility toggle hides/shows everything in the scene.</p></li>
<li><p>Editor: Added support for referencing Assembly Definitions with GUIDs instead of assembly names. Users can enable this setting via the <strong>Use GUIDs</strong> property in the Assembly Definition Inspector.  This is now the default setting for new Assembly Definition files.</p></li>
<li><p>Editor: Added <code>CSHARP_7_3_OR_NEWER</code> preprocessor directive when compiling C# 7.3 on .NET 4.x scripting runtime.</p></li>
<li><p>Editor: Exposed <code>AdvancedDropdown</code> API for implementing searchable <code>AddComponent</code> style dropdowns.</p></li>
<li><p>Editor: Made editor on-demand shader compilation asynchronous, not blocking the editor while compiling the shader on the first time usage. Rendering happens with a replacement shader until the actual shader variant is available. To enable or disable this feature, go to Project Settings &gt; Editor &gt; Asynchronous Shader Compilation.</p></li>
</ul>
