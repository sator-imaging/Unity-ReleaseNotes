# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Known Issues



*   Android: Handheld.use32bitDisplayBuffer (or otherwise recreating the GL context, like changing the AA settings) will result in artifacts and/or crashes if used with Image Filters.
*   Android: Microphone recording is known to crash on some devices, notably, Samsung Galaxy Tab and Galaxy Nexus.
*   Lightmapping: Texel density is not shown on skinned meshes marked lightmap static.
*   Model Import: Autodesk 3ds Max interprets Tiling value differently than Maya (or Unity) - it calculates tiling assuming that pivot of the texture is in the middle of the texture. The pivot for tiling is on the left lower corner in Unity.
*   Model Import: We made fixes to COLLADA import which affects naming of imported objects, which may result in broken prefab connections. This mostly affects COLLADA files exported from modo and direct modo file import into Unity.
*   Model Import: You can not import model materials full transparency (i.e. alpha=0), it will be treated as alpha=1. Unity works this way for backwards compatibility with older 3d packages, which write incorrect transparency factor.
*   Model Import: You can not import model material Opacity texture and Opacity factor at the same time from Autodesk 3ds Max - it doesn't export Opacity value (TransparencyFactor), when Opacity texture is set.
*   Mac OS X 10.5: Building Webplayer, Webplayer Streamed, Webplayer Offline Development and Mac OS Widget doesn't work.