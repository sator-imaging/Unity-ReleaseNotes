# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## New Animation System



*   Once imported as muscle clips, animations can be used with all humanoid characters with no additional conversions needed.
    *   Use the same animations on different proportion characters with no overhead or need for storing multiple versions of the clip.
    *   Map the bones of your model to human muscles with a single click, or fine tune the setup for full control.
*   Slice up your authored or motion-captured animations directly inside Unity with the industry's best tool for the job.
    *   Preview the animation as your drag the ranges of a clip.
    *   Indicators for pose looping quality and motion looping quality lets you easily pick the range with optimal looping.
    *   Differences between start and end pose is smoothed out by the importer to ensure perfect looping.
*   Support for arbitrary animations:
    *   Support for Generic Skeletons.
    *   Support for human avatars with additionals bones (“hybrids”).
    *   Preview of generic or hybrid skeleton in Animation Clip, Blend Tree and Transition inspector.
    *   Multiple IK layer solving (changes to OnAvatarIK() API).
    *   Supports Culling (Animator.cullingMode = AnimatorCullingMode).