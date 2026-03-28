# for your own custom list, USE `guide.md` FIRST BEFORE ADDING ANYTHING ELSE

# illegals in flemish bot (<@1285938242801242194>)
```
DFIntGameNetLocalSpaceMaxSendIndex
DFIntMaximumUnstickForceInGs
DFIntMaximumFreefallMoveTimeInTenths
FFlagDebugHumanoidRendering
DFFlagDebugEnableInterpThrottle
FFlagDebugAvatarChatVisualization
DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth
DFIntDebugSimPhysicsSteppingMethodOverride
DFIntPhysicsDecompForceUpgradeVersion
DFIntSmoothTerrainPhysicsRayAabbSlop
DFIntMaxMissedWorldStepsRemembered
DFIntSolidFloorPercentForceApplication
DFIntNonSolidFloorPercentForceApplication
```

## reduced animation latency
```json
{
  	"DFIntAnimationRateLimiterAssertAmount": "0",
  	"DFIntAnimationRateLimiterMaxAmount": "2147483647",
  	"DFIntAnimationRateLimiterSeconds": "0"
}
```

## better replication
```json
{
  	"DFFlagFasterReplicatorStringStream": "True",
  	"FFlagLargeReplicatorEnabled9": "True",
  	"FFlagLargeReplicatorRead5": "True",
  	"FFlagLargeReplicatorWrite5": "True",
  	"DFIntStreamingObserverInitialReplicatorCapacity": "4",
  	"DFIntGameNetPVHeaderTranslationZeroCutoffExponent": "-5000",
  	"DFIntGameNetPVHeaderRotationalVelocityZeroCutoffExponent": "-5000",
  	"DFIntGameNetPVHeaderLinearVelocityZeroCutoffExponent": "-5000",
  	"DFIntGameNetPVHeaderRotationOrientIdToleranceExponent": "-2147483647",
  	"DFIntGameNetDontSendRedundantNumTimes": "0",
  	"DFIntGameNetDontSendRedundantDeltaPositionMillionth": "0",
  	"DFIntGameNetDontSendRedundantDeltaThresholdMillionth": "0"
}
```

## blatant anim disable
(see all animations client side, other people wont see your animations)
```json
{
"DFIntReplicatorAnimationTrackLimitPerAnimator": "-1"
}
```

## net ownership
```json
{
  	"DFIntMinClientSimulationRadius": "2147000000",
  	"DFIntMinimalSimRadiusBuffer": "2147000000",
  	"DFIntMaxClientSimulationRadius": "2147000000",
  	"DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "True"
}
```

## 240hz physics
```json
{
	"DFFlagDebugAuroraAllowAdaptiveTimestepping": "True",
	"DFFlagSimAdaptiveAdjustTimestepForControllerManager": "False",
	"DFFlagSim240hzWithConstraintLimitsEnabled2": "True",
	"DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "32",
	"FFlagDebugSimForceAdaptiveTimeStepping": "True",
	"DFIntSimAdaptiveExtraIterations": "16", 
	"DFIntSimDefaultHumanoidTimestepMultiplier": "8",
	"DFIntSimTimestepMultiplierDebounceCount": "147483647",
	"DFIntSimArbiterPositionCorrectionFactorThresholdThou": "147483647",
	"DFIntTimestepArbiterHumanoidTurningVelThreshold": "1",
	"DFIntTimestepArbiterHumanoidLinearVelThreshold": "1",
	"DFIntTimestepArbiterVelocityCriteriaThresholdTwoDt": "1",
	"DFIntTimestepArbiterVelocityCriteriaThresholdFourDt": "1",
	"DFIntTimestepArbiterConditionNumberThresholdThou": "501",
	"DFIntTimestepArbiterBoundingBoxIntersectionThresholdThou2": "0",
	"DFIntTimestepArbiterBoundingBoxIntersectionThresholdThou1": "0",
	"DFIntTimestepArbiterAngAccelerationThresholdThou": "0",
	"DFIntTimestepArbiterAccelerationModelFactorThou": "147483647",
	"DFIntTimestepArbiterThresholdCFLThou": "0",
	"DFIntTimestepArbiterOmegaThou": "0",
	"DFIntTimestepArbiterCharacteristicLengthThou": "1",
	"DFIntSimArbiterCFLLengthScaleThou": "1",
	"DFFlagSimAdaptiveAllow60HzControllerManager":"False",
	"DFFlagSimAdaptiveEnable60HzParts": "False",
	"DFFlagDebugSimAdaptiveEnable60HzHumanoids": "False",
	"DFFlagSimAdaptiveUseNewVelocityCriteria": "True",
	"FFlagSimAdaptiveScaleCollisionParameters2": "True",
	"DFFlagDebugSimAdaptiveIncreaseCollisionStiffness": "True",
	"DFIntDebugSimSolverMinFlopsToSpawnLDLThread": "1",
	"FIntLDLMaxBundleDimension": "24",
	"FIntLDLStasisCachePurgeRate": "1200",
	"FIntLDLStasisCacheMaxAge": "2400"
}
```

