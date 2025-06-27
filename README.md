# Kernel recommendations:

### Redmi note 8/8T (*ginkgo*/willow)
- SM6125 -> Recommended to be used on LOS, support in other ROMS is not guaranteed. Non RDP/Non Dynamic ROMs only.

Note: while the kernel doesn't have major modifications, no official support is provided if you're using a different kernel in LOS. DO NOT report bugs while using this kernel.

### Mi A3 (laurel_sprout)

- SM6125 -> Recommended to be used on LOS, support in other ROMS is not guaranteed. Non RDP ROMs only.

Note: while the kernel doesn't have major modifications, no official support is provided if you're using a different kernel in LOS. DO NOT report bugs while using this kernel.

- Snowflake -> Based on NoName, has optimizations over NoName, should work on A15 (not sure about other versions). Non RDP.

- NoName 18.1 -> Recommended for A11-A14 QPR1 ROMs. Non RDP.

- NoName VIC -> Use on RDP roms.

# Kernel Labels:

The kernel label uses the following format:
- `buildDate-deviceName-buildType-kernelVariant-runNumber`
As an example you can see:
- `2025.06.18-MiA3-KSU-SM6125-22.2-148`

### buildDate
The date the kernel was built following the format: `YYYY.MM.DD`.
### deviceName
The name of the device the kernel is built for, like `MiA3`.
### buildType
The type of the build, it can be the following:
- Normal (empty)
- KSU (-KSU)
- RKSU (-RKSU)
- KSUN (-KSUN)

For SUSFS variants, the buildType receives a `.SUSFS` suffix.
### kernelVariant
This is the tag/kernel name, currently these are the tags:
- NoName 18.1 -> NoName-18.1
- NoName VIC -> NoName-VIC
- NoName Snowflake -> Snowflake
- SM6125 22.2 -> SM6125-22.2
### runNumber
Simply the number of the github run, don't use this as a definitive versioning metric, always base yourself on the build date.

# Kernels used when building:
 - [NoName LOS 18.1](https://github.com/Mi-A3-laurel-sprout/kernel_xiaomi_XD/tree/lineage-18.1) • NON-RDP • A11-A14 QPR1
 - [NoName VIC](https://github.com/Mi-A3-laurel-sprout/kernel_xiaomi_XD/tree/vic) • RDP
 - [NoName Snowflake](https://github.com/liquidprjkt/snowflake_laurel_sprout) • NON-RDP
 - [SM6125 LOS 22.2](https://github.com/LineageOS/android_kernel_xiaomi_sm6125) • NON-RDP

# Credits:

**Kernel Sources**:
- [@Skyblueborb](https://github.com/Skyblueborb) -> SM6125, NoName 18.1
- [@aleeeee1](https://github.com/aleeeee1) -> 'heresy' mic fix kernel
- [@PowerX-NOT](https://github.com/PowerX-NOT) -> NoName VIC
- [@RainySorcerer](https://github.com/RainySorcerer) -> Snowflake

**Workflow/Patches**:
- [@TheWildJames](https://github.com/TheWildJames) -> workflow reference, patches
- [@simonpunk](https://gitlab.com/simonpunk) -> susfs patches
- [@sidex15](https://github.com/sidex15) -> susfs patches
