# ElvUI_AddOnSkins — SuttonX fork for WoW 3.3.5a

A compatibility and diagnostics fork of [ElvUI-WotLK/ElvUI_AddOnSkins](https://github.com/ElvUI-WotLK/ElvUI_AddOnSkins).  This plugin styles supported third-party addons to match [ElvUI for Wrath of the Lich King](https://github.com/ElvUI-WotLK/ElvUI).

Credit for the original addon and skins belongs to the upstream authors, including Bunny, Azilroka, and Sortokk.  This independent fork builds on upstream master; it is not an official upstream release.

## Changes in this fork

- Missing-frame guards across 92 skin files skip absent controls during common skin operations.
- Auctionator checkbox guards accommodate controls missing in some versions.
- MoveAnything guards cover mover backdrops, mouse handlers, option controls, and row anchoring.
- Optional suppression of AddOnSkins-related Lua error popups, enabled by default.
- An Errors tab with recent session errors and a clear action.
- Red [!] indicators and the latest recorded error beside affected addon options.

Upstream master's newer skin coverage and compatibility work are retained.  These fixes have been submitted to the original project in [PR #195](https://github.com/ElvUI-WotLK/ElvUI_AddOnSkins/pull/195).

The combined master-based build was tested in game with no popups and no errors recorded that session.  This covers the tested installation, not every supported addon combination.

## Requirements

- World of Warcraft: Wrath of the Lich King **3.3.5a**.
- [ElvUI-WotLK ElvUI](https://github.com/ElvUI-WotLK/ElvUI), installed and enabled.  This required dependency is not bundled.
- Compatible 3.3.5a versions of the supported addons you want to skin.  These addons are not bundled; installing every supported addon is unnecessary.

This fork replaces the original ElvUI_AddOnSkins folder.  Do not install a second differently named copy alongside it.

## Installation and updating

1. Close WoW.
2. On [this fork](https://github.com/SuttonX/ElvUI_AddOnSkins), choose **Code → Download ZIP**.
3. Extract the ZIP and locate the **ElvUI_AddOnSkins** folder inside the outer repository folder.
4. Replace the existing **Interface/AddOns/ElvUI_AddOnSkins** folder with that folder.  Keep your saved variables and WTF folder.
5. Confirm **Interface/AddOns/ElvUI_AddOnSkins/ElvUI_AddOnSkins.toc** exists.  Do not install the outer repository folder or leave the addon nested inside another folder.
6. Start WoW and enable **ElvUI** and **ElvUI AddOnSkins** in the character-selection addon list.

## Settings and diagnostics

Open ElvUI configuration with **/ec** and select the **AddOnSkins** plugin settings to enable or disable individual skins.

The **Errors** tab displays recent AddOnSkins errors, clears the session log, and lets you disable popup suppression.  An attributed skin error marks the affected addon option red with **[!]** and includes its latest error in the description.

Diagnostics reset on UI reload or game restart.  Up to 30 recent records are retained and the latest 10 messages displayed.  No additional error-catching addon is required.

Guards skip missing targets; they do not create controls or guarantee compatibility with every addon version.  Suppression does not repair or resume a failed skin callback.  Attribution uses an AddOnSkins source path in the error message or stack; unrelated errors are forwarded to the previous handler.  Other addons installing error handlers later may affect this behavior.

For a fork-specific problem, include the affected addon/version, what triggered it, and the message from the Errors tab.  See the [original repository](https://github.com/ElvUI-WotLK/ElvUI_AddOnSkins) for upstream development.

## Supported addons

Compatibility depends on addon version.  The inherited upstream list follows; master also includes SlideBar and LootWonAlert skins.

1. _NPCScan
1. _NPCScan.Overlay
1. AckisRecipeList
1. ACP - Addon Control Panel
1. AdiBags
1. AdvancedTradeSkillWindow
1. AllStats
1. Altoholic
1. ArkInventory
1. Atlas
1. AtlasLoot
1. AtlasQuest
1. Auctionator
1. AuctioneerSuite
1. BigWigs
1. BindPad
1. BlackList
1. BugSack
1. BuyEmAll
1. CallToArms
1. Carbonite
1. ChatBar
1. ChocolateBar
1. CLCRet
1. Clique
1. DBM - Deadly Boss Mods
1. Doom_CooldownPulse
1. ElvinCDs
1. EPGP
1. EPGP_LootMaster
1. EquipCompare
1. EventAlert
1. EveryQuest
1. Examiner
1. Factionizer
1. FeralbyNight
1. FishingBuddy
1. FlightMap
1. FloAspectBar
1. FloHunterBars
1. FloTotemBar
1. GearScore
1. GnomishVendorShrinker
1. InspectEquip
1. ItemRack
1. KarniCrap
1. KHunterTimers
1. LightHeaded
1. LootCouncilLite
1. LoseControl
1. MageNuggets
1. Mapster
1. MoveAnything
1. Omen
1. OpenGF
1. oRA3
1. Outfitter
1. Overachiever
1. PAB - Party Ability Bars
1. PallyPower
1. PlateBuffs
1. Poisoner
1. Postal
1. PowerAuras
1. Quartz
1. QuestGuru
1. QuestGuru_Tracker
1. QuestPointer
1. RaidCooldowns
1. RaidRoll
1. RCLootCouncil
1. Recount
1. SatrinaBuffFrame
1. SexyCooldown
1. SilverDragon
1. Skada
1. Skillet
1. Spy
1. Stalker
1. SuperDuperMacro
1. Talented
1. TellMeWhen
1. TinyPad
1. TipTac
1. TotemTimers
1. TradeskillInfo
1. TrinketMenu
1. VanasKoS
1. WIM
1. WeakAuras
1. WowLua
1. ZOMGBuffs
1. ZygorGuidesViewer
1. ZygorTalentAdvisor
1. Quick DKP V2