## faster interpolation
```json
{
	"DFFlagDebugMechanismInterpolationWorldSpace": "False",
	"DFFlagSimLocalBallSocketInterpolation": "True",     
	"DFIntCheckPVDifferencesForInterpolationMinRotVelThresholdRadsPerSecHundredth": "0",
	"DFIntCheckPVDifferencesForInterpolationMinVelThresholdStudsPerSecHundredth": "0",
	"DFIntGameplayNetInterpolationDistanceCorrectionSampleMillionth": "1000000",
	"DFIntInterpolationFramePositionThresholdMillionth": "1",
	"DFIntInterpolationFrameRotVelocityThresholdMillionth": "1",
	"DFIntInterpolationFrameVelocityThresholdMillionth": "1",
	"DFIntInterpolationMinAssemblyCount": "1",
	"DFIntInterpolationNumMechanismsBatchSize": "4",
	"DFIntInterpolationNumMechanismsPerTask": "4",
	"DFIntInterpolationNumParallelTasks": "350",
	"DFIntMaxInterpolationRecursionsBeforeCheck": "50",
	"DFIntNumFramesToKeepAfterInterpolation": "2",
	"DFIntParallelAdaptiveInterpolationBatchCount": "150",
	"DFIntParallelAdaptiveInterpolationCutoff": "1",
	"FFlagInterpolationAwareTargetTime": "False",
	"FIntInterpolationMaxDelayMSec": "500",
	"DFIntTargetTimeDelayFacctorTenths": "11",
	"DFIntMaxAverageFrameDelayExceedFactor": "0",
	"DFIntMaxFrameBufferSize": "1"
}
```

## better garbage collection
```json
{ 
	"DFIntLuaGcBoost": "3",
	"DFIntLuaGcMaxKb": "4096",
	"FIntLuaGcParallelMinMultiTasks": "4",
	"DFIntLuauGcGoal": "200",
	"DFIntLuauGcGoalCore": "180",
	"DFIntLuauGcStepMul": "100",
	"DFIntLuauGcStepSizeKb": "8",
	"FIntLuauGcGoalCore": "180",
	"FIntLuauGcGoal": "200"
}
```

## better client's predicted correction
```json
{
	"DFIntCheckPVLinearVelocityIntegrateVsDeltaPositionThresholdPercent": "1"
}
```

## favor preformance over quality
```json
{
	"DFIntGraphicsOptimizationModePerformanceBiasPercent": "100",
	"DFIntGraphicsOptimizationModeBalancedBiasPercent": "1",
	"DFIntGraphicsOptimizationModeQualityBiasPercent": "1",
	"FStringIXPGraphicsOptimizationModePerformanceBias": "performanceBias",
	"FStringIXPGraphicsOptimizationModeBalancedBias": "null",
	"FStringIXPGraphicsOptimizationModeQualityBias": "null"
}
```

## aggressive LODs for performance
```json
{
	"DFIntSlimLOD0Distance": "5",
	"DFIntSlimLOD1Distance": "10",
	"DFIntSlimLOD2Distance": "15",
	"DFIntSlimLOD3Distance": "20",
	"DFIntSlimTransitionDistance": "20"
}
```

