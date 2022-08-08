# Unity 5.4.6

https://unity3d.com/unity/whats-new/unity-5.4.6

## Known Issue



#### There is a known incompatibility between Unity and Visual Studio 2017 update 3 when targeting UWP, using .NET scripting backend and building generated Visual Studio project. Please note that IL2CPP scripting backend is not affected. For more information about this issue, please refer to this forum post: https://forum.unity.com/threads/net-scripting-backend-and-visual-studio-2017-3-incompatibility.487833/

#### Workaround: Modify HKEY\_LOCAL\_MACHINE\\SOFTWARE\\WOW6432Node\\Microsoft\\Microsoft SDKs\\Windows\\v10.0\\ProductVersion to version older than 10.0.15063. The version provided should be installed. You can find all installed versions here - C:\\Program Files (x86)\\Windows Kits\\10\\Platforms\\UAP

#### Revision: 7c5210d1343f