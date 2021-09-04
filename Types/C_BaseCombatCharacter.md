| Squirrel Name | Type Info | Comment |
| ------------- | --------- | ------- |
| AddSharedEnergy | float | int amount -> void  |  |
| CanUseSharedEnergy | float | int -> bool |  |
| ClearOffhand | () -> void | Clear the player's offhand ability |
| ContextAction_ClearBeingRevived | () -> void | Marks the entity as no longer being revived |
| ContextAction_ClearBusy | () -> void | Marks the entity as no longer doing some kind of context action |
| ContextAction_ClearFastball | () -> void | Marks the entity as no longer executing a fastball |
| ContextAction_ClearInVehicle | () -> void | Marks the entity as no longer inside a vehicle |
| ContextAction_ClearReviving | () -> void | Marks the entity as no longer executing a revive |
| ContextAction_IsActive | () -> bool | Returns whether in the middle of any context action (like melee or leeching) |
| ContextAction_IsBeingRevived | () -> bool | Returns whether the player is in a being-revived context action |
| ContextAction_IsBusy | () -> bool | Returns whether in the middle of a busy context action |
| ContextAction_IsFastball | () -> bool | Returns whether the player is in a fastball context action |
| ContextAction_IsInVehicle | () -> bool | Returns whether the player is in a vehicle context action |
| ContextAction_IsLeeching | () -> bool | Returns whether in the middle of a leeching context action |
| ContextAction_IsMeleeExecution | () -> bool | Returns true if the entity is in the middle of a melee execution context action |
| ContextAction_IsMeleeExecutionAttacker | () -> bool | Returns true if the entity is an attacker in the middle of a melee execution context action |
| ContextAction_IsMeleeExecutionTarget | () -> bool | Returns true if the entity is a target in the middle of a melee execution context action |
| ContextAction_IsRequisitionBattery | () -> bool | Returns whether entity is in the middle of a battery requisition context action |
| ContextAction_IsReviving | () -> bool | Returns whether the player is in a revive context action |
| ContextAction_IsRodeo | () -> bool | Returns whether the player is in a rodeo context action |
| ContextAction_IsZipline | () -> bool | Returns whether the player is in a zipline context action |
| ContextAction_SetBeingRevived | () -> void | Marks the entity as being revived |
| ContextAction_SetBusy | () -> void | Marks the entity as in the middle of a busy context action (so other things don't interrupt them) |
| ContextAction_SetFastball | () -> void | Marks the entity is executing a fastball |
| ContextAction_SetInVehicle | () -> void | Marks the entity as inside a vehicle |
| ContextAction_SetReviving | () -> void | Marks the entity as executing a revive |
| DisablePhaseShiftFlags | () -> void |  |
| EnablePhaseShiftFlags | () -> void |  |
| GetActiveWeapon | eActiveInventorySlot slot -> entity | Returns the active weapon |
| GetActiveWeaponPrimaryAmmoLoaded | int -> int | Get the amount of currently loaded ammo in the active weapon |
| GetAllActiveWeapons | () -> array< entity > | Returns all active weapons. Array indices will not match active weapon slot values and the array will have no null elements |
| GetAntiTitanWeapon | () -> entity | Returns the anti titan weapon |
| GetEntityAtPhaseShiftExitPosition | () -> entity | Gets the entity you are about to phase shift into |
| GetLastFiredTime | () -> float | Returns the last time palyer or NPC fired |
| GetLatestPrimaryWeapon | eActiveInventorySlot slot -> entity | Returns the last primary weapon used |
| GetLatestPrimaryWeaponForIndexZeroOrOne | eActiveInventorySlot slot -> entity |  |
| GetMainWeapons | () -> array< entity > | Get array of the main weapons |
| GetNormalWeapon | WeaponInventorySlot slot -> entity | Get the normal weapon in the specified slot |
| GetOffhandWeapon | Offhand offhand -> entity | Get the offhand weapon in the specified slot |
| GetOffhandWeapons | () -> array< entity > | Get array of the offhand weapons |
| GetPlayerOrNPCViewVector | () -> vector | Gets the view vector of a player or NPC. Prefer GetViewVector or GetNPCViewVector when you know whether you're working with a player or NPC |
| GetSelectedWeapon | eActiveInventorySlot slot -> entity | Returns the selected weapon |
| GetSharedEnergyCount | () -> float |  |
| GetSharedEnergyRegenDelay | float -> void |  |
| GetSharedEnergyRegenRate | () -> float |  |
| GetSharedEnergyTotal | () -> float |  |
| GetSidearmWeapon | () -> entity |  |
| GetTitanSoul | () -> entity | Gets the titanSoul for this entity |
| GetWeaponDisableFlags | () -> WeaponDisableFlags | Returns the weapon disable flags that are active |
| IsPhaseShiftedOrPending | () -> bool |  |
| IsSwitching | WeaponInventorySlot slot -> bool | Returns true if the player is switching weapons in the specified slot |
| IsUsingOffhandWeapon | eActiveInventorySlot slot -> bool | Returns true if player is using an offhand weapon in the active slot |
| IsWeaponSlotDisabled | eActiveInventorySlot slot -> bool | Returns true if the weapon slot is disabled |
| OffsetFromViewAngles | vector offset -> vector | Returns angles that has been offset relative to the view |
| OffsetPositionFromView | vector baseStartPos, vector offset -> vector | Returns position that has been offset relative to the view |
| PhaseShiftBegin | float warmupTime, float duration -> void |  |
| PhaseShiftCancel | () -> void |  |
| PhaseShiftTimePassed | () -> float | Time passed in phase shift |
| PhaseShiftTimeRemaining | () -> float | Time left in phase shift |
| PlayerMelee_ExecutionEndAttacker | () -> void | Let script tell code a melee attack has ended (for the attacker) |
| PlayerMelee_ExecutionEndTarget | () -> void | Let script tell code a melee attack has ended (for the target/victim) |
| PlayerMelee_ExecutionStartAttacker | float duration -> void | Let script tell code a melee attack has started (for the attacker) |
| PlayerMelee_ExecutionStartTarget | entity attacker -> void | Let script tell code a melee attack has started (for the target/victim) |
| SetSelectedOffhand | eActiveInventorySlot slot, entity weapon -> void |  |
| SetSharedEnergyLockoutThreshold | int threshold -> void |  |
| SetSharedEnergyPenaltyDuration | float duration -> void |  |
| SetSharedEnergyRegenDelay | float | int -> void |  |
| SetSharedEnergyRegenRate | int -> void |  |
| SetSharedEnergyTotal | float | int -> void |  |
| TakeSharedEnergy | float | int amount -> void |  |
|  |  |  |