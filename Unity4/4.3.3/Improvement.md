# Unity 4.3.3

https://unity3d.com/unity/whats-new/unity-4.3.3

## Improvement



*   Windows Store Apps/Windows 8.1: SwapChainPanel is now supported, you can set via appCallbacks.SetSwapChainPanel
*   Windows Store Apps/WP8: When unloading unused assets, Unity will output asset names, which are still being used, but are not strongly referenced. That should help identifying problems, where some prefabs are being unloaded.
*   Windows Store Apps: Add "Unprocessed plugins" option in PlayerSettings, so you can specify plugin names, which shouldn't be processed, simply specify plugin file name, for ex., MyPlugin.dll. This should help workaround problems where Unity fails to preprocess an assembly, but actually doesn't need to do it.
*   Windows Store Apps: Added additional defines for scripts: UNITY\_METRO\_8\_0 - when building against Windows SDK 8.0, UNITY\_METRO\_8\_1 - when building against Windows SDK 8.1
*   Windows Store Apps: If you have different plugins for Windows 8 and Windows 8.1, you can place them accordingly to Assets\\Plugins\\Metro\\Win80, Assets\\Plugins\\Metro\\Win81, Unity will pick appropriate directory depending on the selected SDK.
*   WP8: Emulate DX11 level 9.3 graphics in editor to have features similar to actual device