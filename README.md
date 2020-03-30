This information how mod creators can interact with Mod Manager.
Mod page: https://steamcommunity.com/sharedfiles/filedetails/?id=1843965353

# Mod version

For your mod version information to be loaded and showed correctly in Mods list dialog:

* **For .dll mods**, it will read version from **AssemblyInfo.cs -> AssemblyVersion**. If you mod have multiple .dll, you can store version info in *version.info* (see information below).
* **For other**, it will search for file *version.info* in mod directory.
  * If version info not found, it will create *version.info.tpl*. 
  * You can open it with text editor and edit version there.
  * Then save it and rename to *version.info*, upload this file with all other files of your mod.

## Example of version.info contents
    <?xml version="1.0" encoding="utf-8"?>
    <VersionInfo xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <Version>1.0.0.0</Version>
    </VersionInfo>
Example of *version.info* also can be found here: https://github.com/O-n-y/ModManager/blob/master/version.info

Upload *version.info* with other files of your mod using Oxygen Not Included Uploader.


# External Links to Discord, Github and Patreon

For your links to be displayed near your mod in Mods list dialog:

* Create *mod.info* file with following content (replace links to your actual) in your mod root folder
```
<?xml version="1.0" encoding="utf-8"?>
<ModInfoData xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <Discord>https://discord.gg/S6d25A</Discord>
  <Github>https://github.com/O-n-y/oxy.mods</Github>
  <Patreon>https://www.patreon.com/ony_mods</Patreon>
</ModInfoData>
```

Example of *mod.info* also can be found here: https://github.com/O-n-y/ModManager/blob/master/mod.info

Upload *mod.info* with other files of your mod using Oxygen Not Included Uploader.
