## Booting the Library
```lua
local ErrorPopup = loadstring(game:HttpGet("https://raw.githubusercontent.com/EnesXVC/librarys/main/Error/Source"))()
```
## Configure the settings
```lua
ErrorPopup:SetTitle("Rayfield couldn't start")
ErrorPopup:SetSubtitle("Critical Erro")
ErrorPopup:SetContent("Rayfield has encountered an error that is preventing it from running properly.\nDevelopers have been notified and more details can be found in console.")
ErrorPopup:SetIcon("rbxassetid://104519944497764")
ErrorPopup:SetButtonText("Dismiss")
ErrorPopup:SetPosition("center") -- "left", "center", "right"
```
## Create Gui(NEED)
```lua
ErrorPopup:Create()
```
### Credits:
- [EnesXVC](https://github.com/EnesXVC) (Library)
- [SiriusSoftwareLtd](https://github.com/SiriusSoftwareLtd) (Gui)
