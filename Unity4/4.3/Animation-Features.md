# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Animation Features


### New Animation Window has arrived
<ul>
<li>Heavily influenced by the standard "dope sheets".</li>
<li>Only animated properties are shown in the property view (left side of the window).</li>
<li>Sprite animation is possible by animating the SpriteRendrerer component.</li>
<li>Sprites are shown in the dopesheet when SpriteRenderer is unfolded from the left side property view.</li>
<li>'Add Curve' menu added. Shows all properties that can be animated on selected GameObject.</li>
<li>Animation Window now supports Mecanim. Animations can be added to the animator controller from the Animation window. Animations can be modified in the AnimationWindow too.</li>
<li>Added 'Curves' button to menu bar. Changes between dopesheet and curve editor. 'C' key assigned for keyboard shortcut</li>
<li>Added 'Samples' field to menu bar. Changes clip sample value per second.</li>
<li>Added toggle field for animating boolean properties. Created boolean curves use 'Constant' as default key tangent.</li>
<li>'F' will focus on whole clip, or shown curves, if nothing is selected</li>
</ul>

### Mecanim improvements
<ul>
<li>Add a new option "Optimize Game Objects" in ModelImporter inspector. In short, this makes character rigs much faster. 
<ul>
<li>When turned on, the game object transform hierarchy of the imported character will be removed and is instead stored in the Avatar and Animator component.</li>
<li>The SkinnedMeshRenderers of the character will then directly use the Mecanim internal skeleton, so that we can get rid of all the Transforms which used to be there, representing all the bones.</li>
<li>This option will improve the performance of the animated characters. It is recommended to turn it on for the final product. In optimized mode skinned mesh matrix extraction is also multithreaded.</li>
<li>When "Optimize Game Objects" is turned on, the user can specify a list of "Extra Transforms to Expose" in ModelImporter inspector. For example, if you want to attach a sword to the right hand, this acts as a mount point. The exposed transform is flattened in the game object hierarchy, even though it might be somewhere deep in skeleton hierarchy.</li>
</ul></li>
<li>Mecanim supports animating any property including blend shapes properties, camera properties, script float properties, lights and most other float properties on components.</li>
<li>Support for events! Events are created in the animation window for writable Animation Clips attach to an Animator. Can also add AnimationEvents directly in the animation importer.</li>
<li>Various performance optimizations, especially in regards to generic mode.</li>
<li>Added Animator.Play and Animator.CrossFade scripting functions. These functions allow you at runtime to transition to any state in your controller.</li>
<li>Added AnimatorOverrideController, an AnimatorOverrideController allow you to override any clip from a controller with another one.</li>
<li>Loop time vs Loop pose, When an animation clip is already looping, no need to activate Loop Pose, Loop Time will make clip looping without modifying the pose.</li>
<li>Trigger parameter, a trigger is a boolean parameter that is reset by the controller when consumed by a transition.</li>
</ul>
