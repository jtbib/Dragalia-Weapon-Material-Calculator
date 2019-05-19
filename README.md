# Dragalia Weapon Material Calculator

This is a program to calculate how much material you need to make your desired weapons.

DISCLAIMER: I (jtbib) forked this from yujinred's original implementation and used the provided APIs (with minor modifications), as noted in update_data.py. This is left open source if anybody wants to fork their own copy, issue pull requests, take over the project, etc.

Process to update materials and images (for material source locations):
Use https://dragalialost.gamepedia.com/api.php?action=cargoquery&format=json&limit=max&tables=Materials&fields=Id%2C+Name%2C+Description and identify the added materials (e.g. new void drops). Find banner images on gamepedia (can't find a CargoTable that directs there, but you can try https://dragalialost.gamepedia.com/Special:CargoTables yourself) and save them to images. Add an 'Obtain' and 'Difficulty' entry to each item added, with appropriate values as needed.

### Source

weapon_data.js - pulled from https://dragalialost.gamepedia.com/api.php?action=cargoquery&format=json&limit=max&tables=Weapons&fields=Id%2C+BaseId%2C+FormId%2C+WeaponName%2C+Type%2C+Rarity%2C+ElementalType%2C+MinHp%2C+MaxHp%2C+MinAtk%2C+MaxAtk%2C+VariationId%2C+DecBaseId%2C+DecVariationId%2C+BulletBaseId%2C+BulletVariationId%2C+Skill%2C+SkillName%2C+SkillDesc%2C+IsPlayable%2C+FlavorText%2C+SellCoin%2C+SellDewPoint%2C+CraftNodeId%2C+ParentCraftNodeId%2C+CraftGroupId%2C+FortCraftLevel%2C+AssembleCoin%2C+DisassembleCoin%2C+DisassembleCost%2C+MainWeaponId%2C+MainWeaponQuantity%2C+CraftMaterialType1%2C+CraftMaterial1%2C+CraftMaterialQuantity1%2C+CraftMaterialType2%2C+CraftMaterial2%2C+CraftMaterialQuantity2%2C+CraftMaterialType3%2C+CraftMaterial3%2C+CraftMaterialQuantity3%2C+CraftMaterialType4%2C+CraftMaterial4%2C+CraftMaterialQuantity4%2C+CraftMaterialType5%2C+CraftMaterial5%2C+CraftMaterialQuantity5

material_data.js - pulled from https://dragalialost.gamepedia.com/api.php?action=cargoquery&format=json&limit=max&tables=Materials&fields=Id%2C+Name%2C+Obtain+

Weapon Image data - pulled from https://dragalialost.gamepedia.com/api.php?action=query&format=json&prop=&list=allimages&aifrom=301001_01_19901.png&aito=3100001.png&aiprop=timestamp%7Curl&ailimit=max

Material Image data - pulled from https://dragalialost.gamepedia.com/api.php?action=query&format=json&prop=&list=allimages&aiprop=timestamp%7Curl&ailimit=max&aifrom=111001001.png&aito=210001_01.png&*
