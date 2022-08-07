# Unity 2019.3.0
https://unity3d.com/unity/whats-new/2019.3.0

## System Requirements


### For development

#### OS: Windows 7 SP1+, 8, 10, 64-bit versions only; macOS 10.12+. (Server versions of Windows & OS X are not tested.)

#### CPU: SSE2 instruction set support.

#### GPU: Graphics card with DX10 (shader model 4.0) capabilities.

#### The rest mostly depends on the complexity of your projects.

### Additional platform development requirements:
<ul>
<li><p>iOS: Mac computer running minimum macOS 10.12.6 and Xcode 9.4 or higher.</p></li>
<li><p>Android: Android SDK and Java Development Kit (JDK); IL2CPP scripting backend requires Android NDK.</p></li>
<li><p>Universal Windows Platform: Windows 10 (64-bit), Visual Studio 2015 with C++ Tools component or later and Windows 10 SDK</p></li>
</ul>

### For running Unity games

#### Generally content developed with Unity can run pretty much everywhere. How well it runs is dependent on the complexity of your project. More detailed requirements:
<ul>
<li><p>Desktop:</p> 
<ul>
<li>OS: Windows 7 SP1+, macOS 10.12+, Ubuntu 16.04+</li>
<li>Graphics card with DX10 (shader model 4.0) capabilities.</li>
<li>CPU: SSE2 instruction set support.</li>
</ul></li>
<li><p>iOS player requires iOS 10.0 or higher.</p></li>
<li><p>Android: OS 4.4 or later; ARMv7 CPU with NEON support; OpenGL ES 2.0 or later.</p></li>
<li><p>WebGL: Any recent desktop version of Firefox, Chrome, Edge or Safari.</p></li>
<li><p>Universal Windows Platform: Windows 10 and a graphics card with DX10 (shader model 4.0) capabilities</p></li>
<li><p>Exported Android Gradle projects require Android Studio 3.4 and later to build</p></li>
</ul>

### Known Issues in 2019.3.0f6
<ul>
<li><p>Ads:  Verified and default Ads package for 2019.3 should be 3.3.1 instead of 2.0.8 (<a href="https://issuetracker.unity3d.com/issues/ads-older-ads-package-is-available-in-package-manager">1206332</a>)</p></li>
<li><p>Animation: Animator.Update CPU time spikes when multiple animations are playing (<a href="https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing">1184690</a>)</p></li>
<li><p>Global Illumination: Crash on SpookyHash::Short when continually interrupting auto-generating light (<a href="https://issuetracker.unity3d.com/issues/crash-on-spookyhash-short-when-continually-interrupting-auto-generating-light">1205313</a>)</p></li>
<li><p>Global Illumination: [CPU PLM] Out of memory errors after launching bake on an upgraded project on OSX (<a href="https://issuetracker.unity3d.com/issues/cpu-plm-out-of-memory-errors-after-launching-bake-on-an-upgraded-project-on-osx">1131009</a>)</p></li>
<li><p>IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies (<a href="https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies">1193774</a>)</p></li>
<li><p>IMGUI: Editor performance drop when holding down keys and moving mouse when in Playmode (<a href="https://issuetracker.unity3d.com/issues/editor-performance-drop-when-holding-down-keys-and-moving-mouse-when-in-playmode">1211383</a>)</p></li>
<li><p>IMGUI: [TreeCreator] NullReferenceException on modifying properties of "Tree" components when "Branch Material" is set to any material (<a href="https://issuetracker.unity3d.com/issues/terrain-nullreferenceexception-on-modifying-properties-of-tree-components-when-branch-material-is-set-to-any-material">1206697</a>)</p></li>
<li><p>MacOS:  [URP][macOS] Game View is overlayed by background color when Background Type Solid Color property is selected (<a href="https://issuetracker.unity3d.com/issues/urp-macos-game-view-is-overlayed-by-background-color-when-background-type-solid-color-property-is-selected">1210093</a>)</p></li>
<li><p>Mobile: [Android] Loading assets from AssetBundles takes significantly more time when the project is built as an AAB (<a href="https://issuetracker.unity3d.com/issues/android-loading-assets-from-assetbundles-takes-significantly-more-time-when-the-project-is-built-as-an-aab">1153358</a>)</p></li>
<li><p>Physics: Cloth's movement simulation is incorrect when the game object is rotated in world space (<a href="https://issuetracker.unity3d.com/issues/cloths-movement-simulation-is-incorrect-when-the-game-object-is-rotated-in-world-space">1192837</a>)</p></li>
<li><p>Profiling: Exception is thrown with Profiler window turning blank on selecting Memory Module from Profiler window (<a href="https://issuetracker.unity3d.com/issues/exception-is-thrown-with-profiler-window-turning-blank-on-selecting-memory-module-from-profiler-window">1198768</a>)</p></li>
</ul>

### New 2019.3.0f6 Entries since 2019.3.0f5
