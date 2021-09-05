C_Player: C_BaseCombatCharacter - Base player client-side

| Squirrel Name | Type Info | Comment |
| ------------- | --------- | ------- |
| AmmoPool_GetCapacity | () -> int | Get the capacity of the ammo pool |
| AmmoPool_GetCount | eAmmoPoolType ammoType -> int | Get the ammo count in the ammo pool |
| CameraAngles | () -> vector | Get current camera angles |
| CameraPosition | () -> vector | Get current camera position |
| CanStand | () -> bool | Returns true if the player is already standing or has space to stand |
| CanUseJetpack | vector -> bool |  |
| ClearLookStickDebounce | () -> void |  |
| ClearMeleeDisabled | () -> void | Decrements disabled melee counter |
| ClearMenuCameraEntity | () -> void | Clears overrides of the view entity on the client only |
| ClientCommand | string command -> void | Execute command on this client |
| CockpitJolt | vector, float -> void |  |
| ConsumableInventory_Get | () -> array< ConsumableInventoryItem > | Get the consumable inventory |
| ConsumableInventory_GetCount | () -> int | Get the number of filled slots in the consumable inventory |
| CreateClientPointCamera |  | Creates a client point camera |
| DelayEnableWeaponWithSlowDeploy | float delay -> void | Enable the player's weapon with delay |
| DeployWeapon | () -> void | Pull out the player's weapon using slow deploy animation |
| DisableSlowMo | () -> void |  |
| DisableWeapon | () -> void | Disable the player's weapon |
| DisableWeaponViewModel | () -> void | Disable the player's weapon viewmodel |
| DisableWeaponWithSlowHolster | () -> void |  |
| DoesUserHaveTwitchPrimeReward | string rewardName -> bool | Returns true if this player has a Twitch Prime reward |
| EnableSlowMo | () -> void |  |
| EnableWeapon | () -> void | Enable the player's weapon |
| EnableWeaponViewModel | () -> void | Enable the player's weapon viewmodel |
| EnableWeaponWithSlowDeploy | () -> void |  |
| FreezeControlsOnClient | () -> void | Freeze player's controls |
| GetAbilityDownBinding |  | Gets the TAPPED or HELD binding for the given +ability command |
| GetAbilityUpBinding |  | Gets the TAPPED or HELD binding for the given +ability command |
| GetAdsFraction | () -> float | Get the current ADS fraction amount \[0-1\] |
| GetBleedoutState | () -> BleedoutState |  |
| GetCinematicEventFlags | () -> CinematicEventFlags |  |
| GetClassPosCount | () -> int |  |
| GetCockpit | () -> entity | Gets the player cockpit entity |
| GetCommunityName | () -> string | Gets the name of the community this player is currently playing in |
| GetCrosshairPos |  | Gets crosshair position as a fraction of screen size \[0-1\]) |
| GetCrosshairTraceEndPos | () -> vector | Gets the end position for the crosshair trace that we do all the time |
| GetDodgePower | () -> float | Gets the raw dodge power of the suit |
| GetFOV | () -> float | Get FOV of the player |
| GetFaction | () -> string | Gets the name of the faction this player is currently playing for |
| GetFirstPersonProxy | () -> entity | Create and get the player's first person proxy |
| GetForcedDialogueOnly | () -> bool |  |
| GetGen | () -> int | Gets the player's generation |
| GetGlideMeter | () -> float | Returns current glide meter value |
| GetGrappleAutoAimTarget | () -> entity |  |
| GetGrappleHook | () -> entity | Gets the grapple hook entity for this player |
| GetGrappleWeapon | () -> entity |  |
| GetHardpointEntity | () -> entity | Returns the players current hardpoint |
| GetHardware | () -> string | Gets the name of the player's current hardware |
| GetHotDropImpactTime |  | Returns time of the hot drop impact |
| GetInputAxisForward | () -> float | Gets the amount the left stick or WASD keys are pressed forward between -1 to 1. |
| GetInputAxisRight | () -> float | Gets the amount the left stick or WASD keys are pressed right between -1 to 1. |
| GetLastCycleSlot | () -> int | Returns the last main weapon slot that the player had cycled to |
| GetLastTimeDamagedByNPC | () -> float |  |
| GetLastTimeDamagedByOtherPlayer | () -> float |  |
| GetLastTimeDidDamageToNPC | () -> float |  |
| GetLastTimeDidDamageToOtherPlayer | () -> float |  |
| GetLevel | () -> int | Gets the player's Level |
| GetLocalGravityDirection | () -> vector |  |
| GetLocalGravityStrength | () -> float |  |
| GetMeleeDisabled | () -> int | Gets the disabled melee counter |
| GetMinimapCurrentZoomScale |  | Zoom scale lerps over time, this returns the current value of the minimap zoom scale |
| GetMinimapTargetZoomScale |  | Zoom scale lerps over time, this returns the final target after the lerp |
| GetNextTitanRespawnAvailable | () -> float |  |
| GetObjectiveEndTime | () -> float | Get time when the object will expire |
| GetObjectiveEntity | () -> entity | Get entity that client script can use for objective |
| GetObjectiveIndex | () -> int | Get index that client script can use for objective info |
| GetObserverMode | () -> ObserverMode | Returns the player's observer mode |
| GetObserverTarget | () -> entity | Returns the player's observer target |
| GetOutOfBoundsDeadTime | () -> float | Returns time that the player will die if he stays out of bounds |
| GetPINNucleusId |  |  |
| GetPINNucleusPid |  |  |
| GetPINPlatformId |  |  |
| GetPersistentVar | string varName -> result | May return any type |
| GetPersistentVarAsInt | string varName -> int |  |
| GetPetTitan | () -> entity | Returns the player's pet titan |
| GetPetTitanMode | () -> eNPCTitanMode | Returns the player's pet titan mode |
| GetPilotClassIndex | () -> int | Get the players pilot class index |
| GetPlatformUID | () -> string | Gets the player's UID |
| GetPlayerClass | () -> string | What general class is the player (pilot/titan) |
| GetPlayerClassName |  | What class is the player |
| GetPlayerGameStat | PlayerGameStat stat -> int |  |
| GetPlayerGeneralClassName |  |  |
| GetPlayerMaxs | () -> vector | Returns player's maximum bounds |
| GetPlayerMins | () -> vector | Returns player's minimum bounds |
| GetPlayerModHealth | () -> float |  |
| GetPlayerModHealthPerSegment | () -> float |  |
| GetPlayerName | () -> string | Get the player's name |
| GetPlayerNameWithClanTag | () -> string | Get the player's name with their clan tag in front |
| GetPlayerNetBool | string networkVariableName -> bool | Gets a bool network variable on the player (see RegisterNetworkedVariable) |
| GetPlayerNetEnt | string networkVariableName -> _possibly_ entity | Gets an entity network variable on the player (see RegisterNetworkedVariable) |
| GetPlayerNetFloat | string networkVariableName -> float | Gets a float network variable on the player (see RegisterNetworkedVariable) |
| GetPlayerNetInt | string networkVariableName -> int | Gets an int network variable on the player (see RegisterNetworkedVariable) |
| GetPlayerNetTime | string networkVariableName -> float | Gets a time (float) network variable on the player (see RegisterNetworkedVariable) |
| GetPlayerPINPlatformName |  |  |
| GetPlayerPINTitleId |  |  |
| GetPlayerRagdoll |  | Gets the ragdoll of the player on the client |
| GetPlayerRequestedClass |  | What class has the player requested. `Call crashes the game` |
| GetPlayerRequestedSettings | () -> asset | What class has the player requested |
| GetPlayerSettingAsset | string settingName -> asset | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingBool | string settingName -> bool | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingFloat | string settingName -> float | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingInt | string settingName -> int | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingString | string settingName -> string | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingStringAsAsset | string settingName -> asset | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettingVector | string settingName -> vector | Gets the value of the given player settings field for the players current settings |
| GetPlayerSettings | () -> asset |  |
| GetPlayerSettingsBlock | () -> userdata | Gets the player's player settings as a settings block for calls into GetSettingsBlockInt/Float/etc |
| GetPlayerSettingsMods | () -> array< string > | Get an array of mods active on this player |
| GetPlayerSubClass | () -> string | What class is the player (wallrun/boost) |
| GetPredictedFirstPersonProxy | () -> entity | Create and get the player's predicted first person proxy |
| GetRank | () -> int | Gets the player's rank |
| GetSkillMU |  |  |
| GetSuitGrapplePower | () -> float | Gets the percentage of "grapple power" remaining |
| GetSuitJumpPower | () -> float | Gets the percentage of "suit jump power" remaining (used for double jump) |
| GetSuitPower | () -> float | Gets the percentage of "suit power" remaining (used for sprint, etc) |
| GetSyncedEntity | () -> entity | Gets the entity that should be time-aligned with the player |
| GetTargetInCrosshairRange | () -> entity | Returns an enemy target if the player is aiming at it and it is in maximum damage range |
| GetThirdPersonAttackFocus | () -> vector |  |
| GetTitanBubbleShieldTime | () -> float |  |
| GetTitanBuildTime | () -> float |  |
| GetTitanDisembarkEnabled | () -> bool |  |
| GetTitanEmbarkEnabled | () -> bool |  |
| GetTitanTarget |  | Get a titan available for smart targetting type uses |
| GetTrackEntityDistanceMode | () -> string |  |
| GetTrackEntityOffsetDistance | () -> float |  |
| GetTrackEntityOffsetHeight | () -> float |  |
| GetUseEntity | () -> entity | Gets the use entity that would be found if the player tried to use something this frame |
| GetUsePromptEntity | () -> entity | Returns current entity for which the use prompt is displayed, if any |
| GetUsePromptPosition | () -> vector | Returns the use position for the current use entity |
| GetViewForward | () -> vector | Get the forward view vector of the player |
| GetViewModelArmsAttachment | () -> entity | Returns the view model arms attachment entity |
| GetViewModelEntity | () -> entity | Returns the view model entity |
| GetViewRight | () -> vector | Get the right view vector of the player |
| GetViewUp | () -> vector | Get the up view vector of the player |
| GetViewVector | () -> vector | Get the forward view vector of the player |
| GetVoicePackIndex | () -> int | Get index that client script can use for voice pack info |
| GetXP | () -> int | Gets the player's XP |
| GetZoomFrac | () -> float | Get the current zoom fraction amount \[0-1\] |
| Grapple | vector direction -> void | Toggles grapple |
| GrappleDetach | () -> void |  |
| HasBadReputation | () -> bool | Returns true if this player has a bad reputation |
| HasClassMod | string mod -> bool | Given (string), returns true if mod is active on this player |
| HasGrapple | () -> bool | Returns whether this player has grapple available in general |
| HasMic | () -> bool | Returns true if the player has a mic plugged in |
| HasPassive | ePassives passive -> bool |  |
| HasThirdPersonAttackFocus | () -> bool |  |
| HasUsePrompt | () -> bool | Returns whether the player has a use prompt |
| HideCrosshairNames | () -> void | Suppress drawing of player/AI names on the HUD |
| HolsterWeapon | () -> void | Holster player's weapon with slower holster animation |
| InPartyChat | () -> bool | Returns true if the player is in party chat |
| IsBoosting | () -> bool | Returns true if the player is currently boosting |
| IsBot | () -> bool | Returns true if this player is a bot |
| IsClassModAvailableForPlayerSetting | string settings, string mod -> bool | Given (string), returns true if given mod is available to use for this player |
| IsCrouched | () -> bool | Returns if the player is crouched |
| IsDodging | () -> bool | Returns whether the player is dodging |
| IsDoubleJumping | () -> bool | Returns whether the player is in the middle of a double-jump |
| IsGliding | () -> bool | Returns true if the player is currently gliding |
| IsGrappleActive | () -> bool | Checks if grapple hook is deployed (not necessarily attached) |
| IsGrappleAttached | () -> bool | Checks if grapple hook is attached (not necessarily pulling yet) |
| IsGrapplePulling | () -> bool | Checks if grapple hook is pulling the player |
| IsGrapplingZipline | () -> bool |  |
| IsHoverEnabled | () -> bool | Returns true if the player can hover |
| IsHovering | () -> bool | Returns true if the player is currently hovering |
| IsInAirSlowMo | () -> bool | Returns true if the player is in air slowmo |
| IsInThirdPersonReplay | () -> bool | Returns if this player is in a third person replay (usually when killed by AI) |
| IsInputCommandHeld | InputCommand command -> bool | Indicates if the specified input command is being pressed. Only works for the local view player |
| IsInputCommandPressed | InputCommand command -> bool | Indicates if the specified input command was pressed this frame. Only works for the local view player |
| IsInputCommandReleased | InputCommand command -> bool | Indicates if the specified input command was released this frame. Only works for the local view player |
| IsInventoryOpen | () -> bool | Returns true if code thinks the player's inventory screen is open |
| IsMantling | () -> bool | Returns whether the player is mantling |
| IsMountingZipline | () -> bool | Returns true if the player is mounting a zipline |
| IsObserver | () -> bool | Returns whether the player is in an observer mode |
| IsPartyLeader | () -> bool | Returns true if this player is our party leader |
| IsPlayback | () -> bool | Returns true if this player is a bot created to play back a recording from bot_record |
| IsPlayingRanked | () -> bool | Find out if the player is playing in ranked mode |
| IsScriptMenuOn | () -> bool | Returns whether the script menu is on |
| IsShadowForm | () -> bool | Is this player in shadow form? |
| IsSliding | () -> bool | Returns whether the player is sliding |
| IsSprinting | () -> bool | Returns whether the player is sprinting |
| IsStanding | () -> bool | Returns if the player is standing |
| IsTalking | () -> bool | Returns true if the player is currently speaking over voice chat (and we can hear them) |
| IsTextMuted | () -> bool | Returns true if the player is muted |
| IsThirdPersonObserver | () -> bool |  |
| IsThirdPersonShoulderModeOn | () -> bool | Returns whether the player is in third person mode |
| IsTraversing | () -> bool | Returns whether the player is traversing (i.e. mantle or window anims) |
| IsUserCommandButtonHeld | InputCommand command -> bool | Looks at the latest raw usercommand input for the given local player |
| IsVoiceMuted | () -> bool | Returns true if the player is muted |
| IsWallHanging | () -> bool | Returns whether the player is wall-hanging |
| IsWallRunning | () -> bool | Returns whether the player is wallrunning |
| IsZiplining | () -> bool | Returns true if the player is ziplining (in either direction) |
| IsZipliningInReverse | () -> bool | Returns true if the player is ziplining in reverse |
| JoltCockpitAngles | float offsetPitch, float offsetYaw, float offsetRoll, float velocityPitch, float velocityYaw, float velocityRoll -> void |  |
| JoltCockpitOrigin | vector offset, vector velocity -> void |  |
| KnockBack | vector velocity, float duration -> void |  |
| LowHealthEffectsEnabled | () -> bool | Checks to see if the low health effects should be on |
| Lunge_ClearTarget | () -> void | Clears any lunging currently going on |
| Lunge_EnableFlying | () -> void | Allow the lunge to fly into the air, if it needs to |
| Lunge_GetEndPositionOffset | () -> vector |  |
| Lunge_GetSmoothTime | () -> float | Returns how long the lunge will last for |
| Lunge_GetStartPositionOffset |  | Returns the initial relative position of the player from the lunge target |
| Lunge_GetTargetEntity | () -> entity | Get the current lunge target |
| Lunge_GetTargetPosition | () -> vector | Get the position the player is lunging towards |
| Lunge_IsActive | () -> bool | Is the player lunging |
| Lunge_IsGroundExecute | () -> bool | Is the player lunging to ground execute |
| Lunge_IsLungingToEntity | () -> bool | Is the player lunging towards an entity |
| Lunge_IsLungingToPosition | () -> bool | Is the player lunging towards a position |
| Lunge_LockPitch | bool lock -> void | Whether lunging to adjust the player's view pitch |
| Lunge_SetEndPositionOffset | vector offset -> void |  |
| Lunge_SetMaxEndSpeed | float speed -> void | Sets the maximum speed the player can end lunging with |
| Lunge_SetMaxTime | float time -> void | Sets maximum time for how long a lunge will go on for |
| Lunge_SetSmoothTime | float time -> void | Sets how long it takes to lunge to the target |
| Lunge_SetTargetEntity | entity target -> void | Make the player lerp towards the given target |
| Lunge_SetTargetPosition | vector position -> void | Make the player lerp towards the given position |
| MayGrapple | () -> bool | Returns whether this player can grapple the surface they're looking at |
| ModInventory_Get | () -> array< ModInventoryItem > | Get the mod inventory |
| ModInventory_GetCount | () -> int | Get the number of filled slots in the mod inventory |
| PlayerMelee_EndAttack | () -> void | Let code know a melee attack has ended |
| PlayerMelee_GetAttackHitEntity | () -> _possibly_ bool or entity | Let script query whether the melee attack hit flag has been set |
| PlayerMelee_GetState | () -> PlayerMeleeState | Gets scripted melee state (arbitrary integer) |
| PlayerMelee_IsAttackActive | () -> bool | Let script query whether a melee attack is currently started |
| PlayerMelee_IsSprintAttack | () -> bool | Returns true if currently doing a melee attack and the attack was started while sprinting |
| PlayerMelee_SetAttackHitEntity | entity target -> void | Let code know the melee attack hit something (so code will stop the lunge movement) |
| PlayerMelee_SetAttackRecoveryShouldBeQuick | bool quick -> void |  |
| PlayerMelee_SetState | PlayerMeleeState state -> void | Sets scripted melee state (arbitrary integer) |
| PlayerMelee_StartAttack | PlayerMeleeState state -> void | Let code know a melee attack has started |
| Player_GetFreefallAnticipateEndTime | () -> float | Return time freefall anticipation ended |
| Player_GetFreefallAnticipateStartTime | () -> float | Return time freefall anticipation started |
| Player_GetFreefallDistanceToLand | () -> float |  |
| Player_GetFreefallEndTime | () -> float | Return time freefall ended |
| Player_GetFreefallStartTime | () -> float | Return time freefall started |
| Player_IsFreefallAnticipating | () -> bool | Returns true if the player is freefalling and about to land |
| Player_IsFreefalling | () -> bool | Returns true if the player is freefalling |
| RumbleEffect |  | Plays a controller rumble on the current player. Takes three parameters: rumble index (the wave pattern of the vibration or 0 to stop all rumbles), rumble data (optional data for the rumble flags parameter that follows), and rumble flags (additional flags for the rumble). See [rumble_shared.h](https://swarm.workshop.perforce.com/files/guest/knut_wikstrom/ValveSDKCode/game_shared/rumble_shared.h) for further details |
| SetActivateBoost | bool activate -> void | Sets if boost should be activated |
| SetActivateJetpack | bool activate -> void | Set if jetpack should be activated |
| SetBoostMeter | float -> void |  |
| SetFOVScale | float , float -> void |  |
| SetGrappleAutoAimTarget | entity target -> void | Make grapple seek out this target when it is fired |
| SetHandsEffectControlPoint |  | Sets a value of a control point on the player hands effect |
| SetHoldToSwapSlot |  |  |
| SetLCDPlayerClassSettingsEnabled | bool isEnabled -> void |  |
| SetLookStickDebounce | () -> void |  |
| SetMeleeDisabled | () -> void | Increments disabled melee counter |
| SetMenuCameraEntity | entity camera -> void | Overrides the view entity on the client only |
| SetMenuCameraEntityWithAudio | entity camera -> void | Overrides the view entity on the client only, also brings audio listener position along |
| SetMenuCameraNearZ | float nearZval -> void | Overrides the near z value when using the menu camera |
| SetOneHandedWeaponUsageOff | () -> void | Disable one-handed weapon anims |
| SetOneHandedWeaponUsageOn | () -> void | Enable one-handed weapon anims |
| SetSafeHealthFrac | float frac -> void | Set the safe health fraction used by some titan material proxies |
| SetScriptMenuOff | () -> void | Hint to the client system that script has turned off its menu |
| SetScriptMenuOn | () -> void | Hint to the client system that script has a menu up |
| SetTitanDisembarkEnabled | bool enabled -> void |  |
| SetTitanEmbarkEnabled | bool enabled -> void |  |
| SetTrackEntityOffsetDistance | float -> void |  |
| SetTrackEntityOffsetHeight | float -> void |  |
| Skydive_FollowPlayer | entity target -> void | _possibly_ Sets player to follow while skydiving |
| Skydive_GetDiveAngle | () -> float |  |
| Skydive_GetFreelookLockedAngle | () -> vector |  |
| Skydive_GetSpeed | () -> float |  |
| Skydive_GetStrafeAngle | () -> float |  |
| Skydive_IsFollowing | () -> bool |  |
| Skydive_IsFreelooking | () -> bool |  |
| Skydive_QueueStopFollowing | () -> void |  |
| Skydive_SetFreelookMode | bool enabled -> void |  |
| Skydive_StopFollowing | () -> void | Stops following while skydiving |
| SmartAmmo_GetHighestLockOnMeFraction | () -> float | Returns the highest fraction value a smart-ammo-enabled weapon has locked onto this entity right now |
| SmartAmmo_GetHighestLocksOnMeEntities | () -> array< entity > | Returns an array of the weapon entities with the highest fraction/locks on us |
| SmartAmmo_GetPreviousHighestLockOnMeFraction | () -> float | Returns the previous highest fraction value |
| SniperCam_Activate | () -> void | Activate the sniper cam to target this entity |
| SniperCam_Deactivate | () -> void | Fade out and deactivate the sniper cam |
| SniperCam_GetParams |  | Get sniper cam parameters |
| SniperCam_IsActive |  | Does sniper cam exist and is it active |
| SniperCam_SetParams |  | Set sniper cam parameters |
| StartArcCannon | () -> void | Tell code that we are starting the arc cannon effect on this player |
| StartEffectOnPlayerHands | asset, string -> void |  |
| StopArcCannon | () -> void | Tell code to stop the arc cannon effect on this player |
| StopEffectOnPlayerHands | () -> void |  |
| TransformAttackSpreadToScreenSpace |  | Transforms a weapon attack spread angle to screen pixels |
| UnfreezeControlsOnClient | () -> void | Unfreeze player's controls |
| UnhideCrosshairNames | () -> void | Continue drawing of player/AI names on the HUD |
| UseableEyePosition | entity target -> vector | Pass in ent you want to get player eye position for |
| ViewOffsetEntity_SetEntity | entity target -> void | Set view offset entity for first-person animation |
| ViewOffsetEntity_SetLerpInTime | float time -> void | Sets the lerp-in duration for the anim view entity (and view offset entity). Setting the entity resets the time to zero, so call this after setting the view entity |
| ViewOffsetEntity_SetLerpOutTime | float time -> void | Sets the lerp-out duration for the anim view entity (and view offset entity). Setting the entity resets the time to zero, so call this after setting the view entity |
| Zipline_GetActiveZipline | () -> entity | Get the zipline entity the player is currently using |
| Zipline_GetLastZipline | () -> entity | Get the zipline entity the player was last using |
| Zipline_IsZipliningVertically | () -> bool | Returns true if the player is ziplining vertically |
|  |  |  |