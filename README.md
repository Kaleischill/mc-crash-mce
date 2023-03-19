# mc-crash-mce---- Minecraft Crash Report ----
// Uh... Did I do that?

Time: 2023-03-19 15:54:03 CDT
Description: Initializing game

net.minecraftforge.fml.common.LoaderException: thebetweenlands Failed to load new mod instance.
    at net.minecraftforge.fml.common.FMLModContainer.constructMod(FMLModContainer.java:604)
    at sun.reflect.GeneratedMethodAccessor11.invoke(Unknown Source)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.sendEventToModContainer(LoadController.java:219)
    at net.minecraftforge.fml.common.LoadController.propogateStateMessage(LoadController.java:197)
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.distributeStateMessage(LoadController.java:136)
    at net.minecraftforge.fml.common.Loader.loadMods(Loader.java:595)
    at net.minecraftforge.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:232)
    at net.minecraft.client.Minecraft.init(Minecraft.java:467)
    at net.minecraft.client.Minecraft.run(Minecraft.java:3931)
    at net.minecraft.client.main.Main.main(SourceFile:123)
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
    at net.minecraft.launchwrapper.Launch.main(Launch.java:28)
Caused by: java.lang.reflect.InvocationTargetException
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:498)
    at net.minecraftforge.fml.common.ILanguageAdapter$JavaAdapter.getNewInstance(ILanguageAdapter.java:187)
    at net.minecraftforge.fml.common.FMLModContainer.constructMod(FMLModContainer.java:599)
    ... 35 more
Caused by: java.lang.NoClassDefFoundError: thebetweenlands/core/TheBetweenlandsPreconditions
    at thebetweenlands.common.TheBetweenlands.createInstance(TheBetweenlands.java:164)
    ... 41 more
Caused by: java.lang.ClassNotFoundException: thebetweenlands.core.TheBetweenlandsPreconditions
    at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:191)
    at java.lang.ClassLoader.loadClass(ClassLoader.java:418)
    at java.lang.ClassLoader.loadClass(ClassLoader.java:351)
    ... 42 more
