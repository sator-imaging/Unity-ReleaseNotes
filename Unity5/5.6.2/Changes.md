# Unity 5.6.2
https://unity3d.com/unity/whats-new/unity-5.6.2

## Changes

<ul>
<li>GI: Added support for LOD baking in Progressive Lightmapper. Light Probes are not necessary anymore when baking LODs using Progressive Lightmapper.</li>
<li>GI: Support for double sided materials in Progressive Lightmapper. Added a new material setting that causes lighting to interact with backfaces. When enabled, both sides of the geometry get accounted for when calculating Global Illumination. Backfaces do not count as invalid when seen from other objects. Backface rendering is not controlled by this setting nor will backfaces be represented in the lightmaps. Backfaces bounce light using the same emission and albedo as frontfaces.</li>
</ul>
