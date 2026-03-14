# guide

# step 1 (changing `.json`'s values, needs an injector)
_**MUST change**_
- have roblox fps cap at 240

- change `FStringGraphicsDisableUnalignedDxtGPUNameBlacklist` & `FStringDebugGraphicsPreferredGPUName` to full GPU name

- delete `DFFlagAlwaysSkipDiskCache`  if you have an HDD

- [calculate frametime](https://fflag-frametime-calc.netlify.app/), change them, & add `DFIntGraphicsOptimizationModeFRMFrameRateTarget` to your monitor refresh rate (don't add if 60hz)

- change `DFIntCanHideGuiGroupId` to the ID of a group you're in

- change these 5 ffs to your logical CPU logical processors **(8 | 12 | 16 | 24)**
```
DFIntRuntimeConcurrency: 8 | 12 | 16 | 24
FIntTaskSchedulerThreadMin: 7 | 11 | 15 | 23
FIntTaskSchedulerAutoThreadLimit: 8 | 12 | 16 | 24
FIntTaskSchedulerAsyncTasksMinimumThreadCount: 3 | 4 | 4 | 12
DFIntTaskSchedulerJobInitThreads: 7 | 11 | 15 | 23
DFIntTaskSchedulerJobInGameThreads: 4 | 6 | 8 | 16
```

_**optional**_
- remove these 3 ffs to avoid bans (due to network ownership)
```
DFIntMinClientSimulationRadius
DFIntMinimalSimRadiusBuffer
DFIntMaxClientSimulationRadius
```

- add `DFIntTaskSchedulerTargetFps` for custom fps cap

- [calculate runtime](https://configurate-roblox-runtime.vercel.app/), change them, & remove the commas


# step 2 (adding whitelisted fflags)
- put `ClientAppSettings.json` into `ClientSettings` folder in `%localappdata%/roblox`
