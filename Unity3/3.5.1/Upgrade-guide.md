# Unity 3.5.1
https://unity3d.com/unity/whats-new/unity-3.5.1

## Upgrade guide


#### In Unity 3.4 realtime lights were not affecting static objects. In Unity 3.5 realtime lights always affect static and dynamic objects.

#### The result of this is that if you had previously setup your lighting to work around this bug, then you will now get worse performance as you will receive the lighting twice. It will also look different since your lights will be added twice to the scene.

#### The correct way to use these lights is to use a single auto directional light and remove the realtime only light.

#### If you wish to have different realtime lighting than static lighting, you should using light culling masks to affect only dynamic objects.

#### Upgrade Guide
