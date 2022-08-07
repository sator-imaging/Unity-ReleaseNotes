# Unity 5.2.5
https://unity3d.com/unity/whats-new/unity-5.2.5

## Fixes

<ul>
<li>Android: Fixed internal profiler on Gear VR.  (741003).</li>
<li>Android: Fixed a crash after multiple scene loads.  (774183) .</li>
<li>Android: Fixed binary shader cache; cache was always disabled. (765388) .</li>
<li>Android: Fixed Cloth::SetUpSkinnedBuffers() crash.  (750362) .</li>
<li>Android: Fixed crash on Android after sleep/resume when using OnAudioFilterRead.  (771519) .</li>
<li>Android: Fixed crash when load scenes intermittently.  (751530) .</li>
<li>Android: Fixed crash which happens when loading a lot of asset bundles.  (743739) .</li>
<li>Android: Fixed UI flickering issue that was affecting specific Vivante devices.  (780633) .</li>
<li>Android: Skip dexing when exporting Android Project.  (746248, 785026) .</li>
<li>Android: Timeout no longer happens when an application is sent to the background.  (768217) .</li>
<li>Animation: Fixed out-of-bounds crash in the Animator .</li>
<li>Animation: Optimised the time to start play mode for a scene with lots of controllers.  (769964) .</li>
<li>AssetBundles: Removed sync load from AssetBundleRequest. Improves load times when doing multiple consecutive async loads from asset bundles.  (765367) .</li>
<li>Assets/VCS: Fixed an issue where changing date modified on directory meta file caused all files below that directory to be reprocessed. This was also affecting VCS.  (759044) .</li>
<li>Audio: Disabled sound manager watchdog.  (774356) .</li>
<li>Core: Added an extra check for null components while deactivating GameObjects to defend against crashes.</li>
<li>Global Illumination: Fixed an issue with the player looking different to the editor when using linear color space and Precomputed Realtime GI, with Baked GI disabled.  (724426, 728595, 738173, 753098) .</li>
<li>Graphics: In Editor play mode set the graphics device sRGB write mode to match the lighting mode e.g. enable sRGB write mode in linear lighting mode.  (754487) .</li>
<li>Graphics: Added functionality to D3D11 Native Interface to access the underlaying D3D11 texture for a RenderBuffer  (752855) .</li>
<li>Graphics: Fixed&nbsp;skinned mesh memory leak  (760665) .</li>
<li>Graphics: Fixed issue where enabling vertex compression for positions could result in geometry not being rendered.  (754928) .</li>
<li>IL2CPP : The static field initializer is less aggressive now.</li>
<li>IL2CPP: Fixed an issue whereby managed stack trace was not reported correctly on iOS.  (754539) .</li>
<li>iOS: Fixed character rigging, and updated SIMD math code.  (754816) .</li>
<li>iOS: Fixed crash in IL2CPP after the splash screen.  (752737, 751428) .</li>
<li>iOS: IL2CPP code generation fix for Xcode 7.3. </li>
<li>iOS: IPv6 compatibility fixes for .NET libraries and IL2CPP runtime. </li>
<li>iOS: Xcode 7.3 Build &amp; Run support.</li>
<li>Windows Store: Fixed AccessViolationException when initializing matchmaking in UNet.  (747549) .</li>
<li>Windows Store: RunInBackground option will be respected when application window looses focus, and if enabled, the application will keep updating. Note: if application window is minimized it will be still paused, because OS suspends the application.  (759166) .</li>
</ul>

#### Revision: ad2d0368e248
