# step 1 (changing `.json`'s values, needs an injector)

_**MUST change**_
- have roblox fps cap at 240

- change `DFIntCanHideGuiGroupId` to the ID of a group you're in

- [calculate frametime](https://fflag-frametime-calc.netlify.app/), change them, & add `DFIntGraphicsOptimizationModeFRMFrameRateTarget` to your monitor refresh rate. after change `FIntPerformanceControlTargetFrameTimeCeilingHundredthsMs` with calculation (1000000 / refresh_rate)

- [calculate runtime](https://configurate-roblox-runtime.vercel.app/), change them, & remove the commas.

- take your internet upload speed in mbps and multiply by 125000, then change `FIntDataSenderMaxBandwidthBps` to that value

- change `FStringGraphicsDisableUnalignedDxtGPUNameBlacklist`,  `FStringDebugGraphicsPreferredGPUName` & `FStringDisableHQShadersDx11List` to full GPU name, and change these depending on it **(fflag | formula)**
```
FIntRenderTextureTotalBudgetMB | VRAM_GB * 512
FIntRenderTextureTotalBudgetCount | VRAM_GB * 4096
FIntRenderTextureLoadingBudgetMB | VRAM_GB * 256 (max cap 2048)
FIntRenderTextureLoadingMaxMB | VRAM_GB * 128 (max cap 1024)
```

- change these accordingly to your RAM **(fflag | formula)**
```
FIntMemoryUtilityCurveBaseHundrethsPercent | 16000000 / RAM_MB (min cap 2500)
FIntMemoryUtilityCurveTotalMemoryReserve | RAM_MB * 12.8
FIntMemCacheMaxCapacityMB | RAM_GB * 24 (min 128)
FIntDefaultMeshCacheSizeMB | RAM_GB * 24 (min 128)
DFIntAnimationClipCacheBytes | RAM_GB * 23437500
FIntMemoryPressureTriggerMB | RAM_MB * 0.4096
FIntFreeOsMemPercentageBufferPercentage | RAM_GB * 2
FIntLuauGcGoal | RAM_GB * 128
```

- change these accordingly to cpu cores **(fflag | formula)**
```
FIntAnimationParallelThreadMax | CPU_CORES
FIntSimWorldTaskQueueParallelTasks | CPU_CORES
FIntPhysicsReceiveNumParallelTasks | CPU_CORES
FIntLuaGcParallelMinMultiTasks | 1 if cores < 4 else 4
```

- change these accordingly to CPU logical processors **(fflag | formula)**
```
FIntRuntimeConcurrency | CPU_THREADS
FIntTaskSchedulerThreadMin | CPU_THREADS - 1
FIntTaskSchedulerAutoThreadLimit | CPU_THREADS
FIntTaskSchedulerJobInitThreads | CPU_THREADS - 1
FIntInterpolationNumParallelTasks | CPU_THREADS - 1
FIntTaskSchedulerJobInGameThreads | CPU_THREADS / 2
FIntParallelAdaptiveInterpolationBatchCount | CPU_THREADS * 12.5
FIntTaskSchedulerAsyncTasksMinimumThreadCount | 1 | 1 | 4 | 4 | 8 | 12 | SEE FOLLOWING TABLE: (4 | 8 | 12 | 16 | 24 | 32)
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
