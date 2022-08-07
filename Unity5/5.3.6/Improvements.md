# Unity 5.3.6
https://unity3d.com/unity/whats-new/unity-5.3.6

## Improvements

<ul>
<li>Android:  Symbols for release libraries are now available in PlaybackEngines/AndroidPlayer/Variantions/*/Release/Symbols.</li>
<li>Audio:  Added ability to transition AudioMixer snapshots by scaled and unscaled time.</li>
<li>Audio:  Added virtualization of audio effects. For audio sources that are virtual because they have been culled due to low audibility or priority, attached effect components or spatializers are now also bypassed in order to save CPU use. The new behaviour is on by default, but can be turned off in the audio project settings.</li>
<li>Audio:  Audio clip waveform preview now displays the actual format used for compression when the default format isn’t available on a certain platform.</li>
<li>Audio:  Audio clips with the "Streaming" load type are no longer preloaded. This is done to reduce the number of open file handles in scenes referencing a large number of streamed clips. The behaviour is not affected except for a slight increase in playback delay of this type of audio clips.</li>
<li>Audio:  Fixed audio clip waveform preview rendering sync issues after import, and improved the way the waveforms are being rendered to be more dynamic and reveal more detail.</li>
<li>Audio:  Moved Preload Audio Data to the platform-specific settings section. The previous location was confusing as it was shown grayed-out in the inspector with a checkmark that depended on all overrides.</li>
<li>Audio:  SystemInfo now includes supportsAudio info.</li>
<li>GI:  Added a version number to the Lighting Data asset. Give the user a nice error message if their Lighting Data is out of date.</li>
<li>Graphics:  Documentation for Display API.</li>
<li>iOS:  Update Build and Run to work with Xcode 8</li>
<li>Lighting:  Improved an error message about invalid data when baking probes.</li>
<li>Runtime-Other:  Added diagnostic option to cmdline arguments -debugallocator [1/2] which helps to identify memory access issues in the engine on Windows and OSX x64 platforms.</li>
<li>Runtime:   During crashes even if the stack walking is aborted with error (RtlLookupFunctionEntry returned NULL function. Aborting stack walk), Unity will display stripped stack trace instead of displaying zero stack frames.</li>
<li>Shaders:  Removed an outdated comment in UnityStandardCore.cginc</li>
<li>VR:  Updated to Oculus Version 1.5.</li>
<li>VR:  Updated to version 1.4 of the Oculus API.</li>
<li>WebSocket:  Improved memory allocation and socket writing procedure (fixed not expected connection closing)</li>
<li>Windows Store:  Expanded UnityEngine.WSA.Cursor.SetCustomCursor, if you pass 0 to this function, it will restore the cursor to arror icon. (791792)</li>
<li>Windows Store:  Improved 'NULL != certificate' errors, it will now provide a human readable message why it failed to create a certificate. (792507) </li>
</ul>
