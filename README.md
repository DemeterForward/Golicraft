# Introducing a more modular approach to modpack creation.
### Inside the main folder are multiple subfolders acting as modules. These modules will be combined into the creation of the final modpack. With this modularity, better modpack management is gained, especially when updating, troubleshooting or adding additional mods.
<pre>
.
├── create
│   └── mods
├── food
│   ├── 1.20.1
│   │   └── mods
│   └── 1.21.1
│       └── mods
├── magic
│   └── mods
└── storage
    └── mods
</pre>
---
### Modules are created and exported using [packwiz](https://packwiz.infra.link/).
#### Process of creating a module through packwiz:
1. Create a folder *somewhere*
2. `packwiz init`
3. Start adding mods through `packwiz curseforge install` or `packwiz modrinth install` 
	- Most of the time you can just add the mod's name but some times that will not work. For those times, it's recommened to add the link of the mod instead (`packwiz modrinth install https://modrinth.com/mod/modelfix`)
4. `packwiz curseforge export` to export the module into a `.zip` file or `packwiz modrinth export` to export the module into a `.mrpack`, or just `packwiz curseforge export && packwiz modrinth export` for both

> [!NOTE]
> It is not required to add `.mrpack` and `.zip` to the `.packwizignore` as packwiz will ignore them automatically.
