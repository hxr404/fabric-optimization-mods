### Note: The incompatibilities listed are for the mods featured in this list only, and does not take into consideration any mods not featured here.

## Fabric API
Despite being a toolkit for modding functionality, Fabric API actually contains some optimizations and bugfixes. Even if you aren't planning to run any content mods, I recommend that you still use it. [Download it from GitHub](https://github.com/FabricMC/fabric).

## Rendering
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Sodium | A rendering engine replacement designed to boost your framerate and reduce random stuttering. | CaffeineMC | Mostly | No | Canvas | https://github.com/jellysquid3/sodium-fabric/ |
| Canvas | A shader-oriented rendering engine replacement. Focuses on functionality over raw performance. | Grondag | Yes | No | Sodium | https://github.com/grondag/canvas/ |
| Cull Leaves | A renderer tweak that implements leaf culling similar to OptiFine's. NOTE: This will negatively impact visuals! | TeamMidnightDust | Yes | No | None | https://github.com/TeamMidnightDust/CullLeaves/ |
| Entity Culling | A rendering tweak that implements asynchronous culling to entities. | tr7zw | No | No | None | https://github.com/tr7zw/EntityCulling-Fabric/ |
| Better Beds | Makes Minecraft use the built-in renderer for beds rather than the custom one, to improve rendering performance when around beds. | TeamMidnightDust | No | No | None | https://github.com/TeamMidnightDust/BetterBeds/ |
| Enhanced Block Entities | Makes chests (and soon to be more block entities) use baked block models rather than laggy entity models. But doesn't remove animations  | FoundationGames | --- | No | If using with Sodium requires Indium | https://github.com/FoundationGames/EnhancedBlockEntities |
| Fast Chest | Removes dynamic models from chests and makes them render as static chunk geometry. (This removes their lid opening animation) | FakeDomi | --- | No | --- | https://www.curseforge.com/minecraft/mc-mods/fastchest |
| Indium | Adaptation of Indigo (Reference implementation of the Fabric Rendering API) for use with Sodium | comp500 | --- | --- | Some Versions of Sodium | https://github.com/comp500/Indium |