## better framedata
```json
{
	"DFIntMaxFramesToSend": "2147483647"
}
```
(set to 1 for stability)

## disable acknowledgements growth
```json
{
	"DFIntRakNetMinAckGrowthPercent": "0"
}
```

## reduce CPU load%
```json
{
	"DFFlagLightGridSimdNew3": "True"
}
```

## optimized memory and services
```json
{
	"FFlagSlimService9": "True",
	"FFlagSlimPropertySet3": "True",
	"FFlagSlimContentProvider": "True"
}
```

## new optimized CFrame updates:
```json
{
	"FFlagOptimizeCFrameUpdatesIC4": "False",
	"FFlagOptimizeCFrameUpdates4": "True",
	"FFlagOptimizeCFrameUpdatesIC5": "True"
}
```

## gpu caching
idk (8GB+ VRAM)
```json
{
	"DFIntRenderTextureTotalBudgetMB": "8192",
	"DFIntRenderTextureTotalBudgetCount": "65536",
	"DFIntRenderTextureLoadingBudgetMB": "4096",
	"DFIntRenderTextureLoadingMaxMB": "2048",
	"DFIntRbxStorageAvailableDiskSpaceTriggerMB": "256",
	"DFIntRbxStorageCleanupOldCacheChunkSizeMB": "32",
	"DFIntRbxStorageDBCleanTargetPercentMaxCapacity": "90",
	"DFIntRbxStorageDBMaxCapacityMB": "15360",
	"DFIntRbxStoragePeriodicCleanupIntervalSec": "3600",
	"DFIntRbxStorageSyncIntervalSec": "5",
	"FFlagRbxStorageRemoveLargeDb": "True",
	"FFlagRbxStorageUseMemCache": "True",
	"FIntRbxStorageCleanupDelaySeconds": "1800",
	"FIntRbxStorageDBPreallocateMB": "1024",
	"FIntRbxStorageDeleteOldCacheMB": "2048",
	"FIntRbxStorageRemoveLargeDbThresholdMB": "10240"
}
```

## better packets
```json
{
	"DFIntNetworkStopProducingPacketsToProcessThresholdMs": 0,
	"DFIntMaxWaitTimeBeforeForcePacketProcessMS": 1,
	"DFIntClientPacketMaxDelayMs": 1,
	"DFIntClientPacketMinMicroseconds": 100000000,
	"DFIntClientPacketExcessMicroseconds": 10000000,
	"DFIntClientPacketMaxFrameMicroseconds": 1047483647,
	"DFIntClientPacketHealthyAllocationPercent": 75,
	"DFIntClientPacketHealthyMsPerSecondLimit": 1,
	"DFIntClientPacketUnhealthyContEscMsPerSecond": 10000,
	"DFIntMaxProcessPacketsJobScaling": 5000000,
	"DFIntMaxProcessPacketsStepsAccumulated": 0,
	"DFIntMaxProcessPacketsStepsPerCyclic": 1047483647
}
```

## lowered input delay
```json
{
	"FIntCLI20390_2": "0",
	"FFlagRobloxInputUsesRuntime2": "True",
	"FFlagFasterPreciseTime5": "True",
	"FFlagLuaAppLegacyInputSettingRefactor": "True",
	"FIntActivatedCountTimerMSMouse": "1",
	"FIntActivatedCountTimerMSKeyboard": "1",
	"FIntDefaultJitterN": "0",
	"FIntMaquettesFrameRateBufferPercentage": "0",
	"DFIntMaxFrameBufferSize": "1",
	"FIntInterpolationAwareTargetTimeLerpHundredth": "100",
	"DFIntMaxAverageFrameDelayExceedFactor": "0",
	"DFIntTargetTimeDelayFacctorTenths": "9",
	"FStringRemoteAnimationSmoothingStrategy": "Extrapolation",
	"FFlagLuaMenuPerfImprovements": "True",
	"DFIntNetworkQualityResponderMaxWaitTime": "1",
	"FIntSmoothMouseSpringFrequencyTenths": "100",
	"DFIntMaxAcceptableUpdateDelay": "1",
	"FFlagSmoothInputOffset": "True",
	"FFlagStylingFasterTagProcessing": "True",
	"FFlagUserBetterInertialScrolling": "True",
	"FFlagUserCameraControlLastInputTypeUpdate": "False",
	"DFFlagProbesStaggerUpdateCalls": "True"
}
```

