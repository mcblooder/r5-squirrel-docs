| Squirrel Name | Type Info | Comment |
| ------------- | --------- | ------- |
| AddMod | string mod -> void | Given (string), add the mod from this weapon |
| AllowUse | bool -> void | Sets whether a weapon can be used or not |
| CheckWeaponIsDisabled | entity player -> bool | Takes in a player and checks to see if the weapon is disabled |
| ClearForcedADS | () -> void | Lets the player choose whether or not to ads |
| ClearWeaponCharm | () -> void | Clear the wepaon charm entity for the current weapon |
| CustomActivityAttachModel |  | Specifies a model to be attached to the viewmodel during the current custom activity, as well as an attachment index |
| CustomActivityClearAttachedModel |  | Clears the attached custom activity model |
| Deploy | () -> void | Triggers weapon deploy |
| DeployInstant | () -> void | Triggers weapon deploy |
| DoMeleeHitConfirmation | float _possibly_ severityScale -> void |  |
| EmitWeaponNpcSound | float radius, float -> void | Notifies NPCs of weapon sound |
| EmitWeaponNpcSound_DontUpdateLastFiredTime | float radius, float -> void | Notifies NPCs of weapon sound |
| EmitWeaponSound | string -> void | Plays the sound on the weapon |
| EmitWeaponSound_1p3p | string soundName1p, string soundName3p -> void | Plays appropriate 1p and 3p sounds |
| FireWeaponBolt | WeaponFireBoltParams params -> void | Fires a bolt projectile |
| FireWeaponBoltAndReturnEntity | WeaponFireBoltParams params -> entity | Fires a bolt projectile and returns the entity (bolt) to script |
| FireWeaponBullet | vector position, vector direction, int, int weaponDamageFlags -> void | Fires a bullet |
| FireWeaponBullet_Special | WeaponFireBulletSpecialParams params -> void | Fires a bullet, can set to skip lag compensation, have zero spread, dryfire, or only cause a whizby sound |
| FireWeaponGrenade | WeaponFireGrenadeParams params -> entity | Fires a grenade projectile and returns the entity (grenade) to script |
| FireWeaponMissile | WeaponFireMissileParams params -> entity | Fires a missile projectile and returns the entity (missile) to script |
| FireWeapon_Default | vector pos, vector dir, float speed, float patternScale, bool ignoreSpread -> void | Fires the weapon once as per weaponsettings, in a scaled blast pattern (if one is specified) |
| ForceCooldownMilestone | int newMilestone -> void |  |
| ForceRechamberMilestone | int newMilestone -> void |  |
| ForceRelease | () -> void | Forces the offhand weapon to release |
| GetActiveAmmoSource | () -> AmmoSource | Get the ammo source this weapon is using |
| GetAllowHeadShots | () -> bool | Does this weapon allow for headshot damage |
| GetAmmoDisplay |  | Gets the display type of the ammo |
| GetAmmoPerShot | () -> int | Gets the ammo consumed per shot |
| GetAttackDirection | () -> vector | Returns the direction to fire from |
| GetAttackPosition | () -> vector | Returns the position to fire from |
| GetAttackSpreadAngle | () -> float | Returns the weapon's attack spread in degrees from one side of the cone to the other |
| GetBeginStationAnglesForZiplineGrenade | entity -> vector | Returns the exact angle the begin station should be placed at for the zipline grenade/gun |
| GetBeginStationOriginForZiplineGrenade | entity -> vector | Returns the exact origin the begin station should be placed at for the zipline grenade/gun |
| GetBurstFireShotsPending | () -> int |  |
| GetChargeAnimIndex | () -> int |  |
| GetChargeDuration | () -> float | Gets the total charge duration of the weapon |
| GetCharmModelName | () -> string | Get weapon charm model name for the weapon |
| GetCooldownMilestone | () -> int |  |
| GetCoreDuration | () -> float | Gets the core duration |
| GetCurrentAltFireIndex | () -> int | Gets the index for the next shot to be fired |
| GetCurrentWeaponCharm | () -> entity | Get weapon charm for the weapon |
| GetCustomActivityDuration | () -> float | Returns the duration of the current custom weapon activity |
| GetCustomActivityFraction | () -> float | Returns the fraction of the current custom weapon activity that is complete |
| GetDamageAmountForArmorType | ArmorType armorType -> int |  |
| GetDamageSourceID | () -> eDamageSourceId | Gets the damage source ID for this weapon |
| GetForcedADS | () -> bool | Gets whether or not the player is forced into ads |
| GetGrenadeFuseTime | () -> float |  |
| GetGrenadeIgnitionTime | () -> float |  |
| GetImpactTableIndex | string -> int |  |
| GetInventoryIndex | () -> int |  |
| GetLifetimeShotsRemaining | () -> int |  |
| GetMaxDamageFarDist | () -> float | Gets the largest damage far dist for current owner |
| GetMeleeAnim3p |  |  |
| GetMeleeAttackAngle | () -> float |  |
| GetMeleeAttackRange | () -> float |  |
| GetMeleeCanHitHumanSized | () -> bool |  |
| GetMeleeCanHitTitans | () -> bool |  |
| GetMeleeLungeTargetAngle | () -> float |  |
| GetMeleeLungeTargetRange | () -> float |  |
| GetModBitField | () -> int | Gets mods bit field |
| GetMods | () -> array< string > | Get an array of mods active on this weapon |
| GetMods_WithQueued | () -> array< string > | Get an array of mods active or queued on this weapon |
| GetNPCMissFastPlayer | () -> bool |  |
| GetNextAttackAllowedTime | () -> float | Get this weapon's internal when-can-I-shoot-next time |
| GetNextAttackAllowedTimeRaw | () -> float | Get this weapon's internal when-can-I-shoot-next time, ignoring the "ready" timer |
| GetProScreenFloatValForIndex | int index -> int |  |
| GetProScreenIntValForIndex | int index -> int |  |
| GetProjectilesPerShot | () -> int | Gets the number of projectiles per shot |
| GetRechamberMilestone | () -> int |  |
| GetReloadMilestoneIndex | () -> int |  |
| GetRodeoDamage | () -> int | Get the damage amount this weapon should do to a titan that the player is rodeoing |
| GetScriptFlags0 | () -> int |  |
| GetScriptInt0 | () -> int |  |
| GetScriptTime0 | () -> float |  |
| GetShotCount | () -> int |  |
| GetSustainedDischargeDuration | () -> float | Gets the total duration of a sustained discharge |
| GetSustainedDischargeFraction | () -> float | Gets the fraction of completion for the current sustained discharge between \[0, 1\] |
| GetSustainedDischargePulseFrequency | () -> float | Gets the frequency at which pulse callbacks are dispatched if enabled. Also controls frequency of sustained laser damage |
| GetSustainedDischargeRemainder | () -> float | Gets the time remaining for the current sustained discharge between |
| GetWeaponActivity | () -> Activity | Gets the activity that the weapon is in |
| GetWeaponAmmoPoolType | () -> eAmmoPoolType | Gets the ammo pool type this weapon uses |
| GetWeaponBurstFireCount | () -> int | Get the burst fire count |
| GetWeaponChargeEnergyCost | () -> int |  |
| GetWeaponChargeFraction | () -> float | Returns fraction \[0,1\] where the charge level is |
| GetWeaponChargeLevel | () -> int |  |
| GetWeaponChargeLevelMax | () -> int |  |
| GetWeaponChargeTime | () -> float | Returns how long the weapon has been charging |
| GetWeaponChargeTimeRemaining | () -> float | Returns how long the weapon has left to charge |
| GetWeaponCharmIndex | () -> int | Get script index for the weapon charm |
| GetWeaponClass | () -> string | Gets the string specified in the weapon's .txt file for weaponClass (human \| titan \| drone) |
| GetWeaponClassName | () -> string | Returns the class name of the weapon |
| GetWeaponCurrentEnergyCost | () -> int |  |
| GetWeaponDamageFlags | () -> DamageFlags |  |
| GetWeaponDamageForce | () -> float |  |
| GetWeaponDefaultEnergyCost |  |  |
| GetWeaponDescription | () -> string | Returns the description of the weapon |
| GetWeaponExplosionDamageFlags |  |  |
| GetWeaponInfoFileKeyField | string key -> ? | Resolves a string key to its value in this weapons info file |
| GetWeaponInfoFileKeyFieldAsset | string key -> asset | Resolves a string key to its asset in this weapons info file |
| GetWeaponOwner | () -> entity | Returns entity using the weapon |
| GetWeaponPrimaryAmmoCount | AmmoSource source -> int | Get the amount of ammo available for this weapon to use |
| GetWeaponPrimaryAmmoCountMax | AmmoSource source -> int | Get the max ammo that can be available for this weapon to use |
| GetWeaponPrimaryClipCount | () -> int | Returns the amount of primary ammo in the clip |
| GetWeaponPrimaryClipCountMax | () -> int | Returns the max amount of primary ammo that can be in the clip |
| GetWeaponPrintName | () -> string | Returns the display name of the weapon |
| GetWeaponReadyHint |  |  |
| GetWeaponReadyMsg |  |  |
| GetWeaponReadyToFireProgress | () -> float |  |
| GetWeaponSettingAsset | eWeaponVar weaponVar -> asset | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingBool | eWeaponVar weaponVar -> bool | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingEnum | eWeaponVar weaponVar, table enumType -> int | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingFloat | eWeaponVar weaponVar -> float | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingInt | eWeaponVar weaponVar -> int | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingString | eWeaponVar weaponVar -> string | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponSettingVector | eWeaponVar weaponVar -> vector | Retrieve a weapon's current setting. Must be a valid modable eWeaponVar |
| GetWeaponShieldScale | () -> float |  |
| GetWeaponType | () -> WeaponType | Returns weapon type |
| GetWeaponTypeFlags | () -> int | Get Weapon Type Flags |
| GetWeaponUtilityEntity | () -> entity | Get the weapon's utility entity |
| GetWeaponViewmodel | () -> entity | Gets the viewmodel for the weapon. Viewmodels are only valid for active player weapons |
| GetWeaponZoomFOV | () -> float | Gets the current zoom FOV of the weapon |
| HasMod | string mod -> bool | Given (string), returns true if mod is active on this weapon |
| HasSilencer | () -> bool | Returns if weapon has a silencer |
| HideWeapon | () -> void | Hide the weapon |
| IsBurstFireInProgress | () -> bool | Returns true if a burst fire is in progress |
| IsChargeWeapon | () -> bool | Returns true if the weapon has a charge ability |
| IsCooldownPending | () -> bool | Returns true if weapon is has a cooldown state pending |
| IsDiscarding | () -> bool | True if the weapon is being discarded and will be removed from the owner's inventory |
| IsDischarging | () -> bool | Indicates if the weapon is currently performing a sustained discharge |
| IsForceRelease | () -> bool | Returns true if the offhand weapon was forced to release |
| IsInCooldown | () -> bool | Returns true if weapon is in a cooldown state |
| IsInCustomActivity | () -> bool | Queries whether the weapon viewmodel is currently playing a custom activity |
| IsLoadoutPickup | () -> bool |  |
| IsNetOptimized | () -> bool | Returns true if this weapon is net optimized *and* net weapon optimizations are enabled ('net_optimize_weapons 1') |
| IsOverheated | () -> bool | Returns true if the weapon needs to complete an overheat cooldown |
| IsReadyToFire | () -> bool | Returns true if weapon is ready to fire (based on next allowed attack time) |
| IsReloading | () -> bool | Returns true if the weapon is reloading |
| IsSustainedDischargeWeapon | () -> bool | Indicates if this is a sustained discharge weapon |
| IsSustainedLaserWeapon | () -> bool | Indicates if this is a sustained laser weapon |
| IsTossWeapon | () -> bool | Returns true if this is a toss weapon |
| IsWeaponAdsButtonPressed | () -> bool | Returns true if the ADS button is pressed, even if the weapon doesn't allow zooming |
| IsWeaponCharging | () -> bool | Returns true if the weapon is currently charging |
| IsWeaponInAds | () -> bool | Returns true if the weapon is in ADS |
| IsWeaponMelee | () -> bool | Returns true if this is a melee weapon |
| IsWeaponOffhand | () -> bool | Returns true if the weapon is offhand |
| IsWeaponRegenDraining | () -> bool | Gets whether or not the regen ammo on this weapon is draining or not |
| LookupViewModelAttachment | string -> int | Returns index for the given attachment on the weapon's view model |
| LookupWorldModelAttachment | string -> int | Returns index for the given attachment on the weapon's world model |
| OverrideNextAttackTime |  |  |
| PlayWeaponEffect | asset, asset, string, bool persistent = false -> void | Plays the effect on the weapon |
| PlayWeaponEffectNoCull | asset, asset, string, bool persistent = false -> void | Plays the effect on the weapon, always spawn even if out of view |
| PlayWeaponEffectOnOwner | asset, int -> void | Plays the effect on the weapons owner, use this when the weapon does NOT have a world model |
| PlayWeaponEffectReturnViewEffectHandle | asset, asset, string -> int | Plays the effect on the weapon and return an effect handle to view model effect |
| Raise | () -> void | Triggers weapon raise (or equip) |
| RealtimeMod_GetPendingCommands | () -> array< string > | Get all pending realtime mod commands. +mod_name/-mod_name for add/remove |
| RegenerateAmmoReset | () -> void |  |
| RemoveMod | string mod -> void | Given (string), remove the mod from this weapon |
| ResetWeaponToDefaultEnergyCost | () -> void |  |
| SetChargeAnimIndex | int index -> void |  |
| SetDroppedModel | _possibly_ asset -> void |  |
| SetForcedADS | () -> void | Forces the player to ads |
| SetLegendaryModelIndex | int legendaryIndex -> void | Set the legendary weapon model index for this instance of the weapon. The weapon will use the dafault model from weapon info if a negative index is set |
| SetLifetimeShotsRemaining | int count -> void |  |
| SetLifetimeShotsRemainingInfinite | () -> void |  |
| SetModBitField | int bitfield -> void | Sets mods bit field |
| SetMods | array< string > mods -> void | Reset and apply active mods on a weapon |
| SetNextAttackAllowedTime | float time -> void | Set this weapon's internal when-can-I-shoot-next time |
| SetScriptFlags0 | int flags -> void |  |
| SetScriptInt0 | int -> void |  |
| SetScriptTime0 | float time -> void |  |
| SetSustainedDischargeFractionForced | float fraction -> void | Forces the discharge to be at a certain fraction |
| SetViewmodelAmmoModelIndex | int index -> void | Set the index for bodygroup "ammo", if it exists |
| SetWeaponBurstFireCount | int burstFireCount -> void | Set the burst fire count |
| SetWeaponCamo | int -> void | Sets the camo index on the weapon |
| SetWeaponChargeFraction | float -> void | Sets charge of the weapon as a fraction \[0,1\] |
| SetWeaponChargeFractionForced | float -> void |  |
| SetWeaponCharm | asset weaponCharmModel, string attachmentName -> void | Set weapon charm for the model. This spawns an entity with the provided model and attach it to the CHARM attachment on the weapon |
| SetWeaponCharmIndex | int charmScriptIndex -> void | Set script index for weapon charm |
| SetWeaponEnergyCost | int cost -> void |  |
| SetWeaponPrimaryAmmoCount | AmmoSource source, int count -> void | Set the amount of primary ammo |
| SetWeaponPrimaryClipCount | int count -> void | Set the amount of primary ammo in the clip |
| SetWeaponPrimaryClipCountAbsolute | int count -> void | Set the amount of primary ammo in the clip |
| SetWeaponPrimaryClipCountNoRegenReset | int count | Sets primary ammo count, doesn't reset regen |
| SetWeaponSkin | int -> void | Sets the skin index on the weapon |
| ShouldAutoCycleWhenOutOfAmmo | () -> bool |  |
| ShouldPredictProjectiles | () -> bool | Returns true if it is appropriate to fire predicted projectiles on the client |
| ShowWeapon | () -> void  | Show the weapon |
| SmartAmmo_Clear | bool clearStoredTargets, bool clearTrackers -> void | Clears all current smart ammo targets |
| SmartAmmo_GetFirePosition | entity, int -> vector | Returns the position to fire at for this target |
| SmartAmmo_GetNewTargetTime | () -> float | Returns the last time a new target was acquired |
| SmartAmmo_GetNumTrackersOnEntity | entity target -> int | Returns number of trackers currently on entity |
| SmartAmmo_GetSearchAngle | () -> float | Returns the angle used by the smart ammo cone search |
| SmartAmmo_GetStoredTarget | () -> array< entity > | Returns the list of targets that was last stored |
| SmartAmmo_GetTargets | () -> array< SmartAmmoTarget > | Returns a list of targets currently being tracked by the smart ammo system and their current and previous lock fractions |
| SmartAmmo_GetTrackedEntities | () -> array< entity > | Returns array of all entities currently tracked by this weapon |
| SmartAmmo_IsEnabled | () -> bool | Returns true if smart ammo tracking is enabled |
| SmartAmmo_IsVisibleTarget | entity target | Returns true if the given target is visible to the weapon |
| SmartAmmo_SetNewTargetTime | float time -> void | Let script inform code it started locking on a new target in this tick |
| SmartAmmo_SetTarget | entity, float -> void | Appends new smart ammo target if not already in the list |
| SmartAmmo_StoreTargets | () -> void | Stores the current list of smart ammo targets for later retrieval |
| SmartAmmo_TrackEntity | entity target, float duration -> void | Marks an entity as trackable by the smart ammo system |
| SmartAmmo_UntrackEntity | entity target -> void | Clears an entity as trackable by the smart ammo system |
| StartCustomActivity |  | Plays the given activity on the weapon viewmodel |
| StopCustomActivity |  | Stops any custom activities currently playing on the weapon viewmodel |
| StopWeaponEffect | asset, asset -> void | Stops the effect on the weapon |
| StopWeaponSound | string -> void | Stops the sound on the weapon |
| TimeUntilReadyToFire | () -> float | Returns time remaining until ready to fire |
| UsesClipsForAmmo | () -> bool | True if the weapon uses clips for ammo |
| Weapon_CreateClientOnlyModel |  |  |
| Weapon_DestroyClientOnlyModel |  |  |
| Weapon_GetClientOnlyModel |  |  |
| ZiplineGrenadeHasValidSpot | () -> bool |  |
|  |  |  |