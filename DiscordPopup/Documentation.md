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
DiscordPopup:SetPosition("center") -- "left", "center", "right"
```
## Create Gui(NEED)
```lua
local popup = DiscordPopup:Create()
```
### Credits:
- [EnesXVC](https://github.com/EnesXVC) (Library)
- [hellohellohell012321](https://github.com/hellohellohell012321) (Gui)
