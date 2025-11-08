## Booting the Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/EnesXVC/librarys/main/SearchAndChangeLogLibrary/Source"))()
```
## Configure the settings
```lua
local dialog = Library:CreateChangelogDialog({
    Title = "My Changelog",
    ChangelogText = [[
    Version: 1.5
    New Features:
    - Library Build Version 1.5
    - Notifications updated
    ]],
    Search = true, --true , false
    NotifyLibrary = "Rayfield", -- "Luna" or "Rayfield"
    Notifications = true, -- true , false
-- Second Button
    Altbutton = {
        Name = "Join Discord",
        Clipboard = "discord.gg/example" -- discord.gg/rTw5M8dRXN
    },
-- Close Button Nofication
    Notification = {
        Title = "Changelog",
        Content = "The changelog has been closed",
        Duration = 3,
        Image = 10723346871
    },
-- Join Discord Button Nofications
    AltbuttonNotification = {
        Success = {
            Title = "Copied!",
            Content = "Link copied to clipboard",
            Duration = 5,
            Image = 10709798443
        },
        Failure = {
            Title = "Error",
            Content = "Clipboard not supported",
            Duration = 5,
            Image = 10709799124
        }
    }
})
-- And Mobile Support Pc Support
```
### Credits:
- [EnesXVC](https://github.com/EnesXVC) (Library)
- [SiriusSoftware](https://github.com/SiriusSoftwareLtd) (Gui)
