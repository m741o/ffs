# guide

# step 1 (changing `.json`'s values, needs an injector)
_**MUST change**_
- have roblox fps cap at 240

- change `FStringGraphicsDisableUnalignedDxtGPUNameBlacklist` & `FStringDebugGraphicsPreferredGPUName` to full GPU name, and change these depending on it (delete if lower than smallest amount of gb)
```
DFIntRenderTextureTotalBudgetMB
  4 GB VRAM → 1024
  8+ GB VRAM → 4096
DFIntRenderTextureTotalBudgetCount
  4 GB VRAM → 16384
  8+ GB VRAM → 32768
DFIntRenderTextureLoadingBudgetMB
  4 GB VRAM → 768
  8+ GB VRAM → 2048
DFIntRenderTextureLoadingMaxMB
  4 GB VRAM → 384
  8+ GB VRAM → 1024
  ```

- delete `DFFlagAlwaysSkipDiskCache`  if you have an HDD, add if you're on SSD

- [calculate frametime](https://fflag-frametime-calc.netlify.app/), change them, & add `DFIntGraphicsOptimizationModeFRMFrameRateTarget` to your monitor refresh rate (don't add if 60hz)

- [calculate runtime](https://configurate-roblox-runtime.vercel.app/), change them, & remove the commas

- change `DFIntCanHideGuiGroupId` to the ID of a group you're in

- change these accordingly to your RAM (delete if lower than smallest amount of gb)
```
DFIntMemoryUtilityCurveBaseHundrethsPercent:
  4 GB → 5000
  8+ GB → 2500
DFIntMemoryUtilityCurveTotalMemoryReserve:
  4 GB → 51200
  8 GB → 102400
  16+ GB → 204800
DFIntMemCacheMaxCapacityMB
  16 GB → 256
  32+ GB → 512
FIntDefaultMeshCacheSizeMB
  16 GB → 256
  32+ GB → 512
FIntAnimationClipCacheBytes
  16 GB → 250000000
  32+ GB → 500000000
```

- change this accordingly to your CPU cores
```
FIntLuaGcParallelMinMultiTasks
  2 core CPU  → "1"
  4+ core CPU → "4"
```
- change these 5 ffs to your logical CPU logical processors **(8 | 12 | 16 | 24)**
```
DFIntRuntimeConcurrency: 8 | 12 | 16 | 24
FIntTaskSchedulerThreadMin: 7 | 11 | 15 | 23
FIntTaskSchedulerAutoThreadLimit: 8 | 12 | 16 | 24
FIntTaskSchedulerAsyncTasksMinimumThreadCount: 3 | 4 | 4 | 12
DFIntTaskSchedulerJobInitThreads: 7 | 11 | 15 | 23
DFIntTaskSchedulerJobInGameThreads: 4 | 6 | 8 | 16
```

- delete these in case of not having 10gb of free disk space
```
DFIntRbxStorageDBMaxCapacityMB
DFIntRbxStoragePeriodicCleanupIntervalSec
FFlagRbxStorageRemoveLargeDb
FIntRbxStorageCleanupDelaySeconds
FIntRbxStorageDBPreallocateMB
FIntRbxStorageDeleteOldCacheMB
FIntRbxStorageRemoveLargeDbThresholdMB
```

- delete if crashing: `DFIntQosMaxEvents`
_**optional**_
- remove these 3 ffs to avoid possible bans (due to network ownership)
```
DFIntMinClientSimulationRadius
DFIntMinimalSimRadiusBuffer
DFIntMaxClientSimulationRadius
```

- add `DFIntTaskSchedulerTargetFps` for custom fps cap


# step 2 (adding whitelisted fflags)
- put `ClientAppSettings.json` into `ClientSettings` folder in `%localappdata%/roblox`
