# Unity 4.1

https://unity3d.com/unity/whats-new/unity-4.1

## Upgrade Notes



*   If your project uses shader replacement it will now by default use the camera settings for which render path to use. If the replacement shader you use does not support the given render path then the object will not be rendered. If you are using a simple (non-surface) shader for your shader replace set the replacement camera to forward rendering mode.
*   When using shader replacement image effects will now be applied to the resultant render output.