# Unity 2021.3.55f1 LTS
Published at Tue, 05 Aug 2025 14:36:32 GMT  
https://unity.com/releases/editor/whats-new/2021.3.55

# Known Issues in 2021.3.55f1

- DirectX12: Increased Memory usage when Update Mode 'On Demand' Realtime lights are used and DX12 API is selected
    ([UUM-90065](https://issuetracker.unity3d.com/issues/increased-memory-usage-when-update-mode-on-demand-realtime-lights-are-used-and-dx12-api-is-selected))



# 2021.3.55f1 Release Notes

## Fixes

- Android: Fixed warning showing libraries as not 16 KB page aligned when they have been updated externally.
    ([UUM-111393](https://issuetracker.unity3d.com/issues/android-native-libraries-dot-so-are-not-checked-for-16kb-alignment-when-modified-externally))

- Editor: Updated 7-Zip to 25.00.

- Graphics: Fixed crash after disconnecting an external display on Android.
    ([UUM-110456](https://issuetracker.unity3d.com/issues/android-crash-or-freeze-when-disconnecting-an-external-monitor-from-an-android-device))

- iOS: Fixed a crash when loading achievements from GameCenter multiple times.
    ([UUM-105560](https://issuetracker.unity3d.com/issues/ios-application-frequently-crashes-on-social-dot-loadachievements-call-when-many-achievements-are-registered))

- Scripting: Fixed ObjectPool clear timing in no domain reload environment.
    ([UUM-111093](https://issuetracker.unity3d.com/issues/objectpools-pool-is-destroyed-when-entering-play-mode-without-reloading-domain))




## Package changes in 2021.3.55f1

## Packages updated

- com.unity.netcode.gameobjects: [1.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.13//changelog/CHANGELOG.html) to [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@1.14//changelog/CHANGELOG.html)