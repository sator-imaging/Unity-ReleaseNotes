# Unity 3.5.5
https://unity3d.com/unity/whats-new/unity-3.5.5

## Known Issues

<ul>
<li>Mobile: We changed the way Texture2D.ReadPixels works. Now, if you do call it during Update (or, generally, not during rendering frame) to grab the copy of the screen, the call will be deferred to the end of the current frame. Due to this, logic behind Apply was changed too.</li>
<li>What you need to do if you use ReadPixels to read pixels from the screen: 
<ul>
<li>if you just grab screen copy and call Apply, you are good to go: both calls will be deferred to the end of the frame</li>
<li>if you grab screen copy, and do something with it, and call Apply after that: you need to defer all this to the next frame. The easiest way is to use coroutines with yield in between ReadPixels and your operations plus Apply.</li>
<li>On the other hand, you can always do ReadPixels in Camera's OnPostRender, or when you have active RenderTexture.</li>
</ul></li>
<li>Editor: We dropped IMGTech standalone PVR Compressor, and built our own using their PVRTCLib. We do handle most of the options, but we do allow only one form of args with params: -arg</li>
</ul>
