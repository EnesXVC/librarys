## Booting the Library
```lua
local DiscordPopup = loadstring(game:HttpGet("https://raw.githubusercontent.com/EnesXVC/librarys/main/DiscordPopup/Source"))()
```
## Configure the settings
```lua
DiscordPopup:SetCopyText("copy link")
DiscordPopup:SetCloseText("fuck off")
DiscordPopup:SetDiscordLink("https://discord.gg/link")
DiscordPopup:SetLabelText("join the discord :3")
DiscordPopup:SetImages("rbxassetid://18817097052", "rbxassetid://18817519330")
DiscordPopup:SetPosition("left") -- "left", "center", "right"
```
## Create Gui(NEED)
```lua
local popup = DiscordPopup:Create()
```
