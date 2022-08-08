# Unity 5.6

https://unity3d.com/unity/whats-new/unity-5.6.0

## The following are changes and fixes to 5.6.0 features and regressions...

- [Fixes](#fixes)


### Fixes

*   2D: Fixed issues in Sorting Layers serialization when importing from Asset Bundles in Editor. [(885387)](https://issuetracker.unity3d.com/issues/asset-bundles-sprite-renderer-sorting-layer-is-gone-when-asset-is-loaded-from-asset-bundle)
*   AI: Fixed case of NavMesh not carving holes for smaller regions. [(885975)](https://issuetracker.unity3d.com/issues/android-inconsistencies-with-baked-navmeshes-on-mobile)
*   Android: Fixed reading assets from OBB (ApplicationPath). (893913)
*   Android: Removed internet permission in Android manifest for empty projects. (892203)
*   Editor: Fixed case of scene view gizmo for ParticleSystem box shape disappearing when pan tool was active or when rotating the view.
*   Editor: Fixed case of scene view handles for BoxCollider2D appearing in the wrong place, when part of a CompositeCollider2D with an offset that had non-uniform scale or off-axis rotation. [(893487)](https://issuetracker.unity3d.com/issues/box-manipulators-do-not-match-the-outline-and-position-of-the-composite-gizmo)
*   Editor: Fixed crash in profiler when enabling show-related objects. [(889027)](https://issuetracker.unity3d.com/issues/crash-on-profilerhistory-calculateselectedtimeandchart-after-clicking-on-profiled-function-with-show-related-objects-enabled)
*   GI: Fixed issue whereby the progress bar would get stuck when cancelling a baking job. [(876864)](https://issuetracker.unity3d.com/issues/auto-ui-progress-bar-gets-stuck-if-auto-mode-is-disabled-while-building-lighting)
*   GI: Fixed issue with Lightmasks being saved in the wrong color space. [(878494)](https://issuetracker.unity3d.com/issues/editor-manually-generated-lighting-looks-different-between-platforms)
*   iOS: Fixed Airplay mirroring mode when using Open GLES. [(788515)](https://issuetracker.unity3d.com/issues/ios-airplay-camera-dot-settargetbuffers-doesent-work-with-gles2-slash-3)
*   Kernel: Fixed crash when undoing a revert would cause components to be removed. [(870498)](https://issuetracker.unity3d.com/issues/physics-prefab-undo-crash-when-reverting-prefab-who-had-rigidbody-and-joint-deleted-and-then-undoing-the-revert)
*   Physics: CapsuleCollider2D now correctly calculates its mass when using auto-mass. [(890937)](https://issuetracker.unity3d.com/issues/auto-mass-calculates-the-incorrect-value-of-the-capsule-collider-2d)
*   Physics: Fixed case of OverlapPoint queries not taking into account any 'Edge Radius' on 2D colliders.
*   Video: Cured VideoPlayer crashes when calling videoPlayer.Prepare(). [(862078)](https://issuetracker.unity3d.com/issues/android-videoplayer-crashes-when-calling-videoplayer-dot-prepare)
*   Video: Fixed case of looped video crashing on 4th repeat on Galaxy Tab S (SM-T700). (891819)
*   Video: Fixed issue where Video Player didn't play on some devices when AutoGraphics API is enabled. [(888657)](https://issuetracker.unity3d.com/issues/android-video-player-doesnt-play-on-some-devices-when-autographics-api-is-enabled)
*   Video: Fixed issues with some devices not loading videos. (893966)
*   Video: Fixed VideoPlayback audio buffer overflow while playing video in Editor Play mode. (893862)
*   VR: Fixed back button / close button behavior on Daydream to resolve app submission issues. (893219)

#### Revision: 497a0f351392