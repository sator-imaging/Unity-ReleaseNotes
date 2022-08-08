# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Animation Features

- [New Animation Window has arrived](#new-animation-window-has-arrived)
- [Mecanim improvements](#mecanim-improvements)


### New Animation Window has arrived

*   Heavily influenced by the standard "dope sheets".
*   Only animated properties are shown in the property view (left side of the window).
*   Sprite animation is possible by animating the SpriteRendrerer component.
*   Sprites are shown in the dopesheet when SpriteRenderer is unfolded from the left side property view.
*   'Add Curve' menu added. Shows all properties that can be animated on selected GameObject.
*   Animation Window now supports Mecanim. Animations can be added to the animator controller from the Animation window. Animations can be modified in the AnimationWindow too.
*   Added 'Curves' button to menu bar. Changes between dopesheet and curve editor. 'C' key assigned for keyboard shortcut
*   Added 'Samples' field to menu bar. Changes clip sample value per second.
*   Added toggle field for animating boolean properties. Created boolean curves use 'Constant' as default key tangent.
*   'F' will focus on whole clip, or shown curves, if nothing is selected

### Mecanim improvements

*   Add a new option "Optimize Game Objects" in ModelImporter inspector. In short, this makes character rigs much faster.
    *   When turned on, the game object transform hierarchy of the imported character will be removed and is instead stored in the Avatar and Animator component.
    *   The SkinnedMeshRenderers of the character will then directly use the Mecanim internal skeleton, so that we can get rid of all the Transforms which used to be there, representing all the bones.
    *   This option will improve the performance of the animated characters. It is recommended to turn it on for the final product. In optimized mode skinned mesh matrix extraction is also multithreaded.
    *   When "Optimize Game Objects" is turned on, the user can specify a list of "Extra Transforms to Expose" in ModelImporter inspector. For example, if you want to attach a sword to the right hand, this acts as a mount point. The exposed transform is flattened in the game object hierarchy, even though it might be somewhere deep in skeleton hierarchy.
*   Mecanim supports animating any property including blend shapes properties, camera properties, script float properties, lights and most other float properties on components.
*   Support for events! Events are created in the animation window for writable Animation Clips attach to an Animator. Can also add AnimationEvents directly in the animation importer.
*   Various performance optimizations, especially in regards to generic mode.
*   Added Animator.Play and Animator.CrossFade scripting functions. These functions allow you at runtime to transition to any state in your controller.
*   Added AnimatorOverrideController, an AnimatorOverrideController allow you to override any clip from a controller with another one.
*   Loop time vs Loop pose, When an animation clip is already looping, no need to activate Loop Pose, Loop Time will make clip looping without modifying the pose.
*   Trigger parameter, a trigger is a boolean parameter that is reset by the controller when consumed by a transition.