## fixed hitbox
not sure
```json
{
	"FIntTaskSchedulerTargetFps": 240,
	"DFIntSmoothNetPhysicsSendRate": 60,
	"DFIntSmoothNetPhysicsMaxSendRate": 60,
	"DFIntInterpolationTimeMs": 2,
	"DFIntReplicationResendRate": 60,
	"FFlagUserRemoveCameraDrift": true,
	"FFlagFixInputDelay": true,
	"FFlagUserFastGameLoad": true,
	"FFlagFixPredictedProjectilePosition": true,
	"FFlagUserMovementPredictionFix": true,
	"DFIntRenderingPauseDelay": 0,
	"DFIntPhysicsSleepTime": 5
}
```

## illegals with values
```json
	"DFIntMaximumUnstickForceInGs": "1",
	"DFIntMaximumFreefallMoveTimeInTenths": "-1",
	"DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "50000",
	"DFIntDebugSimPhysicsSteppingMethodOverride": "0",
	"DFIntSmoothTerrainPhysicsRayAabbSlop": "1",
	"DFIntMaxMissedWorldStepsRemembered": "1147483647",
	"DFIntSolidFloorPercentForceApplication": "0",
	"DFIntNonSolidFloorPercentForceApplication": "0",
```

## consistent MTU Sizes
```json
{
	"DFIntConnectionMTUSize": "1412",
	"DFIntCrossPlatformMinMTUSize": "1412",
	"DFIntRakNetMtuValue1InBytes": "1412",
	"DFIntRakNetMtuValue2InBytes": "1412",
	"DFIntRakNetMtuValue3InBytes": "1412",
	"DFIntRakNetPacketTracingMinMTUSize": "1412"
}
```

optional bypass (1518, stable) OUTDATED, CREATED PRE-WHITELIST
```json
{
	"DFIntConnectionMTUSize": "1472",
	"DFIntCrossPlatformMinMTUSize": "1472",
	"DFIntRakNetMtuValue1InBytes": "1492",
	"DFIntRakNetMtuValue2InBytes": "1518",
	"DFIntRakNetMtuValue3InBytes": "1518",
	"DFIntRakNetPacketTracingMinMTUSize": "1472"
}
```

## disable telemetry (performance)
```json
{
	"FIntOpenTelemetryScheduleDelayMillis": "2147483647",
	"FIntLogTelemetrySinkIntervalSeconds": "2147483647", 
	"FFlagEnableTelemetryServicePlaySessionInfo": "False",
	"DFIntRbxStorageTelemetryIntervalMS": "2147483647",
	"DFIntPercentileTelemetryHundredPercent": "0",
	"DFFlagAddMachineIDInstallerTelemetry": "False",
	"DFStringHttpPointsReporterUrl": "0.0.0.0",
	"FFlagOpenTelemetryEnabled2": "False",
	"FFlagEnableTelemetryProtocol": "False",
	"FFlagEnableTelemetryService1": "False",
	"DFStringTelemetryV2Url": "0.0.0.0",
	"FLogRobloxTelemetry": "Error,0",
	"DFIntMaxLogHistory": "0"
	"DFFlagAddPlaySessionIdTelemetry": "False",
	"DFIntTelemetryRateLimiterBurstSizeHundredths": "0",
	"DFIntTelemetryRateLimiterRegenRateHundredths": "0",
	"DFStringAltHttpPointsReporterUrl": "0.0.0.0",
	"FFlagEnableTelemetryServiceMemoryCPUInfo": "False",
	"FFlagDisableMemoryTracking": "False",
	"DFStringRobloxTelemetryReliabilityCountAllowList": "null",
	"DFStringRobloxTelemetryCheckSumSalt": "",
	"FFlagRobloxTelemetryAddDeviceRAM": "False",
	"DFIntPerformanceTelemetryGlobalThrottleHundredthsPercent": "0",
	"FFlagRobloxTelemetryAddOsVersionAsTag": "False",
	"FFlagRobloxTelemetryAddOTAVersionAsTag": "False",
	"FStringOpenTelemetryOtlpEndpoint": ""
}
```

