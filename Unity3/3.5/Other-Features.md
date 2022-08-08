# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Other Features



*   Upgraded to MonoDevelop 2.8.2.
*   Generic Social API added, which supports GameCenter only at the moment and Xbox Live support will be enabled later. Limited dummy functionality runs on unsupported platforms (so code is testable in the Editor for example). Third parties can implement the interface to add support for their implementation on any platform.
*   Physics: Added ConfigurableJoint.swapBodies property to make the joint act as if the two connected Rigidbodies were swapped.
*   AssetPostProcessor can now be versioned. See AssetPostProcessor.GetVersion for details.
*   Asset Server can now be used with Cache Server. Note that this requires committing all assets to the server project after upgrading to 3.5 and that the server project will not be usable by older Unity versions after that commit. So remember to back up everything, including the server project.
*   Added Application.StreamingAssetPath which points to the location of the data in the Assets/StreamingAssets folder on all build targets.
*   IME: Added Input.isIMESelected to determine if the user has currently enabled IME conversion mode for keyboard input.
*   All Editor Settings files that need to be versioned have been moved into a ProjectSettings folder.
    *   If upgrading an existing project the current settings files will be copied to the new folder.
    *   If you are using version control you should upgrade your project by opening it in the editor and then you should remove the old settings files from version control and simply add the ProjectSettings folder.
    *   Conclusion: All you need to add to version control in 3.5 is your Assets folder and ProjectSettings folder.