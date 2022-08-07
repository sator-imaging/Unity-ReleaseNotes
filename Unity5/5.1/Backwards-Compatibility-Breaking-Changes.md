# Unity 5.1
https://unity3d.com/unity/whats-new/unity-5.1

## Backwards Compatibility Breaking Changes

<ul>
<li>Animation: Change the behaviour for humanoid controller with generic clip animating a human transform. Before the generic animation for the Human transform had a higher priority than the human animation. Now the Human animation always have the highest priority for humanoid rig overriding any generic animation for this transform, you should see a warning in the inspector if such case is detected with the name of the faulty animation clip and which transform is affected.</li>
<li>Physics: Modifying the HingeJoint Limit, Motor, Spring properties will no longer automatically enable the them. You now need to explicitly set HingeJoint.useLimit, useMotor, useSpring.</li>
<li>XboxOne: Unity is now built with the April 2015 XDK.  You will need to install the April 2015 XDK on your PC and use the same or later recovery on your console.</li>
</ul>