## instance pooling
```json
{
	"FStringInstancesToPoolByName": "Part:4096;MeshPart:4096;WeldConstraint:4096;Motor6D:2048;Attachment:2048;Frame:2048;ImageLabel:2048;TextLabel:2048;Folder:2048;Sound:2048;Humanoid:1024;ParticleEmitter:1024;Trail:1024;Beam:1024;RemoteEvent:1024;Script:1024;LocalScript:1024;ModuleScript:1024;WedgePart:1024;CornerWedgePart:1024;TrussPart:1024;Weld:1024;Decal:1024;Texture:1024;SpecialMesh:1024;UIStroke:1024;BillboardGui:1024;ImageButton:1024;TextButton:1024;ScrollingFrame:1024;UIGridLayout:1024;UIListLayout:1024;Highlight:1024;Tool:512;Explosion:512;Fire:512;Smoke:512;Sparkles:512;Light:512;SpotLight:512;PointLight:512;SurfaceLight:512;HingeConstraint:512;BallSocketConstraint:512;SpringConstraint:512;AlignPosition:512;AlignOrientation:512;BodyForce:512;BodyGyro:512;BodyVelocity:512;ProximityPrompt:512;SelectionBox:512;Configuration:512;RemoteFunction:512;Tween:512;Pose:512;KeyframeSequence:512;BoolValue:512;IntValue:512;NumberValue:512;StringValue:512;ObjectValue:512;CFrameValue:512;Vector3Value:512;RayValue:512;BlockMesh:512;CylinderMesh:512;FileMesh:512;ScreenGui:256;SurfaceGui:256;UIScale:256"
}
```

## light culling
```json
{
	"FFlagDebugForceFSMCPULightCulling": "True",
	"FFlagFastGPULightCulling3": "True"
}
```

## obviously good performance flags
```json
{
	"FFlagDebugPerfMode": "True",
	"FFlagHandleAltEnterFullscreenManually": "False",
	"FIntDefaultJitterN": "0",
	"FFlagDebugSSAOForce": "True",
	"FIntRenderNodeEnterSleepingFrames": "0"
}
```

## performance render distancing ig
it gives a lot of performance boost, hard to explain
```json
{
	"FIntCameraFarZPlane": "2741"
}
```

## performance textures
```json
{
	"FIntTerrainArraySliceSize": "4",
	"FIntTerrainOTAMaxTextureSize": "1024",
	"FFlagDisablePostFx": "True",
	"FFlagRenderFixFog": "True",
	"FFlagRenderNoLowFrmBloom": "False",
	"FIntBloomFrmCutoff": "25",
	"FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[207,208,206,254]}}",
	"FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255,255,255,255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[204,201,200,232]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[212,200,187,250]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[208,208,208,255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[170,170,170,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[105,104,102,244]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547304948\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[113,113,113,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[165,165,159,255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255,255,255,255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[199,199,199,255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[199,199,199,255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[208,208,208,255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[159,119,95,200]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[220,220,220,255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[193,193,193,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[227,227,227,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[212,209,203,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[123,123,123,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[154,154,153,238]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[74,78,80,156]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[226,229,229,243]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[114,114,112,240]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[121,117,113,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[235,234,230,250]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[130,130,130,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[142,142,144,236]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[154,154,154,248]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[220,220,221,255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[174,171,169,246]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[218,218,218,255]}}",
	"FStringTerrainMaterialTable2022": "",
	"FStringTerrainMaterialTablePre2022": ""
}
```
