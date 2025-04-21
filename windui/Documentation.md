https://cdn.discordapp.com/attachments/1345310389402992694/1363893953338016034/image.png?ex=6807b0ba&is=68065f3a&hm=3b162cc29d438428902156d6a2653f6ae115f6f588e5198fe9ece83d566ebe00&

# WindUI Library

## Booting the Library
```lua
local WindUI = loadstring(game:HttpGet("https://tree-hub.vercel.app/api/UI/WindUI"))()
```
## Creating a Window
```lua
local Window = WindUI:CreateWindow({
    Title = "WindUI Library",
    Icon = "door-open",
    Author = "Example UI",
    Folder = "windui",
    Size = UDim2.fromOffset(580, 460),
    Transparent = true,
    Theme = "Dark",
    UserEnabled = false,
    SideBarWidth = 200,
    HasOutline = true,
    KeySystem = { 
        Key = { "1234", "5678" },
        Note = "Example Key System",
        URL = "https://github.com/Footagesus/WindUI",
        SaveKey = true,
    },
})
```
## Creating a Tab
```lua
local Tab = Window:Tab({ 
    Title = "Tab Title", 
    Icon = "icon-name", --source
    Desc = "Description",
    Locked = true/false 
})
```
## Creating a Button
```lua
Tab:Button({
    Title = "Button Text",
    Desc = "Description",
    Callback = function()
      		print("button pressed")
end,
    Locked = true/false
})
```
## Creating a toggle
```lua
Tab:Toggle({
    Title = "Toggle Label",
    Default = false, --true/false
    Callback = function(Value)
		print(Value
 end
})
```
## Creating a Slider
```lua
Tab:Slider({
    Title = "Slider Name",
    Value = {
        Min = 0,
        Max = 100,
        Default = 50
    },
    Callback = function(Value)
    		print(Value)
    end
})
```
## Creating an Input
```lua
Tab:Input({
    Title = "Input Label",
    Default = "default value",
    Placeholder = "placeholder text",
    Callback = function(Value)
		print(Value)
 end
})
```
## Creating a Dropdown
```lua
Tab:Dropdown({
    Title = "Dropdown Label",
    Values = {"Option1", "Option2"},
    Value = "default option",
    Callback = function(option)
		print(option)
 end
})
```
## Creating a Color Picker
```lua
Tab:Colorpicker({
    Title = "Color Picker",
    Default = Color3.fromRGB(255,0,0),
    Callback = function(color)
		print(color)
 end
})
```
## Creating a Code File
```lua
Tab:Code({
    Title = "filename.lua",
    Code = "lua code here"
})
```
## Creating a Paragraph
```lua
Tab:Paragraph({
    Title = "Title",
    Desc = "Description",
    Image = "icon-name",
    Color = "ColorName", -- Red, Orange, Green, Blue, Grey, White
    Buttons = { {Title = "Button1"}, {Title = "Button2"} }
})
```
## Notifying the user
```lua
WindUI:Notify({
    Title = "Notification",
    Content = "Message content",
    Icon = "icon-name",
    Duration = 5,
    Background = "rbxassetid..."
})
```
## Popup the user
```lua
WindUI:Popup({
    Title = "Popup Title",
    Content = "Message",
    Buttons = {
        {
            Title = "Button",
            Callback = function() end,
            Variant = "Primary/Secondary/Tertiary"
        }
    }
})
```
## Theme Customization
```lua
WindUI:AddTheme({
    Name = "CustomTheme",
    Accent = "#RRGGBB",
    Outline = "#RRGGBB",
    Text = "#RRGGBB",
    PlaceholderText = "#RRGGBB"
})
WindUI:SetTheme("CustomTheme")
```
## Configuration Saving
```lua
-- Save settings
SaveFile("filename", {setting1 = value1, setting2 = value2})

-- Load settings
local data = LoadFile("filename")
```
## Dynamic UI Updates
```lua
-- Refresh dropdown options
dropdown:Refresh(newOptionsList)

-- Change toggle state programmatically
toggle:SetValue(true/false)
```
# Example a Script
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/Footagesus/WindUI/refs/heads/main/Example.lua"))()
-- source
-- https://raw.githubusercontent.com/Footagesus/WindUI/refs/heads/main/Example.lua
```
### Credits:
- [Dawid-Scripts](https://github.com/dawid-scripts) (Colorpicker)
- [Lucide-Icons](https://github.com/lucide-icons/lucide) (Icons)


> [Discord Server](https://discord.gg/Q6HkNG4vwP)
> [Documentation](https://tree-hub.vercel.app/docs/WindUI)
