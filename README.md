# ThaumicEnergistics
*Because the digital age could use some magic!*

Preface
---
This is a fork to try and improve the usability of Thaumic Energistics. This is currently being updated to help current
players during Divine Journey 2. Now also used by FTB Interactions 2.12+.

Some warnings
* I know development, but I don't know Minecraft modding. I've not done this before. I might break 
things. Backup before you use this.
* If you're worried about security, don't use this. This isn't yet vetted by anyone, or Curseforge or the like.
Not only that, but it's a fork, of a fork, of a fork. I haven't thoroughly checked the previous contributors for
potential security problems either. It looks fine on the surface, but I haven't gone deep.

Changes in this fork
* Essentia cell partitioning has been fixed. Previously, you could partition a cell, but the logic was not checked for
correctly.
* Arcane Crafting Terminal efficiency improvements. In a test world the ACT is fine, but in a big network
with many items, it was very laggy. By the looks of things, this was getting the entire list of viewable
items, sometimes multiple times. The fixes for this involved just checking the AE2 code base and porting their
efficiency fixes into a form that is compatible with Thaumic Energistics.
  * Changing the ACT to work on a diff of items instead of the entire list.
  * Compressing the packet data sent to the user when data was changed.

---

[![discord]](https://discord.gg/ywBJYK6)
[![curseforge-downloads]](https://minecraft.curseforge.com/projects/thaumic-energistics)
[![curseforge-versions]](https://minecraft.curseforge.com/projects/thaumic-energistics)
[![build-status]](https://ci.brock.pw/job/Thaumic%20Energistics%20RV6/)

The following mods are required for this mod:
- Thaumcraft
- Applied Energistics 2

About
---
The aim of this mod is to serve as a bridge between Thaumcraft and Applied Energistics. The primary focus is essentia management, both in storage, transportation, and application.

Thanks go out to AlgorithmX2 for Applied Energistics, Azanor for Thaumcraft, M3gaFr3ak for ExtraCells, and the Forge team.

1.12.2 Localization's thanks to Hesperusrus.
1.7.10 Localization's thanks to Mrkwtkr, alvin137, puyo061, Wuestengecko, TheVizzy, Adaptivity, Joccob, & Keridos.
Texture thanks to CyanideX.
Special thanks to MKoanga, Keridos & Aquahatsche.

Built for Minecraft 1.12.2

Code Analysis
---
[![](https://sonarcloud.io/images/project_badges/sonarcloud-white.svg)](https://sonarcloud.io/dashboard?id=thaumicenergistics%3AThaumicEnergistics)

![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=sqale_rating) ![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=reliability_rating) ![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=security_rating)

![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=ncloc) ![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=bugs) ![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=vulnerabilities) ![](https://sonarcloud.io/api/project_badges/measure?project=thaumicenergistics%3AThaumicEnergistics&metric=code_smells)

API
---

Thaumic Energistics has an API similar to the AE2 API. Check src/api/java for more API info.

#### Maven

*Coming soon*

How To Contribute
---

## Code Format
Code formatting is pretty simple, just keep to defaults. No tabs, use 4 spaces instead.

## Compile

1. Run ./gradlew setupDecompWorkspace build
2. Your build shall be in build/libs/

[discord]: https://img.shields.io/discord/564475651222929418
[build-status]: https://ci.brock.pw/job/Thaumic%20Energistics%20RV6/badge/icon
[curseforge-downloads]: http://cf.way2muchnoise.eu/thaumic-energistics.svg
[curseforge-versions]: http://cf.way2muchnoise.eu/versions/thaumic-energistics.svg
