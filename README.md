# r5-squirrel-docs

Type information that I'm not sure about is marked as _possibly_

## Variables
* [Variables](Variables.md)
* [Untested Variables](UntestedVariables.md)

## Important types

* [C_BaseCombatCharacter](Types/C_BaseCombatCharacter.md)
* [C_BaseEntity](Types/C_BaseEntity.md)
* [C_Player](Types/C_Player.md)
* [C_WeaponX](Types/C_WeaponX.md)


## Contribution
I work at my pace and hopefully document most of the methods mentioned in [Methods](methods.sql), after that feel free to contribute. The working branch is develop, the master branch is for releasing documentation on github with cross-refs, cross-refs implemented with shitty python script, I may share it after for someone to improve it.

## R5 S3 Squirrel methods, either global or undefined what type they correspond to.

TODO: 
* Mark SERVER / CLIENT / UI methods
* Type Info add nullability information? `ornull`


| Squirrel Name | Type Info | Comment |
| ------------- | --------- | ------- |
| Chroma_SetBaseLayer | int CHROMALOOP_anim, int CHROMATRANS_transition, table< float, vector > gradient, float transitionTime, float animRate = 1.0 | Sets the base layer animation for chroma hardware. gradient  maps values 0-1 to colors |
| Chroma_AddOverlay | int CHROMALOOP_anim, int CHROMAWAVE_alpha, table< float, vector > gradient, float duration, float animRate = 1.0 | Adds a temporary animated overlay on chroma hardware. gradient maps values 0-1 to colors |
| Chroma_AddPersistentOverlay | int CHROMALOOP_anim, int CHROMALOOP_alpha, int CHROMATRANS_transition, table< float, vector > gradient, float transitionTime, float animRate = 1.0, float alphaRate = 1.0 -> int | Adds an animated overlay on chroma hardware. Returns a handle to be passed into Chroma_RemovePersistentOverlay. gradient maps values 0-1 to colors |
| Chroma_RemovePersistentOverlay | int handle, int CHROMATRANS_transition, float transitionTime | Removes an animated overlay previously added with Chroma_AddPersistentOverlay |
| Chroma_SetPersistentOverlayAlpha | int handle, float alpha | Sets the overall opacity of a persistent chroma overlay |
| Dev_GetAISettingByKeyField | _possibly_ return type is an asset, may be bool, int etc... | Get AI setting key field |
| Dev_GetAISettingAssetByKeyField_Global | string settingsName, string | Slow dev ONLY. Given a player setting name and key, resolves a string key to its asset value in that setting info file |
| GetAIClass | () -> [AIClass](Consts/AIClass.md) | Gets the AI Class |
| GetAIClassName | () | Gets the AI Class |
| GetTitanSoulNetBool | string networkVariableName -> bool | Gets a bool network variable on the titan soul (see RegisterNetworkedVariable) |
| GetTitanSoulNetFloat | string networkVariableName -> float | Gets a float network variable on the titan soul (see RegisterNetworkedVariable) |
| GetTitanSoulNetInt | string networkVariableName -> int | Gets an int network variable on the titan soul (see RegisterNetworkedVariable) |
| GetTitanSoulNetTime | string networkVariableName -> float | Gets a time (float) network variable on the titan soul (see RegisterNetworkedVariable) |
| GetTitanSoulNetEnt | string networkVariableName -> _possibly_ entity | Gets an entity network variable on the titan soul (see RegisterNetworkedVariable) |
| GetTitan | () -> entity | Gets the titan for this titanSoul entity |
| HasValidTitan | () -> bool | Returns if the titanSoul has a valid titan |
| SetDecal | int decalIndex -> void | Sets the decalIndex |
| GetCurrentSequenceName | () -> _possibly_ string | Gets the name of the current sequence |
| Anim_GetAttachmentAtTime | string animName, string attachName, float time -> Attachment | Returns the position and angle of an attachment at the given time in the given animation |
| AnimSyncScriptProp_Begin | entity parentEntity, float startCycle, float endCycle, string windowName | Force sync the animation of the created anim prop entity with the parent entity |
| AnimSyncScriptProp_End | entity parentEntity |  |
| TraceToLocalPlayerSimple | () -> float | Get deferred trace fraction from eye to local player eye. Used on NPC's |
| TraceToLocalPlayer | () -> [TraceResults](Types/TraceResults.md) ornull | Get deferred trace result from eye to local player eye, return NULL if deferred trace is not available |
|  |  |  |

