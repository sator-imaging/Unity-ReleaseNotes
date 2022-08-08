# Unity 5.5.1

https://unity3d.com/unity/whats-new/unity-5.5.1

## Improvements



*   Graphics: Added support for feature level 11.1 on D3D11/D3D12. This brings native support for RGB565 and ARGB1555 RenderTexture formats. Note that this does not render correctly for ARGB4444 which will be fixed in one of the future releases.
*   Graphics: An error message is shown in the console for platforms that don't support linear color space rendering with OpenGL ES. (757055)
*   macOS/iOS/tvOS: Allow using Xcode's manual signing workflow by specifying a provisioning profile in Player Settings.
*   Metal: Improved handling of transparent rendering after post-opaque image effects when using MSAA.
*   Shaders: If an unknown/unhandled error occurs during shader compilation, append it to the shader compiler error message. This gives some context on what might be wrong in the shader.
*   Shaders: Optimized in-editor import, load time and memory usage for shaders with massive amounts of potential variants.
*   Unity Ads: Updated native binaries to version 2.0.6.