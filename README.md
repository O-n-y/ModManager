This information how mod creators can interact with Mod Manager.
Mod page: https://steamcommunity.com/sharedfiles/filedetails/?id=1843965353

# Mod version

For your mod version information to be loaded correctly:

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
Also can be found here: https://github.com/O-n-y/ModManager/blob/master/version.info
