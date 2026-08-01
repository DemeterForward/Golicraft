# [packwiz](https://packwiz.infra.link/)
Packs are created and exported using packwiz.
## Process of creating a modpack through packwiz:
1. Create a folder *somewhere*
2. `packwiz init`
3. Start adding mods through `packwiz curseforge install` or `packwiz modrinth install` 
	- Most of the time you can just add the mod's name but some times that will not work. For those times, it's recommened to add the link of the mod instead (`packwiz modrinth install https://modrinth.com/mod/modelfix`).
4. `packwiz curseforge export` to export the modpack into a `.zip` file or `packwiz modrinth export` to export the modpack into a `.mrpack`, or just `packwiz curseforge export && packwiz modrinth export` for both.