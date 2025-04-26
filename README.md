# CharacterInfo

A library that provides character and realm information.

#### Dependencies: [LibStub](https://www.curseforge.com/wow/addons/libstub), [Contracts](https://github.com/Eyal-WowHub/Contracts)

#### Used By: [WowInfo](https://github.com/Eyal-WowHub/WowInfo)

### Example:

```lua
local CharacterInfo = LibStub("CharacterInfo-1.0")

for isPlayerRealm, realm in CharacterInfo:IterableConnectedRealms() do
    if isPlayerRealm then
        print(realm, CharacterInfo:GetName())
    else
        print(realm)
    end
end
```