## Server
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Lithium | A mod that optimizes some aspects of Minecraft's server, while maintaining behavior identical to vanilla. Works in singleplayer. | CaffeineMC | Yes | No | None | https://github.com/jellysquid3/lithium-fabric/ |
| Tic-TACS | A complete rewrite of Minecraft's Threaded Anvil Chunk Storage, or TACS. It allows to multithread chunk generation, and can also allow render distances above 32. | Gegy | No | Yes | None | https://github.com/Gegy/tic-tacs/releases |
| C2ME | A Fabric mod designed to improve the chunk performance of Minecraft | YatopiaMC | No | --- | --- | https://github.com/YatopiaMC/C2ME-fabric |
| Fast Furnace | --- | Tfarcenim | --- | No | --- | https://www.curseforge.com/minecraft/mc-mods/fast-furnace-for-fabric |
| HopperOptimizations | --- | 2No2Name | --- | No | Lithium ([compatible Fork](https://github.com/2No2Name/lithium-fabric) available) | https://github.com/2No2Name/hopperOptimizations |

## Lighting
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Phosphor | A smaller mod that makes Minecraft's bulky and slow lighting engine much faster. | Jellysquid | Yes | No | Starlight | https://github.com/jellysquid3/phosphor-fabric |
| Starlight | An experimental mod that can speed up lighting calculations by 26x compared to Phosphor (according to the developer). | Spottedleaf | Mostly | No | Phosphor | https://github.com/Spottedleaf/Starlight/ |

## Memory
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Hydrogen | Reduces RAM usage of Minecraft by compacting models and other misc. data. More effective with more content mods. | CaffeineMC | Yes | No | None | https://github.com/jellysquid3/hydrogen-fabric/ |
| FerriteCore | Reduces RAM usage in a few different ways | malte0811 | --- | --- | Technically compatible with Hydrogen, but a couple (not all) of Hydrogen's mixins are disabled. | https://github.com/malte0811/FerriteCore |

## Network
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Krypton | Optimizations for Minecraft's general networking. If you're at a bandwidth bottleneck then this can help. | astei | Somewhat | No | None | https://github.com/astei/krypton |

## Start-up
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Cadmium | Loader for Jellysquid's optimized fork of Mojang's DataFixerUpper. Speeds up game loading. LucilleTea's port is required for 1.16.x. | Jellysquid, LucilleTea (port) | No | Yes | None | https://github.com/jellysquid3/cadmium-fabric/, https://github.com/LucilleTea/cadmium-fabric/ |
| LazyDFU | Prevents DFU from being built until it is needed. Compatible with Cadmium and I highly recommend using these two together. | astei | Yes | No | None | https://github.com/astei/lazydfu/ |
| Smooth Boot | Tweaks for Minecraft's bootstrap process, prevents Minecraft from eating your CPU on low end systems and allows for faster boots on high end systems. | UltimateBoomer | Mostly | No (only active on start-up) | None | https://www.curseforge.com/minecraft/mc-mods/smooth-boot |
| DashLoader | caches the modelmanager while accelerating the other components of the client initialization stack | alphaqu | No | Yes | EnhancedBlockEntities, SmoothBoot, Other | https://github.com/alphaqu/DashLoader |

## Other
### Theses are some random mods that I've found.
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Fabric Carpet, Carpet TIS Addition, Carpet Addons | `lagFreeSpawning`, `lightEngineMaxBatchSize`, `maxEntityCollisions`, `optimizedTNT`, `combineXPOrbs` (is implemented invanilla 1.17 snapshots) TIS Addition: `optimizedFastEntityMovement`, `optimizedHardHitBoxEntityCollision`, `optimizedTNTHighPriority` Carpet Addons by wholmT: `projectileRaycastLength` | gnembon, TISUnion, whoImT | --- | No | --- | https://github.com/gnembon/fabric-carpet https://github.com/TISUnion/Carpet-TIS-Addition https://github.com/whoImT/carpet-addons |
| FTL-TNT from johan-carpet | A fork of [johan-carpet](https://github.com/JohanVonElectrum/Johan-Carpet) wich contains only the FTL-TNT rule (TNT optimized for large amounts in Cannons) | DragonEggBedrockBreaking | --- | No | --- | https://github.com/DragonEggBedrockBreaking/FTL-TNT |
| Fabric Zero (Discontinued) | Compability enhancement mod and can slightly improve performance | Fox2Code | Yes | No | None | https://www.curseforge.com/minecraft/mc-mods/fabric-zero |
| FoamFix (outdated) | Outdated do not use | asiekierka | --- | --- | Recent Minecraft Versions | https://www.curseforge.com/minecraft/mc-mods/foamfix-optimization-mod |
| VanillaFix | --- | Dimensional Development | --- | No | --- | https://github.com/DimensionalDevelopment/VanillaFix/tree/1.16 |


## Extra Utility
### Note: These mods are extras that do not improve game performance.
| Name | Description | Developer | Stable | Dangerous | Incompatibilities | Link |
| --- | --- | --- | --- | --- | --- | --- |
| Sodium Extra Fabric (Requires Sodium) | Adds more graphical settings to Sodium, similar to OptiFine's. | FlashyReese | No | No | Canvas | https://github.com/FlashyReese/sodium-extra-fabric/ |
| Dynamic FPS | Slows down Minecraft's rendering when Minecraft is minimized or in the background to improve performance in other applications. | juliand665 | Yes | No | None | https://github.com/juliand665/Dynamic-FPS/ |
| NoFade | Removes long transition animation when you load into Minecraft | UltimateBoomer | Yes | No | None | https://www.curseforge.com/minecraft/mc-mods/no-fade |
| SmoothScrollingEverywhere | Adds smooth scrolling to every vanilla list and the ability the bounce back when overscroll. | shedaniel | No | No | None | https://www.curseforge.com/minecraft/mc-mods/smooth-scrolling-everywhere-fabric |
| Spark | CPU Profiler, Memory Inspection & Server Health Reporting | lucko | Yes | No | None | https://github.com/lucko/spark |
| Item Model Fix | Fixes Item Stitching | Pepper_Bell | Yes | No | --- | https://github.com/PepperCode1/Item-Model-Fix |
