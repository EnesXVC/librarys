## Booting the Library
```lua
local module = loadstring(game:HttpGet("https://raw.githubusercontent.com/EnesXVC/librarys/main/coolbluelib/source"))()
```
## Create Window
```lua
local window = module:New("WindowName")
```
## Create Tab
```lua
local tab1 = window:NewTab("TabName")
```
## Create Button
```lua
tab1:NewButton("Button", "Description", function()
    print("Button Clicked!")
end)
```
## Create Toggle
```lua
tab1:NewBoolButton("Toggle Button", "On/Off switch", function(state)
    print("Toggle state:", state)
end, false)
```
## Create Label
```lua
local label = tab1:NewLabel("This is a label")
```
## Create Textbox (How to works idk)
```lua
local textBox = tab1:NewTextBar("Text Box", "Type something here")
print(textBox:GetText()) -- Get the text
textBox.Text = "New text" -- Change the text
```
## Set Footer
```lua
window:SetFooter("v1.0.0 - Name")
```
## Set Footer
```lua
window:SetFooter("v1.0.0 - Name")
```
## Create Cmd (use cmds for to see commands)
```lua
local cmdBar = window:NewCommandBar("Enter a command...")
```
## Create A Command
```lua
cmdBar:AddCommand("hello", {}, "Prints 'Hello'", function(args)
    print("Hello!")
end)
```
## Create A Command With Arguments
```lua
cmdBar:AddCommand("hello", {}, "Prints 'Hello'", function(args)
    print("Hello!")
end)
```
