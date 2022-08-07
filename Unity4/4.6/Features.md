# Unity 4.6
https://unity3d.com/unity/whats-new/unity-4.6

## Features

<ul>
<li>New UI System: Design UIs for your game or application using Unity's powerful new component based UI framework and visual tools.  
<ul>
<li>Create UIs in screen space with or without perspective and with support for pixel perfect alignment, or in world space for simple creation of in-world interactions.</li>
<li>The layout system combines anchoring to sides, corners, or custom points in the parent container with the ability to stretch to a percentage or full extent of the parent width or height. Simple Scene View handles allows intuitive visual control and tweaking of the positional behavior. </li>
<li>Build up designs and customized controls composed of image, text, masking, and effects. All graphical components have full support for custom materials and lighting.</li>
<li>Built-in controls for buttons, sliders, scroll views, input fields and more have been designed for full cross platform deployment, supporting touch controls (where the Unity touch API is supported) and mouse as well as directional navigation such as arrow keys or gamepad controls.</li>
<li>The UI system integrates with Unity’s animation smoothly, meaning that you can use state machines and other animation features to control your UI elements and panels. </li>
<li>The UI system is designed to be extensible so that it can meet the needs of your projects. Combine existing UI elements together to create new controls, extend existing controls, or write new controls from scratch.</li>
<li>Easily set up callbacks for your UI controls in the Inspector using the new persistent delegate system. A lot of functionality can be hooked up to your UI with no programming needed!</li>
</ul></li>
<li>New Rect Tool: In previous versions, rect handles were used only in 2D mode and only for SpriteRenderers. With the introduction of the new UI system that is a hybrid of 2D and 3D, more explicit control is needed to be able to efficiently position elements. The new Rect tool in the main Unity toolbar can be used for sprites, UI elements, and any other object as well. The rect handles have also received an overhaul to be more consistent with the other tools, and to be more useful for a wide variety of uses. 
<ul>
<li>Rect handles now support Pivot/Center mode as set in the toolbar as well Local/Global mode as set in the toolbar. </li>
<li>Rect handle squashing (holding Control/Command while dragging a side) now supports preserving volume rather than area when holding down Shift. </li>
<li>Rect handles for objects that appear small in the Scene View now show a disc handle that can be used to move the object in the plane of the rect. When zooming further in, the disc will fade out as the normal rect handles fade in. </li>
</ul></li>
<li>Extensible Event Messaging System: Use and extend the new Event System framework. The system is used for the new UI to send and receive events, but it can be extended to support custom input devices and custom event logic. 
<ul>
<li>Inbuilt support for touch and standalone.</li>
<li>Supports 2d, 3d, and UI components.</li>
<li>Extensible; add custom input handling and custom events.</li>
</ul></li>
<li>Persistent Delegates (Unity Events): A new way to set callbacks via the UI and have them be built into a player. This helps non-programmers quickly add functionality to your application within the editor.</li>
<li>New Android Build Targets: Support has been added for x86 as a build target. Fat binary support (x86+ARMv7) is supported as well and is the new default.</li>
</ul>
