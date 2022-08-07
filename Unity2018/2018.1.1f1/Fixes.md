# Unity 2018.1.1f1
https://unity3d.com/unity/whatsnew/unity-2018.1.1

## Fixes

<ul>
<li>Editor: Fixed content drawn with OnSceneGUI not looking correct and consistent whether the project color space is Gamma or Linear.(1018625)</li>
<li>Player: Fixed imbalanced platform profile markers in user scripts. (1005409)</li>
<li>Web: Fixed crash when aborting AssetBundle download using UnityWebRequest. (1017468)</li>
<li>Particles: Improved logic for when Automatic Culling can be used with non-randomized emission. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991235">991235</a>)</li>
<li>Particles: Fixed particle collision not being detected when Particle System used negative scale. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985049">985049</a>)</li>
<li>Particles: Fixed particles occasionally flickering when they have a random start life time and sort mode was set to Youngest or Oldest in front. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/988874">988874</a>)</li>
<li>Particles: Fixed prefabs with a ParticleSystem creating duplicate entries into its serialization after each modification. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989631">989631</a>)</li>
<li>Particles: Fixed particles/alpha blended material inverting colors of other blended objects, when using HDR. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/967476">967476</a>)</li>
<li>Editor: Fixed PresetLibraries classes not being handled correctly by the Preset UI and will be excluded at the moment. (1020017)</li>
<li>Editor: Foxed closing the Create new Preset window logging a Layout error in the console. (1022087)</li>
<li>XR: Fixed XR.WSA.WorldManager.OnPositionalLocatorStateChanged() not getting called when state changes back to active. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/998331">998331</a>)</li>
</ul>

#### Revision: b8cbb5de9840
