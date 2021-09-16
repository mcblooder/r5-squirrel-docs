C_BaseEntity: Root class of all entities

| Squirrel Name | Type Info | Comment | SERVER | CLIENT |
| ------------- | --------- | ------- | ------ | ------ |
| AddToAllRealms | () -> void | Adds the entity to all the realms | + |  |
| AddToOtherEntitysRealms | entity otherEntity -> void | Add this entity to all the realms the other entity belongs to, in addition to the current realms the entity is in | + | + |
| AddToRealm | int realmIndex -> void | Adds the entity to the realm | + |  |
| AddToSpatialPartition | () -> void | Add entity to spatial partition data | + |  |
| AddUsableValue | int -> void | Adds a usable type to the entity. Should not be called often as need to recompute partition mask everytime a new value is added | + |  |
| AllowMantle | () -> void | Allows mantling on this entity (normally disabled for non-pusher entities) | + |  |
| AllowZiplines | () -> void | Allow ziplines to attach to this mover | + |  |
| CanBeMeleed | () -> bool | Get Whether a script entity can be meleed - Damage and Lunge | + | + |
| CanCloak | () -> bool | Gets whether the entity can cloak or not | + | + |
| ClearBoneMerge | () -> void | Clear bone merge and unlink from parent | + |  |
| ClearBossPlayer | () -> void | Clear this entity of any player ownership | + |  |
| ClearHitboxAttachedChildren | () -> void | Clears all children attached to hitboxes | + |  |
| ClearInvulnerable | () -> void | Decrement invulnerability counter. IsInvulnerable will return true as long as that counter is > 0. | + |  |
| ClearParent | () -> void | Clears the parent of an entity. Must be a clientside entity | + | + |
| Code_SetTeam | int -> void |  | + | + |
| ConnectOutput | string eventName, void functionref( entity self, entity activator, entity caller, var value ) -> void | Adds an I/O connection that will call the named function when the specified output fires | + |  |
| CopyGenericKeyValues | entity -> void |  | + |  |
| CopyHighlightState | entity ent -> void | Copy the highlight state of the entity ent to this entity |  | + |
| CreateTableFromModelKeyValues | () -> table | Creates and returns a script table from the entity's model's $keyvalues block | + | + |
| Destroy | () -> void | Destroys the entity | + | + |
| Die | entity attacker = null, entity inflictor = null, table additional -> void | Kill the entity. Additional params table can contain: weapon, origin, force, forceKill, scriptType, damageSourceId, attackerClass, meleeAttack, meleeExecution, hitbox | + |  |
| DisableAttackableByAI | () -> void | Clear this entity from being a threat to AI | + |  |
| DisableDraw | () -> void | Disabling rendering of this entity.  Attached effects with render |  | + |
| DisableGrappleAttachmen | () -> void | Prevents grapple from attaching to this entity | + |  |
| DisableHealthChangedCallback | () -> void | Unregisters the entity from having the script function ClientCallback_OnHealthChanged called when their health changes |  | + |
| DisableHibernation | () -> void | Prevents this entity from ever hibernating (so it is sent to all clients). Consider using MinimizeHibernation() instead | + |  |
| DisableIdLights | () -> void | Disables Id lights on this entity | + | + |
| DisablePhysics | () -> void | Turns off physics collision (for bouncy rolly type physics) | + |  |
| DisableRenderAlways | () -> void | Set this entity to not render always | + | + |
| DisableRenderWithCockpit | () -> void | Causes entity to NOT render with the cockpit |  | + |
| DisableRenderWithHud | () -> void | Causes entity to NOT render with the hud |  | + |
| DisableRenderWithViewModels | () -> void | Causes entity to NOT render in the view model pass |  | + |
| DisableRenderWithViewModelsNoZoom | () -> void | Causes entity to NOT render with viewmodels, but doesn't zoom in when ADS |  | + |
| DisallowZiplines | () -> void | Disallow ziplines to attach to this mover | + |  |
| DisconnectOutput | string eventName, void functionref( entity self, entity activator, entity caller, var value ) -> void | Removes a connected script function from an I/O event | + |  |
| DispatchImpactEffects | entity target, vector startPos, vector endPos, vector direction, int surfaceProp, int staticProp, int codeDamageType, int impactIndex, entity attacker, int impactEffectFlags -> void |  | + | + |
| DoDeathCallback | bool -> void | Turn on/off death callback on entity |  | + |
| DoesShareRealms | entity otherEntity -> bool | Check if the entity shares a realm with this entity | + | + |
| DontIncludeParentBbox | () -> void | Don't create a giant bounding box even though we are attached to an attachment | + | + |
| DumpParentingState | () -> void | Prints information about the entity's parenting | + |  |
| EnableAttackableByAI | AIPriority priority, int extraPriority, AIAPFlag extraPriorityFlags -> void | Make AI treat this as a threat. Compare priority with values set in player and AI settings files. Flags are prefixed AI_AP_FLAG_* | + |  |
| EnableDraw | () -> void | Draw this entity |  | + |
| EnableGrappleAttachment | () -> void | Prevents grapple from attaching to this entity | + |  |
| EnableHealthChangedCallback | () -> void | Registers the entity to have the script function ClientCallback_OnHealthChanged called when their health changes |  | + |
| EnableHibernation | () -> void | Returns this entity to normal hibernation behavior | + |  |
| EnableIdLights | () -> void | Enables Id lights on this entity | + | + |
| EnableRenderAlways | () -> void | Set this entity to render always | + | + |
| EnableRenderWithCockpit | () -> void | Causes entity to render with the cockpit |  | + |
| EnableRenderWithHud | () -> void | Causes entity to render with the hud |  | + |
| EnableRenderWithViewModels | () -> void | Causes entity to render in the view model pass |  | + |
| EnableRenderWithViewModelsNoZoom | () -> void | Causes entity to render with viewmodels, but doesn't zoom in when ADS |  | + |
| EyeAngles | () -> vector | Get eye angles | + | + |
| EyePosition | () -> vector | Get vector to eye position - absolute coords | + | + |
| FirstMoveChild | () -> entity |  | + |  |
| ForceShadowVisible | bool -> void | Force entity to have shadows even if it isn't visible to the client.  Useful for makingt he thirdperson model cast a shadow while in first person |  | + |
| GetAbsOrigin | () -> vector |  | + | + |
| GetAbsVelocity | () -> vector |  | + | + |
| GetAngles | () -> vector | Get entity pitch, yaw, roll as a vector | + | + |
| GetAngularVelocity | () -> vector | Get the local angular velocity - returns a vector of pitch,yaw,roll | + |  |
| GetArmorType | () -> ArmorType | Get the entity's armor type | + | + |
| GetBaseVelocity | () -> vector | Gets the "base" velocity, typically given to an entity from the last pusher it touched | + |  |
| GetBlocksLOS | () -> bool | Gets whether this entity will block AI LOS | + |  |
| GetBlocksRadiusDamage | () -> bool | Gets whether this flag is set | + |  |
| GetBodygroupNameFromHitboxId | int hitBox -> string | Returns Body group name from the hitboxid | + | + |
| GetBossPlayer | () -> entity | Gets the boss player for an entity | + | + |
| GetBossPlayerName | () -> string | Get's the entity's boss player's name |  | + |
| GetBoundingMaxs | () -> vector | Get a vector containing max bounds, centered on object | + | + |
| GetBoundingMins | () -> vector | Get a vector containing min bounds, centered on object | + | + |
| GetCenter | () -> vector | Get vector to center of object - absolute coords | + |  |
| GetChildren | () -> array < entity > | Get list of children entities. ( Entities that have this as the move parent. ) |  | + |
| GetClassName | () -> string | Reliably returns server-side class name | + |  |
| GetCloakEndTime | () -> float | Return when cloak ends (ie, when fade-in begins) | + | + |
| GetCloakFadeFactor | () -> float | Return the cloak fade time amount (0 = off, 1 = on) |  | + |
| GetCodeClassName | () -> string | Avoid using outside of debug code | + | + |
| GetCritsPrevented | () -> bool |  | + | + |
| GetDamage | () -> float | Returns the amount of damage this entity would potentially inflict | + |  |
| GetEncodedEHandle | () -> int | Get an encoded handle to this ent, suitable for sending to client script | + | + |
| GetEntIndex | () -> int |  | + | + |
| GetEntityName | () -> string |  |  | + |
| GetForwardVector | () -> vector | Get the forward vector of the entity | + | + |
| GetGrade | () -> int |  | + | + |
| GetGroundEntity | () -> entity | Return ground entity | + | + |
| GetGroundRelativePos | () -> vector | Transform a world space position to where it would be if moving ground entity is in its original position | + |  |
| GetHealth | () -> int | Gets this entity's health | + | + |
| GetIndexForEntity | () -> int | Get an index that can be used for kill replay | + |  |
| GetInstanceName | () -> string | Returns the instance_name of this entity | + | + |
| GetLifeState | () -> int |  | + | + |
| GetLinkEnt | () -> entity | Returns the single entity this entity is linked to (if there is one) | + | + |
| GetLinkEntArray | () -> array< entity > | Returns array of entities that this entity is linked to | + | + |
| GetLinkParent | () -> entity | Returns the single entity that connects to this entity (if there is one) | + | + |
| GetLinkParentArray | () -> array< entity > | Returns array of entities that are linked to this entity | + | + |
| GetLocalAngles | () -> vector | Get entity pitch, yaw, roll as a vector relative to parent | + | + |
| GetLocalOrigin | () -> vector |  | + | + |
| GetLocalVelocity | () -> vector | Returns the local velocity of this entity | + | + |
| GetMaxHealth | () -> int | Gets this entity's maximum health | + | + |
| GetModelName | () -> asset | Returns the name of the model | + | + |
| GetNetBool | string networkVariableName -> bool | Gets a bool network variable (see RegisterNetworkedVariable) | + | + |
| GetNetEnt | string networkVariableName -> _possibly_ entity | Gets an entity network variable (see RegisterNetworkedVariable) | + | + |
| GetNetFloat | string networkVariableName -> float | Gets a float network variable (see RegisterNetworkedVariable) | + | + |
| GetNetInt | string networkVariableName -> int | Gets an int network variable (see RegisterNetworkedVariable) | + | + |
| GetNetTime | string networkVariableName -> float | Gets a time (float) network variable (see RegisterNetworkedVariable) | + | + |
| GetNetworkedClassName | () -> string | Works on both server and client. Can return null | + | + |
| GetNextKey |  | Takes a key in the entity's key value list and returns the next key. Useful for iterating through key values | + | + |
| GetNoTarget | () -> bool |  | + | + |
| GetNoTargetSmartAmmo | () -> bool | Get whether the smart ammo system can see this target | + | + |
| GetOrigin | () -> vector |  | + | + |
| GetOwner | () -> entity | Gets this entity's owner | + | + |
| GetParent | () -> entity | If in hierarchy, retrieves the entity's parent | + | + |
| GetParentAttachment | () -> string | Gives the name of the attachment that we are parented to | + | + |
| GetParentAttachmentIndex | () -> int | Gives the index of the attachment that we are parented to | + | + |
| GetParentHitbox | () -> int | Gives the index of the hitbox that we are parented to | + | + |
| GetPassDamageToParent | () -> bool |  | + |  |
| GetPassThroughFlags | () -> int |  | + | + |
| GetPhysics | () -> MoveType | Gets the move type | + | + |
| GetPhysicsSolidMask | () -> int | Gets the solid mask for this entity | + |  |
| GetPreTemplateName | () -> string | Get the entity name stripped of template unique decoration | + | + |
| GetPusher | () -> bool | Sets whether this entity pushes other entities | + |  |
| GetRealms | () -> array< int > | Get list of realms this entity belongs to | + | + |
| GetRightVector | () -> vector | Get the right vector of the entity | + | + |
| GetRootMoveParent | () -> entity | If in hierarchy, walks up the hierarchy to find the root parent | + |  |
| GetScriptId | () -> string | Retrieve the unique identifier used to refer to the entity within the scripting system | + | + |
| GetScriptName | () -> string | Returns the script_name of this entity | + | + |
| GetScriptScope | () -> table | Retrieve the script-side data associated with an entity | + | + |
| GetSharedRealms | entity otherEntity -> array< int > | Get list of realms this entity shares with the other entity | + | + |
| GetShieldHealth | () -> int |  | + | + |
| GetShieldHealthMax | () -> int |  | + | + |
| GetSmoothedVelocity | () -> vector | Get velocity that is weighted averaged with previous velocity | + |  |
| GetSpawner | () -> entity | Returns spawner that created this entity, if it was created from one | + |  |
| GetSquadID | () -> int |  | + | + |
| GetTargetName | () -> string |  | + | + |
| GetTarget_Deprecated | () -> string | Shortcut for GetValueForKey( "target" ) | + | + |
| GetTeam | () -> int |  | + | + |
| GetTeamMemberIndex | () -> int |  | + | + |
| GetTimeSinceSpawning | () -> float | Return the time that this entity spawned | + |  |
| GetTitle | () -> string | Gets an entity's title. This may be displayed on client HUD's | + |  |
| GetTitleForUI | () -> string |  |  | + |
| GetUpVector | () -> vector | Get the up vector of the entity | + | + |
| GetUsableValue | () -> int | Returns an integer representing of the usable state, so that you can return to this state later | + |  |
| GetValueForEffectNameKey | () -> asset | type safe equivalent of effect_name = ent.kv.effect_name | + | + |
| GetValueForKey | string -> string | Get a string representation of the specified key's value | + | + |
| GetValueForModelKey | () -> asset | type safe equivalent of model = ent.kv.model | + | + |
| GetValueForTextureKey | () -> asset | type safe equivalent of texture = ent.kv.texture | + | + |
| GetVelocity | () -> vector | Returns the absolute velocity of this entity | + | + |
| GetWorldSpaceCenter | () -> vector | Get the centerpoint of an entity | + |  |
| HasGibModel | () -> bool | True if the entity has gib models | + | + |
| HasKey | string -> bool | Returns true if the specified key exists on the entity | + | + |
| HasOutput | string -> bool | Returns true if an entity has an output of the given name | + |  |
| HasPusherAncestor | () -> bool | True if entity is parented to a pusher | + | + |
| Hide | () -> void | Make a client-side entity invisible to a local player (0 = first player, 1 = next player, etc.) | + | + |
| HighlightDisableForTeam | int team -> void |  | + | + |
| HighlightEnableForTeam | int team -> void |  | + | + |
| HighlightSetTeamBitField | int -> void |  | + | + |
| Highlight_Enable | () -> void | Enable highlighting on this entity | + | + |
| Highlight_GetCurrentContext | () -> HighlightContext | Get the current highlight context | + | + |
| Highlight_GetCurrentInsideOpacity | () -> float | Get the inside opacity on the current context | + | + |
| Highlight_GetCurrentOutlineOpacity | () -> float | Get the outline opacity on the current context | + | + |
| Highlight_GetFarFadeDist | () -> float | Gets far fade dist |  | + |
| Highlight_GetFlag | HighlightFlag flag -> bool | Gets whether or not a flag is active on a highlight |  | + |
| Highlight_GetInheritHighlight | () -> bool | Tells if this entity can inherit the highlighting settings from a parent entity if there is no local settings | + | + |
| Highlight_GetInsideFunction | HighlightContext contextId -> int | Get the inside function slot on the given context. 0 for a disabled a function | + | + |
| Highlight_GetNearFadeDist | () -> float | Gets near fade dist |  | + |
| Highlight_GetOutlineFunction | HighlightContext contextId -> int | Get the outline function slot on the given context. 0 for a disabled a function | + | + |
| Highlight_GetOutlineRadius | HighlightContext contextId -> float | Get the outline radius on the given context | + | + |
| Highlight_GetParam | HighlightContext contextId, int param -> vector | 'Get custom parameters on the given context. Parameters are shared between inside and outline functions | + | + |
| Highlight_GetState | HighlightContext contextId -> int | Get custom state on the given context. Parameters are shared between inside and outline functions | + | + |
| Highlight_HideInside | float duration -> void | Hide inside function in a given duration. 0 to hide immediately | + | + |
| Highlight_HideOutline | float duration -> void | Hide outline function in a given duration. 0 to hide immediately | + | + |
| Highlight_IsAfterPostProcess | HighlightContext contextId -> bool | Tells if this highlight will be drawn after all post-processes | + | + |
| Highlight_IsEntityVisible | HighlightContext contextId -> bool | Tells if this entity will be drawn | + | + |
| Highlight_PopPingedState | () -> void |  |  | + |
| Highlight_PushPingedState | () -> void |  |  | + |
| Highlight_ResetFlags | () -> void | Sets the highlight flags back to 0 |  | + |
| Highlight_SetCurrentContext | HighlightContext contextId -> void | Set the current highlight context. 0 by default. Server has priority over client. Use context -1 to disable highlighting | + | + |
| Highlight_SetFadeInTime | float duration -> void | Sets fade in time for highlight |  | + |
| Highlight_SetFadeOutTime | float duration -> void | Sets fade out time for highlight |  | + |
| Highlight_SetFarFadeDist | float distance -> void | Sets far fade dist |  | + |
| Highlight_SetFlag | HighlightFlag flag, bool value -> void | Sets a flag to active or not on a highlight |  | + |
| Highlight_SetFunctions | HighlightContext contextId, int insideSlot, bool entityVisible, int outlineSlot, float outlineRadiusl, int state bool afterPostProcess -> void | Set function slots on the given context. Use slot 0 to disable a function | + | + |
| Highlight_SetInheritHighlight | bool -> void | Set if this entity can inherit the highlighting settings from a parent entity if there is no local settings. False by default. Shared by all contexts | + | + |
| Highlight_SetLifeTime | float duration -> void | Sets how long the highlight lasts for before fading out |  | + |
| Highlight_SetNearFadeDist | float distance -> void | Sets near fade dist |  | + |
| Highlight_SetParam | HighlightContext contextId, int, vector -> void| Set custom parameters on the given context. Parameters are shared between inside and outline functions | + | + |
| Highlight_SetVisibilityType | HighlightVisibility visibility -> void | Sets visibility type for highlight |  | + |
| Highlight_ShowInside | float duration -> void | Show inside function in a given duration. 0 to show immediately | + | + |
| Highlight_ShowOutline | float duration -> void | Show outline function in a given duration. 0 to show immediately | + | + |
| Highlight_StartOn | () -> void | Starts the highlight as on no matter what |  | + |
| IsBreakableGlass | () -> bool | True if the entity is breakable glass | + | + |
| IsChild | entity ent -> bool | Returns true if given entity is already a child of this entity | + |  |
| IsClientOnly | () -> bool | Returns whether this entity is client only |  | + |
| IsCloaked | bool -> bool | Return if player is cloaked | + | + |
| IsDraw | () -> bool |  | + |  |
| IsEntAlive | () -> bool | Is this entity alive? | + | + |
| IsFuncBrush | () -> bool | Returns true if entity is a func_brush entity | + | + |
| IsHidden | () -> bool | Check if the entity is hidden ( Hide function for client entities )  |  | + |
| IsHighlightEnabledForTeam | int team -> bool |  | + | + |
| IsHologram | () -> bool | True if the entity is a hologram | + | + |
| IsHuman | () -> bool | True if the entity is human type | + | + |
| IsIgnoredByAimAssist | () -> bool | True if this entity is ignored by the aimassist system |  | + |
| IsInRealm | int realmIndex -> bool | Check if the entity belongs to the realm | + | + |
| IsInvulnerable | () -> bool | Returns whether the entity is invulnerable to damage |  | + |
| IsInvulnerable | () -> bool | Returns whether the entity is invulnerable to damage | + |  |
| IsLinkedToEnt | entity ent -> bool | Returns true if there exists a link from this entity to the given entity | + |  |
| IsMarkedForDeletion | () -> bool | True if this entity is being removed (deleted or killed) | + | + |
| IsMechanical | () -> bool | True if the entity is mechanical type | + | + |
| IsNPC | () -> bool | Returns true if entity is an NPC | + | + |
| IsOnGround | () -> bool | True if standing on something | + | + |
| IsOperator | () -> bool | True if the entity is human type |  | + |
| IsPhaseShifted | () -> bool |  | + | + |
| IsPlayer | () -> bool | Returns true if entity is a player | + | + |
| IsPlayerDecoy | () -> bool | True if the entity is a player decoy | + | + |
| IsPredictedProjectile | () -> bool | Returns true if the entity is a predicted projectile |  | + |
| IsProjectile | () -> bool | Returns true if this is a projectile | + | + |
| IsRenderingWithViewModels | () -> bool | Returns true if the entity is rendering in the view model pass | + | + |
| IsRopeZipline | () -> bool | True if the entity is a zipline type |  | + |
| IsSolid | () -> bool | Returns true if solid entity | + |  |
| IsTitan | () -> bool | True if the entity is titan type | + | + |
| IsTriggerBox | () -> bool | Returns true if this is a trigger box | + |  |
| IsValidAIMeleeTarget | () -> bool | Gets if AI can melee this entity | + |  |
| IsWorld | () -> bool | Returns true if entity is the world entity | + | + |
| IsZipline | () -> bool | True if the entity is a zipline type | + | + |
| LagCompensate | bool -> void | Make entity do lag compensation | + |  |
| LinkToEnt | entity ent -> void | Creates a link from the current entity to the given entity | + |  |
| LookupAttachment | string attachment -> int | Get the named attachement id |  | + |
| MakeInvisible | () -> void | Hides this entity and its children (entity still gets sent to the client, it just isn't rendered) | + |  |
| MakeVisible | () -> void | Shows this entity | + |  |
| MarkAsNonMovingAttachment | () -> void | Marks this entity as an attachment that never moves away from the attachment point | + | + |
| Minimap_AlwaysShow | int team, entity ent -> void | Forces this entity to show up on client minimaps that match the team or player handle | + |  |
| Minimap_DisplayDefault | int team, entity ent -> void | Allows this entity to do default draw behavior on client minimaps that match the team or player handle (This is exclusive with AlwaysShow/Hide) | + |  |
| Minimap_GetCustomState | () -> int |  |  | + || SetVisibleForLocalPlayer | int -> void | Make a client-side entity visible to a local player (0 = first player, 1 = next player, etc.) |  | + |
| Minimap_GetZOrder | () -> int |  |  | + |
| Minimap_Hide | int team, entity ent -> void | Forces this entity to NOT show up on client minimaps that match the team or player handle | + |  |
| Minimap_SetAlignUpright | bool -> void | Tell this entity whether to draw always upright on client minimaps | + |  |
| Minimap_SetClampToEdge | bool -> void | Tell this entity whether to clamp to the edges of client minimaps when drawing | + |  |
| Minimap_SetCustomState | int -> void | A custom integer that can be RUI tracked on the client. Code behavior isn't affected by this variable. Must be positive or 0 | + |  |
| Minimap_SetHeightTracking | bool -> void | Tell this entity whether to use height tracking behavior on client minimaps | + |  |
| Minimap_SetObjectScale | float scale -> void | The size ratio of this icon relative to the size of the smaller side of client minimaps. Values around 0.1 are ideal | + |  |
| Minimap_SetZOrder | MinimapZ z -> void | The z order of this entity on the minimap relative to all other minimap entities. Larger values draw on top. Must be positive or 0 | + |  |
| MinimizeHibernation | () -> void | Makes this entity only hibernate beyond hibernation_far_dist | + |  |
| NextMovePeer | () -> entity |  | + |  |
| NotSolid | () -> void | Set the entity to be not solid | + |  |
| PhysicsSetAutoDisableNotifications | bool -> void | Sets whether CodeCallback_OnPhysicsAutoDisable() should be called for this entity | + |  |
| PhysicsSetDamping | float, float -> void | ( linear, angular ) Set damping on the entity's physics object. 0 to infinity. | + |  |
| PhysicsSetFriction | float -> void | Set friction on the entity's physics object. 0 to infinity | + |  |
| RemoveFromAllRealms | () -> void | Removes the entity from all the realms | + | + |
| RemoveFromRealm | int realmIndex -> void | Removes the entity from the realm | + |  |
| RemoveFromSpatialPartition | () -> void | Remove entity from spatial partition data | + |  |
| RemoveUsableValue | int -> void | Removes a usable type from the entity. Should not be called often as need to recompute partition mask evertime a new value is removed | + |  |
| RenderWithViewModels | bool -> void | Controls whether the given entity is drawn in the view model pass | + | + |
| RoundOriginAndAnglesToNearestNetworkValue | () -> void | Rounds entity origin and angles so they will exactly match on client and server | + |  |
| SetAIObstacle | bool -> void | Make AI try to path around this entity or not | + |  |
| SetAbsAngles | vector -> void | Set entity pitch, yaw, roll relative to world, regardless of parent orientation | + |  |
| SetAbsAnglesSmooth | vector -> void | Set entity pitch, yaw, roll relative to world, regardless of parent orientation. Will smoothly interpolate to the new angles | + |  |
| SetAbsForwardVector | vector -> void | Set the orientation of the entity to have this forward vector relative to the world, regardless of parent orientation | + |  |
| SetAbsOrigin | vector -> void | Sets the position of the entity relative to the world, regardless of parent orientation | + |  |
| SetAbsOriginSmooth | vector -> void | Sets the position of the entity relative to the world, regardless of parent orientation. Does it by smoothly interpolating the entity to the new location | + |  |
| SetAimAssistAllowed | bool -> void |  | + |  |
| SetAlive | bool isAlvie -> void | Make this client entity alive or dead. Needed for id lights to work |  | + |
| SetAngles | vector -> void | Set entity pitch, yaw, roll as a vector | + | + |
| SetAngularVelocity | vector -> void | Set the local angular velocity - takes float pitch,yaw,roll velocities | + |  |
| SetAttachOffsetAngles | vector -> void | Sets the local angles offset of an attached entity |  | + |
| SetAttachOffsetOrigin | vector -> void | Sets the local position offset of an attached entity |  | + |
| SetBaseVelocity | vector -> void | Sets the "base" velocity, typically given to an entity from the last pusher it touched | + |  |
| SetBlocksLOS | bool -> void | Sets whether this entity will block AI LOS | + |  |
| SetBlocksRadiusDamage | bool -> void | Sets whether this entity will block radius damage. An entity may block radius damage for other reasons, but setting this flag ensures that it will | + |  |
| SetBoneMerge | entity -> void | Treat entity as part of parent when calculating animations | + |  |
| SetBossPlayer | entity ent -> void | Mark this entity as belonging to the specified player | + |  |
| SetBoundingBox | vector, vector -> void | Specify the bounding box for this entity, also switch collision over to BBOX (may stop physics movement, etc.) | + |  |
| SetCanBeAimAssistTrackedWhilePhased | bool -> void | Allows ent to have aim assit applied to them on non phased players while they are phased | + | + |
| SetCanBeMeleed | bool -> void | Set Whether a script entity can be meleed - Damage and Lunge | + |  |
| SetCanCloak | bool -> void | Sets whether the entity can cloak or not | + | + |
| SetCloakDuration | float fadeIn, float duration, float fadeOut -> void | Sets the cloak duration: -1 for infinite, 0 to turn off | + |  |
| SetCloakFlicker | float amount, float duration -> void  | Makes existing cloak flicker off for amount: 0..1; duration: -1 for infinite, 0 to turn off | + |  |
| SetCollisionAllowed | bool -> void | Sets whether this object has collision allowed or not. Note that other things might affect this object's collision, like its solid type | + |  |
| SetCollisionDetailHigh | () -> void | Sets the collision detail level of an entity to high | + |  |
| SetDamageNotifications | bool -> void | Sets whether CodeCallback_DamageEntity should be called for this entity. Equivalent to ent.kv.damageNotifications | + |  |
| SetDeathNotifications | bool -> void | Sets whether CodeCallback_OnEntityKilled should be called for this entity. Equivalent to ent.kv.deathNotifications | + |  |
| SetDoDestroyCallback | bool -> void | If true, this entity will be do a callback to script before being destroyed | + | + |
| SetDoPusherCallback | bool -> void | If true, this entity will be do a callback to script whenever it pushes an object | + |  |
| SetFadeDistance | float distance -> void | Set the distance that this entity starts fading | + | + |
| SetForceVisibleInPhaseShift | bool -> void | Forces an entity to be visible during phase shift | + | + |
| SetForwardVector | vector -> void | Set the orientation of the entity to have this forward vector | + |  |
| SetForwardVectorWithUp | vector -> void | Set the orientation of the entity to have this forward vector, based on the given up vector | + |  |
| SetGrade | int grade -> void |  | + |  |
| SetGrenadeTargetDebounce | float -> void | Set the debounce duration for when AI are allowed to throw grenades at this target | + |  |
| SetGroundEntity | entity ent -> void | Sets the ground entity on a given entity | + |  |
| SetHealth | int health -> void |  | + |  |
| SetIgnorePredictedTriggerTypes | int -> void | Sets whether this entity will touch predicted triggers of a type or not | + |  |
| SetInactive | bool -> void | Sets the entity to be active or inactive | + |  |
| SetInvisibleForLocalPlayer | int -> void | Make a client-side entity invisible to a local player (0 = first player, 1 = next player, etc.) |  | + |
| SetInvulnerable | () -> void | Increment invulnerability counter. IsInvulnerable will return true as long as that counter is > 0 | + |  |
| SetIsValidAIMeleeTarget | bool -> void | Sets if AI can melee this entity | + |  |
| SetKillNPCOnPush | bool -> void | Sets whether this entity should kill NPCs when it pushes them | + |  |
| SetLocalAngles | vector -> void | Set entity pitch, yaw, roll as a vector relative to parent | + | + |
| SetLocalForwardVector | vector -> void | Set the orientation of the entity to have this forward vector relative to its parent | + |  |
| SetLocalForwardVectorWithUp | vector -> void | Set the orientation of the entity to have this forward vector, based on the given up vector, relative to its parent | + |  |
| SetLocalOrigin | vector -> void | Sets the position of the entity relative to parent | + | + |
| SetMaxHealth | int maxHealth -> void |  | + |  |
| SetModel | asset -> bool | Set the file path of the model | + | + |
| SetNameVisibleToEnemy | bool -> void | Set player visibility of this entity's name | + |  |
| SetNameVisibleToFriendly | bool -> void | Set player visibility of this entity's name | + |  |
| SetNameVisibleToNeutral | bool -> void | Set player visibility of this entity's name | + |  |
| SetNameVisibleToOwner | bool -> void | Set player visibility of this entity's name | + |  |
| SetNetBool | string networkVariableName, bool value -> void | Sets a bool network variable (see RegisterNetworkedVariable) | + |  |
| SetNetEnt | string networkVariableName, entity value -> void | Sets an entity network variable (see RegisterNetworkedVariable) | + |  |
| SetNetFloat | string networkVariableName, float value -> void | Sets a float network variable (see RegisterNetworkedVariable) | + |  |
| SetNetFloatOverTime | string, float, float -> void | Changes a float network variable gradually over time from its current value to the specified new value (see RegisterNetworkedVariable) | + |  |
| SetNetInt | string networkVariableName, int value -> void | Sets an int network variable (see RegisterNetworkedVariable) | + |  |
| SetNetTime | string networkVariableName, float value -> void | Sets a time (float) network variable (see RegisterNetworkedVariable) | + |  |
| SetNextThinkNow | () -> void | Sets the entity's next think time to as soon as possible. Calling this on multiple entities at the same time will synchronize their think times | + |  |
| SetNoTarget | bool -> void |  | + |  |
| SetNoTargetSmartAmmo | bool -> void |  | + |  |
| SetOrigin | vector -> void | Sets the position of the entity | + | + |
| SetOwner | entity owner -> void |  | + |  |
| SetParent | entity parentEnt, string attachment = "", bool maintainOffset = null, float blendTime = 0 -> void | Parents this entity to another entity | + | + |
| SetParentWithHitbox | entity parentEnt, int hitboxIdx, bool maintainOffset = null, float blendTime = 0 -> void | Parents this entity to another entity's hitbox | + | + |
| SetPassDamageToParent | bool -> void |  | + |  |
| SetPassThroughDirection | float -> void | Sets the direciton the shot has to come from to pass the ent | + | + |
| SetPassThroughFlags | int flags -> void | Sets flags for when pass through happens on this entity | + | + |
| SetPassThroughThickness | float -> void | Sets the thickness of and entity for pass through bullets | + | + |
| SetPhysics | MoveType type -> void | Sets the move type | + | + |
| SetPreventCrits | bool -> void |  | + | + |
| SetPusher | bool -> void | Sets whether this entity pushes other entities | + |  |
| SetScriptName | string -> void | Sets the script_name of this entity | + | + |
| SetSeeOtherNonShifters | bool -> void | Allows the shifter to see others while not in phase shift | + | + |
| SetShieldHealth | int -> void | Set the shield health | + |  |
| SetShieldHealthMax | int -> void | Set the maximum shield health | + |  |
| SetSize | vector, vector -> void |  | + |  |
| SetSoundCodeControllerValue | float -> void | Set sound 'code' controller for sounds attached to entity. Overrides code value (if any). (The client-side version of this script hook is not for server entities!) | + | + |
| SetSquadID | int newID -> void |  | + |  |
| SetTakeDamageType | DamageType type -> void | Sets the take damage type | + | + |
| SetTeamMemberIndex | int newIndex -> void |  | + |  |
| SetTitle | string -> void | Sets an entity's title. This may be displayed on client HUD's | + |  |
| SetToSameParentAs | entity ent -> void | Sets this entity's move parent to be the same as the given entity | + | + |
| SetTouchTriggers | bool -> void | Set whether this entity will touch triggers | + |  |
| SetUsable | () -> void | Marks this entity as usable by any player | + |  |
| SetUsableByGroup | string -> void | Marks this entity as usable by specific players | + |  |
| SetUsableDistanceOverride | float distance -> void | In order for an object to be usable, the player must be a within a certain distance of the object's bounding box. This sets an override for that distance. Must also set flag USABLE_USE_DISTANCE_OVERRIDE to enable. | + |  |
| SetUsableFOV | float -> void | Set fov for this ent to use | + |  |
| SetUsableFOVByDegrees | float -> void | Converts to cosine degrees | + |  |
| SetUsablePriority | UsablePriority priority -> void | Sets the priority of a usable ent | + |  |
| SetUsableValue | int -> void | Sets the usable state by integer, which was earlier obtained from | + |  |
| SetUsePromptSize | float -> void |  | + |  |
| SetUsePrompts | string, string -> void | Sets the entity's hold use and press use prompts | + |  |
| SetValueForEffectNameKey | asset -> void | type safe equivalent of ent.kv.effect_name = effect_name | + | + |
| SetValueForKey | string, string -> void |  | + | + |
| SetValueForModelKey | asset -> void | type safe equivalent of ent.kv.model = model | + | + |
| SetValueForTextureKey | asset -> void | type safe equivalent of ent.kv.texture = texture | + | + |
| SetVelocity | vector -> void |  | + | + |
| SetVisibilityFlags | int flags -> void | Set the visibility flags for a given entity | + | + |
| ShipHack_PositionBetweenEyes | () -> vector | The the position between the entity's eyes | + | + |
| Show | () -> void | Make a client-side entity visible to a local player (0 = first player, 1 = next player, etc.) | + | + |
| SnapToAbsOrigin | vector -> void | Like SetAbsOrigin(), except it will not do any blending/lerping to the new location | + |  |
| Solid | () -> void | Sets an entity to solid ( usually something that had NotSolid called on it ) | + |  |
| StopPhysics | () -> void | Stops physics for an entity | + | + |
| TakeDamage | int damage, entity attacker, entity inflictor, table additionalParams -> void | Deals damage to the entity. Additional params table can contain: weapon, origin, force, forceKill, scriptType, damageSourceId, attackerClass, meleeAttack, meleeExecution, hitbox | + |  |
| TraceAttackToTriggers | int, entity, entity, table, vector, vector, vector -> void  | Does a trace to trigger all triggers along it | + |  |
| TransferChildrenTo | entity -> void | Transfers all children (entities parented to this entity) to another parent. | + |  |
| UnlinkFromEnt | entity ent -> void | Removes a link from the current entity to the given entity | + |  |
| UnsetSoundCodeControllerValue | () -> void | Unset sound 'code' controller for sounds attached to entity. (The client-side version of this script hook is not for server entities!) | + | + |
| UnsetUsable | () -> void | Undoes the effects of SetUsable() | + |  |
| UseHitBoxForTraceCheck | () -> void | Hitbox overrides vphysics for trace checks on this entity | + |  |
| ValidateScriptScope |  | Ensure that an entity's script scope has been created | + | + |
| WorldSpaceSurroundingMaxs | () -> vector | Returns maximum bounds in world-space. This takes into account all movement of the current animation | + | + |
| WorldSpaceSurroundingMins | () -> vector | Returns minimum bounds in world-space. This takes into account all movement of the current animation | + | + |
|  |  |  |  |  |