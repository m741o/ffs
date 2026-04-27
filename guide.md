# step 1 (changing `.json`'s values, needs an injector)

_**MUST change**_
- have roblox fps cap at 240

- change `DFIntCanHideGuiGroupId` to the ID of a group you're in

- [calculate frametime](https://fflag-frametime-calc.netlify.app/), change them, & add `DFIntGraphicsOptimizationModeFRMFrameRateTarget` to your monitor refresh rate

- [calculate runtime](https://configurate-roblox-runtime.vercel.app/), change them, & remove the commas

- change `FStringGraphicsDisableUnalignedDxtGPUNameBlacklist` & `FStringDebugGraphicsPreferredGPUName` to full GPU name, and change these depending on it (delete if lower than smallest amount of gb) **(4 | 8)**
```
DFIntRenderTextureTotalBudgetMB: 1024 | 4096
DFIntRenderTextureTotalBudgetCount: 16384 | 32768
DFIntRenderTextureLoadingBudgetMB: 768 | 2048
DFIntRenderTextureLoadingMaxMB: 384 | 1024
```

- change these accordingly to your RAM (delete if lower than smallest amount of gb) **(4 | 8 | 16 | 32)**
```
DFIntMemoryUtilityCurveBaseHundrethsPercent: 5000 | 2500 | ? | ?
DFIntMemoryUtilityCurveTotalMemoryReserve: 51200 | 102400 | 204800 | ?
DFIntMemCacheMaxCapacityMB: ? | ? | 256 | 512
FIntDefaultMeshCacheSizeMB: ? | ? | 256 | 512
FIntAnimationClipCacheBytes: ? | ? | 250000000 | 500000000
```

- change this accordingly to your CPU cores (2 | 4)
```
FIntLuaGcParallelMinMultiTasks: 1 | 4
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
DFIntRbxStoragePeriodicCleanupIntervalSec
FFlagRbxStorageRemoveLargeDb
FIntRbxStorageCleanupDelaySeconds
FIntRbxStorageDeleteOldCacheMB
FIntRbxStorageRemoveLargeDbThresholdMB
```


_**optional**_
- remove these 3 ffs to avoid possible bans (due to network ownership)
```
DFIntMinClientSimulationRadius
DFIntMinimalSimRadiusBuffer
DFIntMaxClientSimulationRadius
```

- delete if crashing: `DFIntQosMaxEvents`


# step 2 (adding whitelisted fflags)
- put `ClientAppSettings.json` into `ClientSettings` folder in your current version at `%localappdata%/roblox/versions`
