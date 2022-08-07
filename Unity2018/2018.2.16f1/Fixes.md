# Unity 2018.2.16f1
https://unity3d.com/unity/whatsnew/unity-2018.2.16

## Fixes

<ul>
<li><p>AI: Fixed an issue with NavMeshObstacle carving that could create an unexpected boundary where one of the hull's corners or edges sits precisely on a NavMesh polygon edge. (<a href="https://issuetracker.unity3d.com/issues/a-navmeshobstacle-placed-at-a-specific-position-creates-a-boundary-on-an-unobstructed-navmesh">1078553</a>, 1097930)</p></li>
<li><p>AI: Fixed RemoveAllNavMeshData() not waiting for NavMeshObstacles to finish carving, causing a crash. (1075239)</p></li>
<li><p>Android: Fixed wrong path returned by IPostGenerateGradleAndroidProject.OnPostGenerateGradleAndroidProject during project export.</p></li>
<li><p>Android: Increased JVM heap size from 2gb to 4gb. (<a href="https://issuetracker.unity3d.com/issues/android-gradle-build-fails-when-building-project-with-asset-bundle">969563</a>)</p></li>
<li><p>Asset Import: Fixed scripts that are in special folders like Assets/Plugins/Android/ not being ignored during compilation. (<a href="https://issuetracker.unity3d.com/issues/2018-dot-2-the-condition-for-ignoring-importing-files-inside-assets-slash-plugins-slash-android-slash-stopped-working">1092532</a>)</p></li>
<li><p>Asset Import: Fixed the import of the root node rotation for assets with a shared avatar. (<a href="https://issuetracker.unity3d.com/issues/prefab-rotation-offset-is-ignored-on-prefab-instance-at-runtime">1077942</a>, 1095518)</p></li>
<li><p>Audio: Fixed FMOD shutdown to avoid a deadlock, which could causes freezes on Android. (<a href="https://issuetracker.unity3d.com/issues/android-google-play-video-recording-freezes-the-application-when-unlocking-the-device">1046752</a>, 1087597)</p></li>
<li><p>Cache Server: Fixed duplicate downloads of assets from Cache Server. (1084628)</p></li>
<li><p>IL2CPP: Add support for CultureInfo in WebGL when exceptions are disabled. (<a href="https://issuetracker.unity3d.com/issues/webgl-unitywebrequest-throws-an-exception-when-scripting-runtime-version-is-net-4-dot-x-equivalent">1083520</a>)</p></li>
<li><p>IL2CPP: COM Callable Wrappers for managed arrays now implement IReferenceArray interface. This fixes cases where Windows Runtime APIs expected objects to implement this interface, and if they don't, they report errors such as "Data of this type is not supported." and "Error trying to serialize the value to be written to the application data store". (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-msal-error-trying-to-serialize-the-value-to-be-written-to-the-application-data-store">1054327</a>)</p></li>
<li><p>IL2CPP: Fixed a call to GetGenericArguments on a MethodInfo not working for an inflated generic type. (1087317)</p></li>
<li><p>IL2CPP: Fixed COM Objects representing Windows.Foundation.IAsyncAction and Windows.Foundation.IAsyncOperation getting destroyed after converting them to System.Threading.Tasks.Task via "AsTask" extension method. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-runtime-failure-on-call-to-windows-dot-storage-dot-streams-dot-getresults">1086209</a>)</p></li>
<li><p>IL2CPP: Fixed Debug.WriteLine() not implemented. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-assertion-error-being-triggered-on-calling-debug-dot-writeline">1088770</a>)</p></li>
<li><p>IL2CPP: Fixed Marshal.SizeOf not supported for types with a generic base class when the base class does not use the generic type in any field. (<a href="https://issuetracker.unity3d.com/issues/marshal-dot-sizeof-causes-argumentexception-errors-in-il2cpp-builds">1083239</a>)</p></li>
<li><p>iOS: Added iPhone XR/XS/XS Max resolutions to Game View.</p></li>
<li><p>iOS: Fixed wrong Screen.safeArea on iPhone on Start(). (<a href="https://issuetracker.unity3d.com/issues/ios-wrong-screen-dot-safearea-on-iphone-on-start">1085662</a>)</p></li>
<li><p>PS4: Fixed render target clear with solid color wasn't cleared properly under Scriptable render pipeline. (1096478)</p></li>
<li><p>Shaders: Fixed loading shaders from AssetBundles that were created in 2017.2 not being allowed.. (1096787)</p></li>
</ul>

#### Revision: 39a4ac3d51f6
