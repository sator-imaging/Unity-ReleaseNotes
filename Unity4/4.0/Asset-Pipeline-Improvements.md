# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Asset Pipeline Improvements



*   Added userData string property to AssetImporter, use this to pass per asset data to asset post processor.
*   Manual asset reimport (via context menu) always reimports, even if cache server already has the result.
*   Optimized file system performance of asset imports. Library/cache and Library/previews folders are gone; all imported results are in Library/metadata.