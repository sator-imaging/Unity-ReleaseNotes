# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Rewrite of the GUI system



*   The existing GUI system (OnGUI) had its core rewritten, optimized and cleaned up. It uses less memory and induces less garbage collection cycles. In some cases we’ve seen it being 10x faster without GUILayout, and several times faster than previous version when GUILayout is used.
*   Note: this is not the “New GUI” that is coming to a later Unity 4.x release. It’s existing GUI, made much faster.