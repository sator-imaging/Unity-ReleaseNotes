# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Audio

- [Fixes](#fixes)


### Fixes

*   AudioSource attached to a movie texture is no longer reporting false isPlaying.
*   Fixed audio sources referencing wrong clips when reusing cached sounds.
*   Effects now working audio sources, where ignoreListenerVolume is set.
*   WWW.audio now works on iPhone.
*   Fix rare crash when AudioSource.clip was reset in the same frame as the source was played.
*   DSP buffer settings set in 3.3 is now read correctly in 3.4.
*   Bitrate in .meta files are now serialized correctly.
*   Fixed FMOD errors when using AudioSource.PlayOneShot.