# Unity 5.3.6

https://unity3d.com/unity/whats-new/unity-5.3.6

## Improvements



*   Android: Symbols for release libraries are now available in PlaybackEngines/AndroidPlayer/Variantions/\*/Release/Symbols.
*   Audio: Added ability to transition AudioMixer snapshots by scaled and unscaled time.
*   Audio: Added virtualization of audio effects. For audio sources that are virtual because they have been culled due to low audibility or priority, attached effect components or spatializers are now also bypassed in order to save CPU use. The new behaviour is on by default, but can be turned off in the audio project settings.
*   Audio: Audio clip waveform preview now displays the actual format used for compression when the default format isn’t available on a certain platform.
*   Audio: Audio clips with the "Streaming" load type are no longer preloaded. This is done to reduce the number of open file handles in scenes referencing a large number of streamed clips. The behaviour is not affected except for a slight increase in playback delay of this type of audio clips.
*   Audio: Fixed audio clip waveform preview rendering sync issues after import, and improved the way the waveforms are being rendered to be more dynamic and reveal more detail.
*   Audio: Moved Preload Audio Data to the platform-specific settings section. The previous location was confusing as it was shown grayed-out in the inspector with a checkmark that depended on all overrides.
*   Audio: SystemInfo now includes supportsAudio info.
*   GI: Added a version number to the Lighting Data asset. Give the user a nice error message if their Lighting Data is out of date.
*   Graphics: Documentation for Display API.
*   iOS: Update Build and Run to work with Xcode 8
*   Lighting: Improved an error message about invalid data when baking probes.
*   Runtime-Other: Added diagnostic option to cmdline arguments -debugallocator \[1/2\] which helps to identify memory access issues in the engine on Windows and OSX x64 platforms.
*   Runtime: During crashes even if the stack walking is aborted with error (RtlLookupFunctionEntry returned NULL function. Aborting stack walk), Unity will display stripped stack trace instead of displaying zero stack frames.
*   Shaders: Removed an outdated comment in UnityStandardCore.cginc
*   VR: Updated to Oculus Version 1.5.
*   VR: Updated to version 1.4 of the Oculus API.
*   WebSocket: Improved memory allocation and socket writing procedure (fixed not expected connection closing)
*   Windows Store: Expanded UnityEngine.WSA.Cursor.SetCustomCursor, if you pass 0 to this function, it will restore the cursor to arror icon. (791792)
*   Windows Store: Improved 'NULL != certificate' errors, it will now provide a human readable message why it failed to create a certificate. (792507)