Caused by: java.lang.NullPointerException


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
  Minecraft Version: 1.12.2
  Operating System: Windows 10 (amd64) version 10.0
  Java Version: 1.8.0_312, Temurin
  Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Temurin
  Memory: 1213968992 bytes (1157 MB) / 2818572288 bytes (2688 MB) up to 13086228480 bytes (12480 MB)
  JVM Flags: 8 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx12480M -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
  IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
  FML: MCP 9.42 Powered by Forge 14.23.5.2860 382 mods loaded, 380 mods active
       States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
       
       | State | ID                                | Version                  | Source                                                      | Signature                                |
       |:----- |:--------------------------------- |:------------------------ |:----------------------------------------------------------- |:---------------------------------------- |
       | LC    | minecraft                         | 1.12.2                   | minecraft.jar                                               | None                                     |
       | LC    | mcp                               | 9.42                     | minecraft.jar                                               | None                                     |
       | LC    | FML                               | 8.0.99.99                | forge-1.12.2-14.23.5.2860.jar                               | e3c3d50c7c986df74c645c0ac54639741c90a557 |
       | LC    | forge                             | 14.23.5.2860             | forge-1.12.2-14.23.5.2860.jar                               | e3c3d50c7c986df74c645c0ac54639741c90a557 |
       | LC    | advancedrocketrycore              | 1                        | minecraft.jar                                               | None                                     |
       | LC    | ColorUtility                      | 1.0.4                    | minecraft.jar                                               | None                                     |
       | LC    | creativecoredummy                 | 1.0.0                    | minecraft.jar                                               | None                                     |
       | LC    | ivtoolkit                         | 1.3.3-1.12               | minecraft.jar                                               | None                                     |
       | LC    | littletilescore                   | 1.0.0                    | minecraft.jar                                               | None                                     |
       | LC    | reachfix                          | 1.0.5                    | minecraft.jar                                               | None                                     |
       | LC    | mixinbooter                       | 5.0                      | minecraft.jar                                               | None                                     |
       | LC    | openmodscore                      | 0.12.2                   | minecraft.jar                                               | None                                     |
       | LC    | foamfixcore                       | 7.7.4                    | minecraft.jar                                               | None                                     |
       | LC    | obfuscate                         | 0.4.2                    | minecraft.jar                                               | None                                     |
       | LC    | opencomputers|core                | 1.7.5.192                | minecraft.jar                                               | None                                     |
       | LC    | randompatches                     | 1.12.2-1.22.1.10         | randompatches-1.12.2-1.22.1.10.jar                          | None                                     |
       | LC    | tweakersconstruct                 | 1.12.2-1.6.0             | tweakersconstruct-1.12.2-1.6.0.jar                          | None                                     |
       | LC    | fastbench                         | 1.7.3                    | FastWorkbench-1.12.2-1.7.3.jar                              | None                                     |
       | LC    | actuallyadditions                 | 1.12.2-r152              | ActuallyAdditions-1.12.2-r152.jar                           | None                                     |
       | LC    | forgeendertech                    | 1.12.2-4.5.5.0           | ForgeEndertech-1.12.2-4.5.5.0-build.0561.jar                | None                                     |
       | LC    | adhooks                           | 1.12.2-3.3.0.0           | AdHooks-1.12.2-3.3.0.0-build.0528.jar                       | None                                     |
       | LC    | adlods                            | 1.12.2-1.0.8.0           | AdLods-1.12.2-1.0.8.0-build.0504.jar                        | None                                     |
       | LC    | redstoneflux                      | 2.1.1                    | RedstoneFlux-1.12-2.1.1.1-universal.jar                     | None                                     |
       | LC    | cofhcore                          | 4.6.6                    | CoFHCore-1.12.2-4.6.6.1-universal.jar                       | None                                     |
       | LC    | libvulpes                         | 0.4.2.-75                | LibVulpes-1.12.2-0.4.2-75-universal.jar                     | None                                     |
       | LC    | advancedrocketry                  | 1.7.0.-232               | AdvancedRocketry-1.12.2-1.7.0-232-universal.jar             | None                                     |
       | LC    | ctm                               | MC1.12.2-1.0.2.31        | CTM-MC1.12.2-1.0.2.31.jar                                   | None                                     |
       | LC    | appliedenergistics2               | rv6-stable-7             | appliedenergistics2-rv6-stable-7.jar                        | dfa4d3ac143316c6f32aa1a1beda1e34d42132e5 |
       | LC    | bdlib                             | 1.14.3.12                | bdlib-1.14.3.12-mc1.12.2.jar                                | None                                     |
       | LC    | ae2stuff                          | 0.7.0.4                  | ae2stuff-0.7.0.4-mc1.12.2.jar                               | None                                     |
       | LC    | baubles                           | 1.5.2                    | Baubles-1.12-1.5.2.jar                                      | None                                     |
       | LC    | mysticalworld                     | 1.12.2-1.11.0            | mysticalworld-1.12.2-1.11.0.jar                             | None                                     |
       | LC    | endercore                         | 1.12.2-0.5.76            | EnderCore-1.12.2-0.5.76.jar                                 | None                                     |
       | LC    | crafttweaker                      | 4.1.20                   | CraftTweaker2-1.12-4.1.20.679.jar                           | None                                     |
       | LC    | mtlib                             | 3.0.6                    | MTLib-3.0.6.jar                                             | None                                     |
       | LC    | modtweaker                        | 4.0.18                   | modtweaker-4.0.18.jar                                       | None                                     |
       | LC    | jei                               | 4.16.1.301               | jei_1.12.2-4.16.1.301.jar                                   | None                                     |
       | LC    | thaumcraft                        | 6.1.BETA26               | Thaumcraft-1.12.2-6.1.BETA26.jar                            | None                                     |
       | LC    | codechickenlib                    | 3.2.3.358                | CodeChickenLib-1.12.2-3.2.3.358-universal.jar               | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LC    | cofhworld                         | 1.4.0                    | CoFHWorld-1.12.2-1.4.0.1-universal.jar                      | None                                     |
       | LC    | thermalfoundation                 | 2.6.7                    | ThermalFoundation-1.12.2-2.6.7.1-universal.jar              | None                                     |
       | LC    | thermalexpansion                  | 5.5.7                    | ThermalExpansion-1.12.2-5.5.7.1-universal.jar               | None                                     |
       | LC    | enderio                           | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | mantle                            | 1.12-1.3.3.55            | Mantle-1.12-1.3.3.55.jar                                    | None                                     |
       | LC    | chisel                            | MC1.12.2-1.0.2.45        | Chisel-MC1.12.2-1.0.2.45.jar                                | None                                     |
       | LC    | enderiointegrationtic             | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | tombstone                         | 4.1.2                    | tombstone-4.1.2-1.12.2.jar                                  | None                                     |
       | LC    | quark                             | r1.6-179                 | Quark-r1.6-179.jar                                          | None                                     |
       | LC    | twilightforest                    | 3.11.1021                | twilightforest-1.12.2-3.11.1021-universal.jar               | None                                     |
       | LC    | tconstruct                        | 1.12.2-2.13.0.183        | TConstruct-1.12.2-2.13.0.183.jar                            | None                                     |
       | LC    | p455w0rdslib                      | 2.3.161                  | p455w0rdslib-1.12.2-2.3.161.jar                             | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | ae2wtlib                          | 1.0.34                   | AE2WTLib-1.12.2-1.0.34.jar                                  | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | infinitylib                       | 1.12.2-1.12.0            | infinitylib-1.12.0.jar                                      | None                                     |
       | LC    | agricraft                         | 2.12.0-1.12.0-a6         | AgriCraft-2.12.0-1.12.0-a6.jar                              | None                                     |
       | LC    | aiimprovements                    | 0.0.1.3                  | AIImprovements-1.12-0.0.1b3.jar                             | None                                     |
       | LC    | aireducer                         | 0.3.0                    | AIReducer-1.12.2-0.3.0.jar                                  | None                                     |
       | LC    | akashictome                       | 1.2-12                   | AkashicTome-1.2-12.jar                                      | None                                     |
       | LC    | creativecore                      | 1.10.0                   | CreativeCore_v1.10.70_mc1.12.2.jar                          | None                                     |
       | LC    | ambientsounds                     | 3.0                      | AmbientSounds_v3.1.5_mc1.12.2.jar                           | None                                     |
       | LC    | ancientbeasts                     | 1.9.99999                | ancientbeasts-1.9.99999.jar                                 | None                                     |
       | LC    | applecore                         | 3.4.0                    | AppleCore-mc1.12.2-3.4.0.jar                                | None                                     |
       | LC    | appleskin                         | 1.0.14                   | AppleSkin-mc1.12-1.0.14.jar                                 | None                                     |
       | LC    | architecturecraft                 | @VERSION@                | architecturecraft-1.12-3.98.jar                             | None                                     |
       | LC    | conarm                            | 1.2.5.10                 | conarm-1.12.2-1.2.5.10.jar                                  | b33d2c8df492beff56d1bbbc92da49b8ab7345a1 |
       | LC    | armoryexpansion                   | 1.4.2                    | armoryexpansion-1.4.2.jar                                   | None                                     |
       | LC    | armoryexpansion-custommaterials   | 1.4.2                    | armoryexpansion-1.4.2.jar                                   | None                                     |
       | LC    | hammercore                        | 2.0.6.32                 | HammerLib-1.12.2-2.0.6.32.jar                               | 9f5e2a811a8332a842b34f6967b7db0ac4f24856 |
       | LC    | thaumadditions                    | 12.7.8                   | ThaumicAdditions-1.12.2-12.7.8.jar                          | 9f5e2a811a8332a842b34f6967b7db0ac4f24856 |
       | LC    | llibrary                          | 1.7.20                   | llibrary-1.7.20-1.12.2.jar                                  | b9f30a813bee3b9dd5652c460310cfcd54f6b7ec |
       | LC    | iceandfire                        | 1.9.1                    | iceandfire-1.9.1-1.12.2.jar                                 | None                                     |
       | LC    | armoryexpansion-iceandfire        | 1.4.2                    | armoryexpansion-1.4.2.jar                                   | None                                     |
       | LC    | armoryexpansion-matteroverdrive   | 1.4.2                    | armoryexpansion-1.4.2.jar                                   | None                                     |
       | LC    | artifacts                         | 1.12.2-1.2.3             | Artifacts-1.12.2-1.2.3.jar                                  | None                                     |
       | LC    | astralsorcery                     | 1.10.27                  | astralsorcery-1.12.2-1.10.27.jar                            | a0f0b759d895c15ceb3e3bcb5f3c2db7c582edf0 |
       | LC    | attributefix                      | 1.0.4                    | AttributeFix-1.12.2-1.0.4.jar                               | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | atum                              | 2.0.20                   | Atum-1.12.2-2.0.20.jar                                      | None                                     |
       | LC    | mdecore                           | 1.12-1.1                 | mdecore-1.12-1.1.jar                                        | None                                     |
       | LC    | autooredictconv                   | 1.12-1.0.1               | autooredictconv-1.12-1.0.1.jar                              | None                                     |
       | LC    | autoreglib                        | 1.3-32                   | AutoRegLib-1.3-32.jar                                       | None                                     |
       | LC    | badwithernocookiereloaded         | 1.12.2-3.4.18            | badwithernocookiereloaded-1.12.2-3.4.18.jar                 | None                                     |
       | LC    | battletowers                      | 1.6.5                    | BattleTowers-1.12.2.jar                                     | None                                     |
       | LC    | betterbuilderswands               | 0.13.2                   | BetterBuildersWands-1.12.2-0.13.2.271+5997513.jar           | None                                     |
       | LC    | bettercaves                       | 1.12.2                   | bettercaves-1.12.2-2.0.4.jar                                | None                                     |
       | LC    | botania                           | r1.10-363                | Botania r1.10-363.jar                                       | None                                     |
       | LC    | mowziesmobs                       | 1.5.8                    | mowziesmobs-1.5.8.jar                                       | None                                     |
       | LC    | patchouli                         | 1.0-23.6                 | Patchouli-1.0-23.6.jar                                      | None                                     |
       | LC    | bewitchment                       | 0.22.63                  | bewitchment-1.12.2-0.0.22.64.jar                            | None                                     |
       | LC    | bibliocraft                       | 2.4.6                    | BiblioCraft[v2.4.6][MC1.12.2].jar                           | None                                     |
       | LC    | biomeinfo                         | v1.2.5                   | biomeinfo-1.12.2-v1.2.5.jar                                 | None                                     |
       | LC    | biomesoplenty                     | 7.0.1.2441               | BiomesOPlenty-1.12.2-7.0.1.2441-universal.jar               | None                                     |
       | LC    | biomestaff                        | 1.0.0                    | BiomeStaff-1.12.2-1.0.0.jar                                 | None                                     |
       | LC    | blockdrops                        | 1.4.0                    | blockdrops-1.12.2-1.4.0.jar                                 | None                                     |
       | LC    | cyclicmagic                       | 1.20.8                   | Cyclic-1.12.2-1.20.8.jar                                    | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
       | LC    | guideapi                          | 1.12-2.1.8-63            | Guide-API-1.12-2.1.8-63.jar                                 | None                                     |
       | LC    | bloodmagic                        | 1.12.2-2.4.3-105         | BloodMagic-1.12.2-2.4.3-105.jar                             | None                                     |
       | LC    | bookshelf                         | 2.3.590                  | Bookshelf-1.12.2-2.3.590.jar                                | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | bountifulbaubles                  | 0.0.1                    | Bountiful Baubles-1.12.2-0.1.6.jar                          | None                                     |
       | LC    | forgelin                          | 1.8.4                    | Forgelin-1.8.4.jar                                          | None                                     |
       | LC    | bountiful                         | 2.2.2                    | Bountiful-2.2.2.jar                                         | None                                     |
       | LC    | brokenwings                       | 2.0.0                    | brokenwings-3.0.0.jar                                       | None                                     |
       | LC    | buildcraftlib                     | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftcore                    | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftbuilders                | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcrafttransport               | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftsilicon                 | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftenergy                  | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | reborncore                        | 3.19.5                   | RebornCore-FORK-1.12.2-3.19.5-universal.jar                 | None                                     |
       | LC    | techreborn                        | 2.27.3.1084              | TechReborn-1.12.2-2.27.3.1084-universal.jar                 | 8727a3141c8ec7f173b87aa78b9b9807867c4e6b |
       | LC    | forestry                          | 5.8.2.422                | forestry_1.12.2-5.8.2.422.jar                               | None                                     |
       | LC    | buildcraftcompat                  | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftfactory                 | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildcraftrobotics                | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                                | None                                     |
       | LC    | buildinggadgets                   | 2.8.4                    | BuildingGadgets-2.8.4.jar                                   | None                                     |
       | LC    | capsule                           | 1.12.2-3.3.11            | Capsule-1.12.2-3.3.11.jar                                   | None                                     |
       | LC    | careerbees                        | 1.0                      | careerbees-0.4.0.jar                                        | None                                     |
       | LC    | chameleon                         | 1.12-4.1.3               | Chameleon-1.12-4.1.3.jar                                    | None                                     |
       | LC    | champions                         | 1.12.2-1.0.11.10         | champions-1.12.2-1.0.11.10.jar                              | b33d2c8df492beff56d1bbbc92da49b8ab7345a1 |
       | LC    | chancecubes                       | 1.12.2-5.0.2.385         | ChanceCubes-1.12.2-5.0.2.385.jar                            | None                                     |
       | LC    | charm                             | 1.4                      | Charm-1.12.2-1.4.1.jar                                      | None                                     |
       | LC    | cherishedworlds                   | 1.12.2-1.0.1             | cherishedworlds-1.12.2-1.0.1.jar                            | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
       | LC    | chiselsandbits                    | 14.33                    | chiselsandbits-14.33.jar                                    | None                                     |
       | LC    | neid                              | 1.5.4.4                  | NotEnoughIDs-1.5.4.4.jar                                    | None                                     |
       | LC    | phosphor-lighting                 | 1.12.2-0.2.6             | phosphor-1.12.2-0.2.6+build50-universal.jar                 | f0387d288626cc2d937daa504e74af570c52a2f1 |
       | LC    | cqrepoured                        | 2.6.12B                  | Chocolate_Quest_Repoured-1.12.2-2.6.12B.jar                 | None                                     |
       | LC    | chunkpregenerator                 | 2.5.0                    | Chunk Pregenerator-V1.12-2.5.0.jar                          | None                                     |
       | LC    | clumps                            | 3.1.2                    | Clumps-3.1.2.jar                                            | None                                     |
       | LC    | collective                        | 2.25                     | collective-1.12.2-2.25.jar                                  | None                                     |
       | LC    | cyclopscore                       | 1.6.7                    | CyclopsCore-1.12.2-1.6.7.jar                                | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LC    | commoncapabilities                | 2.4.8                    | CommonCapabilities-1.12.2-2.4.8.jar                         | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LC    | compactmachines3                  | 3.0.18                   | compactmachines3-1.12.2-3.0.18-b278.jar                     | None                                     |
       | LC    | controlling                       | 3.0.10                   | Controlling-3.0.10.jar                                      | None                                     |
       | LC    | cookingforblockheads              | 6.5.0                    | CookingForBlockheads_1.12.2-6.5.0.jar                       | None                                     |
       | LC    | cosmeticarmorreworked             | 1.12.2-v5a               | CosmeticArmorReworked-1.12.2-v5a.jar                        | aaaf83332a11df02406e9f266b1b65c1306f0f76 |
       | LC    | craftingtweaks                    | 8.1.9                    | CraftingTweaks_1.12.2-8.1.9.jar                             | None                                     |
       | LC    | ctgui                             | 1.0.0                    | CraftTweaker2-1.12-4.1.20.679.jar                           | None                                     |
       | LC    | crafttweakerjei                   | 2.0.3                    | CraftTweaker2-1.12-4.1.20.679.jar                           | None                                     |
       | LC    | crimsonwarfare                    | 1.5                      | crimsonwarfare-1.5.jar                                      | None                                     |
       | LC    | cucumber                          | 1.1.3                    | Cucumber-1.12.2-1.1.3.jar                                   | None                                     |
       | LC    | culinaryconstruct                 | 1.3.4                    | culinaryconstruct-1.3.4.jar                                 | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
       | LC    | customizeddungeonloot             | 1.0.3                    | Customized-Dungeon-Loot-1.12 -(v.1.0.3).jar                 | None                                     |
       | LC    | custommainmenu                    | 2.0.9.1                  | CustomMainMenu-MC1.12.2-2.0.9.1.jar                         | None                                     |
       | LC    | waila                             | 1.8.26                   | Hwyla-1.8.26-B41_1.12.2.jar                                 | None                                     |
       | LC    | stg                               | 1.12.2-1.2.3             | stg-1.12.2-1.2.3.jar                                        | None                                     |
       | LC    | mousetweaks                       | 2.10                     | MouseTweaks-2.10-mc1.12.2.jar                               | None                                     |
       | LC    | danknull                          | 1.7.101                  | DankNull-1.12.2-1.7.101.jar                                 | 644f38521a349310a5dae0239577dc7beebefaec |
       | LC    | darknesslib                       | 1.1.0                    | DarknessLib-1.12.2-1.1.0.jar                                | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LC    | dimdoors                          | 3.0.10                   | DimensionalDoors-1.12.2-3.0.12.jar                          | None                                     |
       | LC    | ding                              | 1.0.2                    | Ding-1.12.2-1.0.2.jar                                       | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LC    | discordcraft                      | 1.0                      | DiscordCraft-2.0.jar                                        | None                                     |
       | LC    | doggytalents                      | 1.15.1.6                 | DoggyTalents-1.12.2-1.15.1.6.jar                            | None                                     |
       | LC    | dungeonsmod                       | 1.12.2-1.0.6             | DungeonsMod-1.12.2-1.0.6.jar                                | None                                     |
       | LC    | dungeontactics                    | DT-0.16.9                | DungeonTactics-1.12.2-0.16.9.jar                            | None                                     |
       | LC    | eerieentities                     | 1.0.7                    | EerieEntities-1.12.2-1.0.7.jar                              | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | ebwizardry                        | 4.3.7                    | ElectroblobsWizardry-4.3.8.jar                              | None                                     |
       | LC    | elenaidodge2                      | 1.0.8b                   | ElenaiDodge2-1.12.2-1.0.8b.jar                              | None                                     |
       | LC    | enchdesc                          | 1.1.15                   | EnchantmentDescriptions-1.12.2-1.1.15.jar                   | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | enderiobase                       | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderioconduits                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderioconduitsappliedenergistics | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | opencomputers                     | 1.7.5.192                | OpenComputers-MC1.12.2-1.7.5.192.jar                        | None                                     |
       | LC    | enderioconduitsopencomputers      | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderioconduitsrefinedstorage     | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderiointegrationforestry        | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderiointegrationticlate         | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderioinvpanel                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | ftblib                            | 5.4.7.2                  | FTBLib-5.4.7.2.jar                                          | None                                     |
       | LC    | enderiomachines                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | enderiopowertools                 | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                                   | None                                     |
       | LC    | mcmultipart                       | 2.5.3                    | MCMultiPart-2.5.3.jar                                       | None                                     |
       | LC    | mekanism                          | 1.12.2-9.8.3.390         | Mekanism-1.12.2-9.8.3.390.jar                               | None                                     |
       | LC    | gasconduits                       | 5.3.70                   | EnderIO-conduits-mekanism-1.12.2-5.3.70.jar                 | None                                     |
       | LC    | enderstorage                      | 2.4.6.137                | EnderStorage-1.12.2-2.4.6.137-universal.jar                 | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LC    | energyconverters                  | 1.3.7.30                 | energyconverters_1.12.2-1.3.7.30.jar                        | None                                     |
       | LC    | erebus                            | 1.0.32                   | Erebus-1.0.32.jar                                           | None                                     |
       | LC    | erebusfix                         | 1.12.2-0.0.0.1           | erebusfix-1.12.2-0.0.0.1.jar                                | None                                     |
       | LC    | extrabitmanipulation              | 1.12.2-3.4.1             | ExtraBitManipulation-1.12.2-3.4.1.jar                       | None                                     |
       | LC    | extracells                        | 2.6.5                    | ExtraCells-1.12.2-2.6.5.jar                                 | None                                     |
       | LC    | extrautils2                       | 1.0                      | extrautils2-1.12-1.9.9.jar                                  | None                                     |
       | LC    | fairylights                       | 2.1.10                   | fairylights-2.2.0-1.12.2.jar                                | None                                     |
       | LC    | farmingforblockheads              | 3.1.28                   | FarmingForBlockheads_1.12.2-3.1.28.jar                      | None                                     |
       | LC    | mod_lavacow                       | 1.3.3                    | Fish's Undead Rising-1.3.3.jar                              | None                                     |
       | LC    | sonarcore                         | 5.0.19                   | sonarcore-1.12.2-5.0.19-20.jar                              | None                                     |
       | LC    | fluxnetworks                      | 4.1.0                    | FluxNetworks-1.12.2-4.1.1.34.jar                            | None                                     |
       | LC    | foamfix                           | 0.10.14-1.12.2           | foamfix-0.10.14-1.12.2.jar                                  | None                                     |
       | LC    | forgemultipartcbe                 | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar                | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LC    | microblockcbe                     | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar                | None                                     |
       | LC    | minecraftmultipartcbe             | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar                | None                                     |
       | LC    | fossil                            | 8.0.5                    | fossilsarcheology-8.0.6.jar                                 | None                                     |
       | LC    | iceologer                         | 1.5                      | Frozen-Fiend-1.5.jar                                        | None                                     |
       | LC    | ftbbackups                        | 1.1.0.1                  | FTBBackups-1.1.0.1.jar                                      | None                                     |
       | LC    | ftbutilities                      | 5.4.1.131                | FTBUtilities-5.4.1.131.jar                                  | None                                     |
       | LC    | itemfilters                       | 1.0.4.2                  | ItemFilters-1.0.4.2.jar                                     | None                                     |
       | LC    | reskillable                       | 1.12.2-1.13.0            | Reskillable-1.12.2-1.13.0.jar                               | None                                     |
       | LC    | ftbquests                         | 1202.9.0.15              | FTBQuests-1202.9.0.15.jar                                   | None                                     |
       | LC    | ftbmoney                          | 1.2.0.47                 | FTBMoney-1.2.0.47.jar                                       | None                                     |
       | LC    | futuremc                          | 0.2.6                    | future-mc-0.2.11.jar                                        | None                                     |
       | LC    | geckolib3                         | 3.0.30                   | geckolib-forge-1.12.2-3.0.31.jar                            | None                                     |
       | LC    | gendustry                         | 1.6.5.8                  | gendustry-1.6.5.8-mc1.12.2.jar                              | None                                     |
       | LC    | ghostsexplosives                  | 2.3.0 - MC 1.12.2        | Ghost's Explosives 2.3.0 - MC1.12.2.jar                     | None                                     |
       | LC    | gottschcore                       | 1.15.0                   | GottschCore-mc1.12.2-f14.23.5.2859-v1.15.0.jar              | None                                     |
       | LC    | grue                              | 1.8.0                    | Grue-1.12.2-1.8.0.jar                                       | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LC    | guardillagers                     | 1.0.1                    | guardillagers-1.12.2-1.0.1.jar                              | None                                     |
       | LC    | gunpowderlib                      | 1.12.2-1.1               | GunpowderLib-1.12.2-1.1.jar                                 | 4ffa87db52cf086d00ecc4853a929367b1c39b5c |
       | LC    | hardcoredarkness                  | 2.0                      | HardcoreDarkness-MC1.12.2-2.0.jar                           | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LC    | ichunutil                         | 7.2.2                    | iChunUtil-1.12.2-7.2.2.jar                                  | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LC    | hats                              | 7.1.1                    | Hats-1.12.2-7.1.1.jar                                       | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LC    | hunterillager                     | 1.2                      | hunterillager-1.12.2-1.2.jar                                | None                                     |
       | LC    | icbmclassic                       | 1.12.2-4.0.1.75          | ICBM-classic-1.12.2-4.0.1b75.jar                            | None                                     |
       | LC    | illagers_plus                     | 1.1                      | IllagersPlus-1.12.2-1.1.3.jar                               | None                                     |
       | LC    | immersiveengineering              | 0.12-98                  | ImmersiveEngineering-0.12-98.jar                            | None                                     |
       | LC    | immersivecables                   | 1.3.2                    | ImmersiveCables-1.12.2-1.3.2.jar                            | None                                     |
       | LC    | immersivepetroleum                | 1.1.9                    | immersivepetroleum-1.12.2-1.1.9.jar                         | None                                     |
       | LC    | immersiveposts                    | 0.2.1                    | ImmersivePosts-0.2.1.jar                                    | 0ba8738eadcf158e7fe1452255a73a022fb15feb |
       | LC    | improvedbackpacks                 | 1.12.2-1.5.0.0           | ImprovedBackpacks-1.12.2-1.5.0.0.jar                        | None                                     |
       | LC    | incontrol                         | 3.9.18                   | incontrol-1.12-3.9.18.jar                                   | None                                     |
       | LC    | teslacorelib                      | 1.0.17                   | tesla-core-lib-1.12.2-1.0.17.jar                            | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | industrialforegoing               | 1.12.2-1.12.2            | industrialforegoing-1.12.2-1.12.13-237.jar                  | None                                     |
       | LC    | instantunify                      | 1.1.2                    | instantunify-1.12.2-1.1.2.jar                               | None                                     |
       | LC    | instrumentalmobs                  | 1.2                      | Instrumental-Mobs-1.2.1.jar                                 | None                                     |
       | LC    | integrateddynamics                | 1.1.11                   | IntegratedDynamics-1.12.2-1.1.11.jar                        | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LC    | integrateddynamicscompat          | 1.0.0                    | IntegratedDynamics-1.12.2-1.1.11.jar                        | None                                     |
       | LC    | integratedtunnels                 | 1.6.14                   | IntegratedTunnels-1.12.2-1.6.14.jar                         | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LC    | integratedtunnelscompat           | 1.0.0                    | IntegratedTunnels-1.12.2-1.6.14.jar                         | None                                     |
       | LC    | mysticalagriculture               | 1.7.5                    | MysticalAgriculture-1.12.2-1.7.5.jar                        | None                                     |
       | LC    | mysticalagradditions              | 1.3.2                    | MysticalAgradditions-1.12.2-1.3.2.jar                       | None                                     |
       | LC    | nuclearcraft                      | 2.18zzz                  | NuclearCraft-2.18zzz-1.12.2.jar                             | None                                     |
       | LC    | harvestcraft                      | 1.12.2zb                 | Pam's HarvestCraft 1.12.2zg.jar                             | None                                     |
       | LC    | randomthings                      | 4.2.7.4                  | RandomThings-MC1.12.2-4.2.7.4.jar                           | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LC    | mcjtylib_ng                       | 3.5.4                    | mcjtylib-1.12-3.5.4.jar                                     | None                                     |
       | LC    | rftools                           | 7.73                     | rftools-1.12-7.73.jar                                       | None                                     |
       | LC    | integrationforegoing              | 1.12.2-1.11              | IntegrationForegoing-1.12.2-1.11.jar                        | 4ffa87db52cf086d00ecc4853a929367b1c39b5c |
       | LC    | inventorypets                     | 2.0.12                   | inventorypets-1.12-2.0.12.jar                               | None                                     |
       | LC    | inventorytweaks                   | 1.63+release.109.220f184 | InventoryTweaks-1.63.jar                                    | 55d2cd4f5f0961410bf7b91ef6c6bf00a766dcbe |
       | LC    | ironchest                         | 1.12.2-7.0.67.844        | ironchest-1.12.2-7.0.72.847.jar                             | None                                     |
       | LC    | itlt                              | 1.0.3                    | itlt-1.12.2-1.0.3.jar                                       | None                                     |
       | LC    | jaopca                            | 1.12.2-2.2.8.103         | JAOPCA-1.12.2-2.2.8.103.jar                                 | None                                     |
       | LC    | oredictinit                       | 1.12.2-2.2.1.71          | JAOPCA-1.12.2-2.2.8.103.jar                                 | None                                     |
       | LC    | jeibees                           | 0.9.0.5                  | jeibees-0.9.0.5-mc1.12.2.jar                                | None                                     |
       | LC    | journeymap                        | 1.12.2-5.7.1             | journeymap-1.12.2-5.7.1.jar                                 | None                                     |
       | LC    | jehc                              | 1.7.2                    | just-enough-harvestcraft-1.12.2-1.7.2.jar                   | None                                     |
       | LC    | jecalculation                     | 1.12.2-3.2.5             | JustEnoughCalculation-1.12.2-3.2.5.jar                      | None                                     |
       | LC    | jee                               | 1.0.8                    | JustEnoughEnergistics-1.12.2-1.0.8.jar                      | None                                     |
       | LC    | loottweaker                       | 0.3.1                    | LootTweaker-0.3.1+MC1.12.2.jar                              | None                                     |
       | LC    | jeresources                       | 0.9.2.60                 | JustEnoughResources-1.12.2-0.9.2.60.jar                     | None                                     |
       | LC    | laggoggles                        | FAT-1.12.2-4.11-92       | LagGoggles-FAT-1.12.2-4.11-92.jar                           | None                                     |
       | LC    | letsencryptcraft                  | @VERSION@                | letsencryptcraft-1.10.2-1.2.0.jar                           | None                                     |
       | LC    | levelup2                          | ${version}               | levelup2-1.5.8.jar                                          | None                                     |
       | LC    | littleframes                      | 1.0.0                    | LittleFrames_v1.0.12_mc1.12.2.jar                           | None                                     |
       | LC    | littletiles                       | 1.5.0                    | LittleTiles_v1.5.58_mc1.12.2.jar                            | None                                     |
       | LC    | lodsofemone                       | 0.1                      | LodsOfEmone-0.1.jar                                         | None                                     |
       | LC    | login_shield                      | 1.12.2-6-g5654706        | Login_Shield-1.12.2-6-g5654706.jar                          | None                                     |
       | LC    | lootcapacitortooltips             | 1.3                      | lootcapacitortooltips-1.3.jar                               | None                                     |
       | LC    | timecore                          | 1.0.1.1                  | TimeCore-1.12.2-1.0.1.1.jar                                 | None                                     |
       | LC    | lootgames                         | 1.0.3.1                  | LootGames-1.12.2-1.0.3.1.jar                                | None                                     |
       | LC    | lostmagic                         | 1.0                      | lostmagic-1.0.2.jar                                         | None                                     |
       | LC    | magicbees                         | 1.0                      | MagicBees-1.12.2-3.1.10.jar                                 | None                                     |
       | LC    | malisiscore                       | 1.12.2-6.5.1-SNAPSHOT    | malisiscore-1.12.2-6.5.1.jar                                | None                                     |
       | LC    | malisisdoors                      | 1.12.2-7.3.0             | malisisdoors-1.12.2-7.3.0.jar                               | None                                     |
       | LC    | maxpotidext                       | 1.0.3                    | maxpotidext-1.0.3.jar                                       | b851b8b7c7f4d8d0e910ff27618150ba80c026ec |
       | LC    | immersivetech                     | 1.9.100                  | MCTImmersiveTechnology-1.12.2-1.9.100.jar                   | None                                     |
       | LC    | mcwroofs                          | 1.0.2                    | mcw-roofs-1.0.2-mc1.12.2.jar                                | None                                     |
       | LC    | mekanismgenerators                | 1.12.2-9.8.3.390         | MekanismGenerators-1.12.2-9.8.3.390.jar                     | None                                     |
       | LC    | mekanismtools                     | 1.12.2-9.8.3.390         | MekanismTools-1.12.2-9.8.3.390.jar                          | None                                     |
       | LC    | menumobs                          | 1.21                     | MenuMobs-1.12.2-1.21.jar                                    | None                                     |
       | LC    | moartinkers                       | 0.6.0                    | moartinkers-0.6.0.jar                                       | None                                     |
       | LC    | mob_grinding_utils                | 0.3.13                   | MobGrindingUtils-0.3.13.jar                                 | None                                     |
       | LC    | numina                            | 1.12.2-1.0.38            | Numina-1.12.2-1.0.38.jar                                    | None                                     |
       | LC    | powersuits                        | 1.12.2-1.0.46            | ModularPowersuits-1.12.2-1.0.46.jar                         | None                                     |
       | LC    | moreoverlays                      | 1.15.1                   | moreoverlays-1.15.1-mc1.12.2.jar                            | None                                     |
       | LC    | guilib                            | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar                  | None                                     |
       | LC    | paintingselgui                    | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar                  | None                                     |
       | LC    | morepaintings                     | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar                  | None                                     |
       | LC    | morph                             | 7.2.0                    | Morph-1.12.2-7.2.1.jar                                      | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LC    | morpheus                          | 1.12.2-3.5.106           | Morpheus-1.12.2-3.5.106.jar                                 | None                                     |
       | LC    | mputils                           | 1.5.6                    | MPUtils-1.12.2-1.5.7.jar                                    | None                                     |
       | LC    | naturesaura                       | 18.1                     | NaturesAura-18.1.jar                                        | None                                     |
       | LC    | naturescompass                    | 1.8.5                    | NaturesCompass-1.12.2-1.8.5.jar                             | None                                     |
       | LC    | netherportalfix                   | 5.3.17                   | NetherPortalFix_1.12.1-5.3.17.jar                           | None                                     |
       | LC    | netherportalspread                | 5.1                      | netherportalspread_1.12.2-5.1.jar                           | None                                     |
       | LC    | recipehandler                     | 0.13                     | NoMoreRecipeConflict-0.13(1.12.2).jar                       | None                                     |
       | LC    | norecipebook                      | 1.2.1                    | noRecipeBook_v1.2.2formc1.12.2.jar                          | None                                     |
       | LC    | oldjava                           | 1.1.11                   | OldJavaWarning-1.12.2-1.1.11.jar                            | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | omlib                             | 3.1.4-249                | omlib-1.12.2-3.1.4-249.jar                                  | None                                     |
       | LC    | openmods                          | 0.12.2                   | OpenModsLib-1.12.2-0.12.2.jar                               | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LC    | openblocks                        | 1.8.1                    | OpenBlocks-1.12.2-1.8.1.jar                                 | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LC    | openmodularturrets                | 3.1.12-378               | openmodularturrets-1.12.2-3.1.12-378.jar                    | None                                     |
       | LC    | oreexcavation                     | 1.4.150                  | OreExcavation-1.4.150.jar                                   | None                                     |
       | LC    | overpoweredarmorbar               | @VERSION@                | overloadedarmorbar-1.0.4g.jar                               | None                                     |
       | LC    | packmode                          | 1.2.0                    | packmode-1.12.2-1.2.0.jar                                   | None                                     |
       | LC    | packmodemenu                      | 1.0.4                    | PackModeMenu-1.0.4.jar                                      | None                                     |
       | LC    | pamscookables                     | 1.1                      | pamscookables-1.1.jar                                       | None                                     |
       | LC    | pigstep                           | 1.12                     | pigstep-1.12.jar                                            | None                                     |
       | LC    | placebo                           | 1.6.0                    | Placebo-1.12.2-1.6.0.jar                                    | None                                     |
       | LC    | thermaldynamics                   | 2.5.6                    | ThermalDynamics-1.12.2-2.5.6.1-universal.jar                | None                                     |
       | LC    | simplyjetpacks                    | 2.2.14.67                | SimplyJetpacks2-1.12.2-2.2.14.67.jar                        | None                                     |
       | LC    | plustic                           | 8.0.1.0                  | plustic-8.0.1.0.jar                                         | None                                     |
       | LC    | portalgun                         | 7.1.0                    | PortalGun-1.12.2-7.1.0.jar                                  | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LC    | potioncore                        | 1.9_for_1.12.2           | PotionCore-1.9_for_1.12.2.jar                               | None                                     |
       | LC    | practicallogistics2               | 3.0.8                    | practicallogistics2-1.12.2-3.0.8-11.jar                     | None                                     |
       | LC    | progressivebosses                 | 1.5.4                    | ProgressiveBosses-1.5.4-mc1.12.x.jar                        | None                                     |
       | LC    | quarkoddities                     | 1                        | QuarkOddities-1.12.2.jar                                    | None                                     |
       | LC    | rats                              | 3.2.14                   | rats-3.2.14-1.12.2.jar                                      | None                                     |
       | LC    | reauth                            | 4.0.3                    | ReAuth-1.12-Forge-4.0.3.jar                                 | daba0ec4df71b6da841768c49fb873def208a1e3 |
       | LC    | reccomplex                        | 1.4.8.2                  | RecurrentComplex-1.4.8.2.jar                                | None                                     |
       | LC    | xreliquary                        | 1.12.2-1.3.4.796         | Reliquary-1.12.2-1.3.4.796.jar                              | None                                     |
       | LC    | resourceloader                    | 1.5.3                    | ResourceLoader-MC1.12.1-1.5.3.jar                           | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LC    | rftoolsdim                        | 5.71                     | rftoolsdim-1.12-5.71.jar                                    | None                                     |
       | LC    | roguelike                         | 2.3.2                    | RoguelikeDungeonsFnarEdition-1.12.2-2.3.2.jar               | None                                     |
       | LC    | roots                             | @VERSION@                | Roots-1.12.2-3.1.6.jar                                      | None                                     |
       | LC    | savemystronghold                  | 1.12.2-1.0.0             | savemystronghold-1.12.2-1.0.0.jar                           | None                                     |
       | LC    | scannable                         | 1.6.3.26                 | Scannable-MC1.12.2-1.6.3.26.jar                             | None                                     |
       | LC    | signpost                          | 1.08.3                   | signpost-1.12.2-1.08.3.jar                                  | None                                     |
       | LC    | storagenetwork                    | 1.8.1                    | SimpleStorageNetwork-1.12.2-1.8.1.jar                       | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
       | LC    | simplycats                        | 1.12.2-0.0.3.1           | simplycats-1.12.2-0.0.3.1.jar                               | None                                     |
       | LC    | stevescarts                       | 2.4.32.137               | StevesCarts-1.12.2-2.4.32.137.jar                           | None                                     |
       | LC    | storagedrawers                    | 5.2.2                    | StorageDrawers-1.12.2-5.4.2.jar                             | None                                     |
       | LC    | storagedrawersextra               | @VERSION@                | StorageDrawersExtras-1.12-3.1.0.jar                         | None                                     |
       | LC    | stupidthings                      | 1.1.6                    | Stupid Things-1.12.2-1.1.6.jar                              | None                                     |
       | LC    | stygian                           | 1.0.4                    | stygian-1.0.4.jar                                           | None                                     |
       | LC    | taiga                             | 1.12.2-1.3.3             | taiga-1.12.2-1.3.4.jar                                      | None                                     |
       | LC    | tfspellpack                       | 1.1.0                    | TFSpellPack-1.1.0-MC1.12.2.jar                              | None                                     |
       | LC    | thaumicaugmentation               | 1.12.2-2.1.8             | ThaumicAugmentation-1.12.2-2.1.8.jar                        | 8f678591ba6f78d579e553a8aa94b4c4766cb13d |
       | LC    | thaumicjei                        | 1.6.0                    | ThaumicJEI-1.12.2-1.6.0-27.jar                              | None                                     |
       | LC    | thaumicperiphery                  | 0.3.1                    | thaumicperiphery-0.3.1.jar                                  | None                                     |
       | LC    | beneath                           | 1.7.0                    | The Beneath-1.12.2-1.7.0.jar                                | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LC    | theaurorian                       | 1.12.2-Release           | theaurorian-1.12.2-release-may3021.jar                      | None                                     |
       | LC    | thermalcultivation                | 0.3.6                    | ThermalCultivation-1.12.2-0.3.6.1-universal.jar             | None                                     |
       | LC    | thermalinnovation                 | 0.3.6                    | ThermalInnovation-1.12.2-0.3.6.1-universal.jar              | None                                     |
       | LC    | tidychunk                         | 1.0.0.0                  | TidyChunk-1.12.2-1.0.0.0.jar                                | 7a2128d395ad96ceb9d9030fbd41d035b435753a |
       | LC    | tinkersjei                        | 1.2                      | tinkersjei-1.2.jar                                          | None                                     |
       | LC    | tinkertoolleveling                | 1.12.2-1.1.0.DEV.b23e769 | TinkerToolLeveling-1.12.2-1.1.0.jar                         | None                                     |
       | LC    | tips                              | 1.0.9                    | Tips-1.12.2-1.0.9.jar                                       | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LC    | totemic                           | 1.12.2-0.11.6            | Totemic-1.12.2-0.11.6.jar                                   | 21d11d7bf4d97b465382a1f95428029aac6daaea |
       | LC    | toughnessbar                      | @VERSION@                | toughnessbar-2.4.jar                                        | None                                     |
       | LC    | treasure2                         | 2.1.1                    | Treasure2-mc1.12.2-f14.23.5.2859-v2.1.1.jar                 | None                                     |
       | LC    | treasure2_twilight_forest_lp      | 2.0.0                    | Treasure2TwilightForestLP-mc1.12.2-f14.23.5.2859-v2.0.0.jar | None                                     |
       | LC    | treasure2_wizardry_lp             | 2.0.0                    | Treasure2WizardryLP-mc1.12.2-f14.23.5.2859-v2.0.0.jar       | None                                     |
       | LC    | treechop                          | 0.14.6                   | TreeChop-1.12.2-0.14.7.jar                                  | None                                     |
       | LC    | vampiresneedumbrellas             | 1.4                      | VampiresNeedUmbrellas-1.12.2-1.5.jar                        | None                                     |
       | LC    | vampirism                         | 1.6.2                    | Vampirism-1.12.2-1.6.2.jar                                  | None                                     |
       | LC    | teamlapen-lib                     | 1.6.2                    | Vampirism-1.12.2-1.6.2.jar                                  | None                                     |
       | LC    | vampirism_integrations            | vampirism_integrations   | VampirismIntegrations-1.12.2-1.3.0.jar                      | None                                     |
       | LC    | vanillafix                        | 1.0.10-150               | VanillaFix-1.0.10-150.jar                                   | None                                     |
       | LC    | villagenames                      | 4.1.5                    | VillageNames-1.12.2-4.1.5.jar                               | None                                     |
       | LC    | wailaharvestability               | 1.1.12                   | WailaHarvestability-mc1.12-1.1.12.jar                       | None                                     |
       | LC    | wanionlib                         | 1.12.2-2.5               | WanionLib-1.12.2-2.5.jar                                    | None                                     |
       | LC    | waystones                         | 4.1.0                    | Waystones_1.12.2-4.1.0.jar                                  | None                                     |
       | LC    | wings                             | 1.1.6                    | wings-1.1.6-1.12.2.jar                                      | None                                     |
       | LC    | mowzies_wings                     | 1.0.0                    | wings-1.1.6-1.12.2.jar                                      | None                                     |
       | LC    | bauble_wings                      | 1.0.0                    | wings-1.1.6-1.12.2.jar                                      | None                                     |
       | LC    | wct                               | 3.12.97                  | WirelessCraftingTerminal-1.12.2-3.12.97.jar                 | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LC    | witherskelefix                    | 2.6.3                    | WitherSkeletonTweaks-1.12.2-2.6.3.jar                       | None                                     |
       | LC    | wgblockreplacer                   | 2.2.0                    | WorldgenBlockReplacer-1.12.2-2.2.0.jar                      | None                                     |
       | LC    | wrcbe                             | 2.3.2                    | WR-CBE-1.12.2-2.3.2.33-universal.jar                        | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LC    | xnet                              | 1.8.2                    | xnet-1.12-1.8.2.jar                                         | None                                     |
       | LC    | yabba                             | 1.1.2.54                 | YABBA-1.1.2.54.jar                                          | None                                     |
       | LC    | ynot                              | 0.2.4                    | YNot-0.2.4.jar                                              | None                                     |
       | LC    | yoyos                             | 1.12.2-1.3.3.25          | yoyos_1.12.2-1.3.3.25.jar                                   | None                                     |
       | LC    | zerocore                          | 1.12.2-0.1.2.9           | zerocore-1.12.2-0.1.2.9.jar                                 | None                                     |
       | LC    | ancientspellcraft                 | 1.12.2-1.5.5             | AncientSpellcraft-1.12.2-1.5.5.jar                          | None                                     |
       | LC    | lemonlib                          | 1.3.0                    | lemonlib-1.12.2-1.3.0.jar                                   | None                                     |
       | LC    | arcaneworld                       | 0.0.11                   | arcaneworld-1.12.2-0.0.11.jar                               | None                                     |
       | LC    | rf-capability-adapter             | 1.1.1                    | capabilityadapter-1.1.1.jar                                 | None                                     |
       | LC    | structurize                       | 1.12.2-0.10.277-RELEASE  | structurize-1.12.2-0.10.277-RELEASE.jar                     | None                                     |
       | LC    | minecolonies                      | 1.12.2-0.11.841-ALPHA    | minecolonies-1.12.2-0.11.841-BETA-universal.jar             | None                                     |
       | LC    | wizardryutils                     | 1.12.2-v1.1.1            | WizardryUtils-1.12.2-v1.1.1.jar                             | None                                     |
       | LC    | morphspellpack                    | 1.12.2-1.0.0             | MorphSpellPack-1.12.2-1.0.0.jar                             | None                                     |
       | LC    | mospells                          | 1.0.3                    | MoSpells-1.12.2-1.0.3.jar                                   | None                                     |
       | LC    | solcarrot                         | 1.8.4                    | solcarrot-1.12.2-1.8.4.jar                                  | None                                     |
       | LC    | spellbundle                       | 1.12.2-1.1.2             | SpellBundle-1.12.2-1.1.2.jar                                | None                                     |
       | LC    | techreborn_compat                 | 1.0.0                    | TechReborn-ModCompatibility-1.12.2-1.4.0.76.jar             | 8727a3141c8ec7f173b87aa78b9b9807867c4e6b |
       | LE    | thebetweenlands                   | 3.7.3                    | TheBetweenlands-3.7.3-universal.jar                         | 38067d6878811efb38b6a045521cfd80b9b60b38 |
       | L     | midnight                          | 0.3.5                    | themidnight-0.3.5.jar                                       | None                                     |
       | L     | necromancersdelight               | 1.0.3                    | WizardryNecromancersDelight-1.12.2-1.0.3.jar                | None                                     |
       | L     | armoryexpansion-conarm            | 1.4.2                    | armoryexpansion-1.4.2.jar                                   | None                                     |
       | L     | mysticallib                       | 1.12.2-1.13.0            | mysticallib-1.12.2-1.13.0.jar                               | None                                     |
       | L     | teslacorelib_registries           | 1.0.17                   | tesla-core-lib-1.12.2-1.0.17.jar                            | None                                     |
       | L     | tweakersconstructpostload         | 1.12.2-1.6.0             | tweakersconstruct-1.12.2-1.6.0.jar                          | None                                     |
       | L     | unidict                           | 1.12.2-3.0.7             | UniDict-1.12.2-3.0.7.jar                                    | None                                     |
       | L     | wrapup                            | 1.12-1.1.3               | WrapUp-1.12-1.1.3.jar                                       | None                                     |
       | UD    | mdecore-core                      | 1.0                      | minecraft.jar                                               | None                                     |
       | UD    | mobends_wings                     | 1.0.0                    | wings-1.1.6-1.12.2.jar                                      | None                                     |
  Loaded coremods (and transformers): wings (wings-1.1.6-1.12.2.jar)
                                        me.paulf.wings.server.asm.WingsRuntimePatcher
                                        me.paulf.wings.server.asm.mobends.WingsMoBendsRuntimePatcher
                                      IELoadingPlugin (ImmersiveEngineering-core-0.12-98.jar)
                                        blusunrize.immersiveengineering.common.asm.IEClassTransformer
                                      TransformerLoader (OpenComputers-MC1.12.2-1.7.5.192.jar)
                                        li.cil.oc.common.asm.ClassTransformer
                                      MekanismCoremod (Mekanism-1.12.2-9.8.3.390.jar)
                                        mekanism.coremod.KeybindingMigrationHelper
                                      BewitchmentFMLLoadingPlugin (bewitchment-1.12.2-0.0.22.64.jar)
                                        
                                      Quark Plugin (Quark-r1.6-179.jar)
                                        vazkii.quark.base.asm.ClassTransformer
                                      AppleCore (AppleCore-mc1.12.2-3.4.0.jar)
                                        squeek.applecore.asm.TransformerModuleHandler
                                      ObfuscatePlugin (obfuscate-0.4.2-1.12.2.jar)
                                        com.mrcrayfish.obfuscate.asm.ObfuscateTransformer
                                      iceandfire (iceandfire-1.9.1-1.12.2.jar)
                                        com.github.alexthe666.iceandfire.patcher.IceAndFireRuntimePatcher
                                      Inventory Tweaks Coremod (InventoryTweaks-1.63.jar)
                                        invtweaks.forge.asm.ContainerTransformer
                                      EnderCorePlugin (EnderCore-1.12.2-0.5.76-core.jar)
                                        com.enderio.core.common.transform.EnderCoreTransformer
                                        com.enderio.core.common.transform.SimpleMixinPatcher
                                      PhosphorFMLLoadingPlugin (phosphor-1.12.2-0.2.6+build50-universal.jar)
                                        
                                      Thaumic Augmentation Core Plugin (ThaumicAugmentation-1.12.2-2.1.8.jar)
                                        thecodex6824.thaumicaugmentation.core.TATransformer
                                      ratscore (rats-3.2.14-1.12.2.jar)
                                        com.github.alexthe666.rats.server.misc.RatsRuntimePatcher
                                      LittlePatchingLoader (LittleTiles_v1.5.58_mc1.12.2.jar)
                                        com.creativemd.littletiles.LittleTilesTransformer
                                      LevelUpCore (levelup2-1.5.8.jar)
                                        
                                      LoadingPlugin (ResourceLoader-MC1.12.1-1.5.3.jar)
                                        lumien.resourceloader.asm.ClassTransformer
                                      MixinBooter (!mixinbooter-5.0.jar)
                                        
                                      MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
                                        
                                      LoadingPlugin (HardcoreDarkness-MC1.12.2-2.0.jar)
                                        lumien.hardcoredarkness.asm.ClassTransformer
                                      IvToolkit (IvToolkit-1.3.3-1.12.jar)
                                        
                                      LoadingPlugin (Reskillable-1.12.2-1.13.0.jar)
                                        codersafterdark.reskillable.base.asm.ClassTransformer
                                      ColorUtilityCorePlugin (ColorUtility-universal-1.0.4.jar)
                                        com.Axeryok.ColorUtility.ColorUtilityTransformer
                                      LoadingPlugin (RandomThings-MC1.12.2-4.2.7.4.jar)
                                        lumien.randomthings.asm.ClassTransformer
                                      ErebusFix Mixin Loading Plugin (erebusfix-1.12.2-0.0.0.1.jar)
                                        
                                      RandomPatches (randompatches-1.12.2-1.22.1.10.jar)
                                        com.therandomlabs.randompatches.core.RPTransformer
                                      ReachFixPlugin (ReachFix-1.12.2-1.0.5.jar)
                                        meldexun.reachfix.asm.ReachFixClassTransformer
                                      CQRPlugin (Chocolate_Quest_Repoured-1.12.2-2.6.12B.jar)
                                        team.cqr.cqrepoured.asm.CQRClassTransformer
                                      ForgelinPlugin (Forgelin-1.8.4.jar)
                                        
                                      midnight (themidnight-0.3.5.jar)
                                        com.mushroom.midnight.core.transformer.MidnightClassTransformer
                                      CreativePatchingLoader (CreativeCore_v1.10.70_mc1.12.2.jar)
                                        
                                      Do not report to Forge! (If you haven't disabled the FoamFix coremod, try disabling it in the config! Note that this bit of text will still appear.) (foamfix-0.10.14-1.12.2.jar)
                                        pl.asie.foamfix.coremod.FoamFixTransformer
                                      OpenModsCorePlugin (OpenModsLib-1.12.2-0.12.2.jar)
                                        openmods.core.OpenModsClassTransformer
                                      FutureMC (future-mc-0.2.11.jar)
                                        thedarkcolour.futuremc.asm.CoreTransformer
                                      CorePlugin (ForgeEndertech-1.12.2-4.5.5.0-build.0561.jar)
                                        
                                      Launcher Tray (ftb-progress.jar)
                                        net.creeperhost.launchertray.transformer.MinecraftTransformer
                                        net.creeperhost.launchertray.transformer.StepTransformer
                                        net.creeperhost.launchertray.transformer.SplashTransformer
                                      CTMCorePlugin (CTM-MC1.12.2-1.0.2.31.jar)
                                        team.chisel.ctm.client.asm.CTMTransformer
                                      AdvancedRocketryPlugin (AdvancedRocketry-1.12.2-1.7.0-232-universal.jar)
                                        zmaster587.advancedRocketry.asm.ClassTransformer
                                      CharmLoadingPlugin (Charm-1.12.2-1.4.1.jar)
                                        svenhjol.charm.base.CharmClassTransformer
                                      Plugin (NotEnoughIDs-1.5.4.4.jar)
                                        ru.fewizz.neid.asm.Transformer
                                      llibrary (llibrary-core-1.0.11-1.12.2.jar)
                                        net.ilexiconn.llibrary.server.core.plugin.LLibraryTransformer
                                        net.ilexiconn.llibrary.server.core.patcher.LLibraryRuntimePatcher
                                      AstralCore (astralsorcery-1.12.2-1.10.27.jar)
                                        
                                      MDECore-Core (mdecore-1.12-1.1.jar)
                                        com.mattdahepic.mdecore.asm.TickrateTransformer
                                      VanillaFixLoadingPlugin (VanillaFix-1.0.10-150.jar)
                                        
                                      HCASM (HammerLib-1.12.2-2.0.6.32.jar)
                                        com.zeitheron.hammercore.asm.HammerCoreTransformer
                                      Max Potion ID Extender (maxpotidext-1.0.3.jar)
                                        zabi.minecraft.maxpotidext.MPIDTransformer
                                      TARCore (ThaumicAdditions-1.12.2-12.7.8.jar)
  GL info: ' Vendor: 'NVIDIA Corporation' Version: '4.6.0 NVIDIA 516.94' Renderer: 'NVIDIA GeForce GTX 960/PCIe/SSE2'
  OpenModsLib class transformers: [llama_null_fix:FINISHED],[horse_base_null_fix:FINISHED],[pre_world_render_hook:FINISHED],[player_render_hook:FINISHED],[horse_null_fix:FINISHED]
  AE2 Version: stable rv6-stable-7 for Forge 14.23.5.2768
  Ender IO: No known problems detected.
            Authlib is : /C:/Users/19317/AppData/Local/.ftba/bin/libraries/com/mojang/authlib/1.5.25/authlib-1.5.25.jar
            
            !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
            !!!You are looking at the diagnostics information, not at the crash.       !!!
            !!!Scroll up until you see the line with '---- Minecraft Crash Report ----'!!!
            !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
  Pulsar/tconstruct loaded Pulses: - TinkerCommons (Enabled/Forced)
                                   - TinkerWorld (Enabled/Not Forced)
                                   - TinkerTools (Enabled/Not Forced)
                                   - TinkerHarvestTools (Enabled/Forced)
                                   - TinkerMeleeWeapons (Enabled/Forced)
                                   - TinkerRangedWeapons (Enabled/Forced)
                                   - TinkerModifiers (Enabled/Forced)
                                   - TinkerSmeltery (Enabled/Not Forced)
                                   - TinkerGadgets (Enabled/Not Forced)
                                   - TinkerOredict (Enabled/Forced)
                                   - TinkerIntegration (Enabled/Forced)
                                   - TinkerFluids (Enabled/Forced)
                                   - TinkerMaterials (Enabled/Forced)
                                   - TinkerModelRegister (Enabled/Forced)
                                   - chiselIntegration (Enabled/Not Forced)
                                   - chiselsandbitsIntegration (Enabled/Not Forced)
                                   - craftingtweaksIntegration (Enabled/Not Forced)
                                   - wailaIntegration (Enabled/Not Forced)
                                   - quarkIntegration (Enabled/Not Forced)
  HammerCore Debug Information: Dependent Mods:
                                -Thaumic Additions: Reconstructed (thaumadditions) @ 12.7.8
  Suspected Mods: The Betweenlands (thebetweenlands)
  Launched Version: 1.12.2-forge-14.23.5.2860
  LWJGL: 2.9.4
  OpenGL: NVIDIA GeForce GTX 960/PCIe/SSE2 GL version 4.6.0 NVIDIA 516.94, NVIDIA Corporation
  GL Caps: Using GL 1.3 multitexturing.
           Using GL 1.3 texture combiners.
           Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
           Shaders are available because OpenGL 2.1 is supported.
           VBOs are available because OpenGL 1.5 is supported.
  Using VBOs: Yes
  Is Modded: Definitely; Client brand changed to 'fml,forge'
  Type: Client (map_client.txt)
  Resource Packs: 
  Current Language: English (US)
