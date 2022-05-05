# nhm-plugins
**Custom NiceHash Miner Plugins**

On February 17, 2022, NiceHash announced that they will no longer support unsigned and unverified miners (https://www.nicehash.com/blog/post/nicehash-miner-ceases-support-for-unsigned-and-unverified-miners).  This is my attempt to create custom NHM plugins to replace popular miners like GMiner and T-Rex.

## Instructions
1. Follow the NHM instructions to create a new empty user plugin: https://github.com/nicehash/NiceHashMiner/tree/master/doc/UserPlugins
    - Name your plugin the same as it is here (`GMinerCustom`, `TRexCustom`, etc).  This isn't required but just for ease of use.
    - When editing the `Devices.json` file, make sure the `miner_device_id` matches correctly.  This is not always the case when you have multiple GPUs.  This will cause incorrect benchmarks, otherwise.
    - STOP after editing the `Devices.json` file.  The rest will be taken care of by this repo.
2. Copy the contents over for the appropriate miner plugin.
3. Update each miner's `bins` directory with the latest version of the miner (README in plugin folder has the download link).
4. Start NiceHash Miner.

## Completed
- GMiner (https://github.com/develsoftware/GMinerRelease)

## TODO
- T-Rex (https://github.com/trexminer/T-Rex)
- miniZ (https://github.com/miniZ-miner/miniZ) ??

## References
NHM Algorithm IDs:
https://github.com/nicehash/NiceHashMiner/blob/d5b99f69b7a818043c8825dedaa491f88f41c039/src/NHM.Common/Enums/AlgorithmType.cs
