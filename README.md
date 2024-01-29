# Syrex Library V3

## loadstring Source

Library Source
```lua
local SyrexLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/SyrexHUB/SyrexLib/main/Source.lua"))()
```
Source Functions
```lua
--[[
  SyrexLib:Destroy() - Void
  
  SyrexLib:Set(550) - number
  
  SyrexLib:Visible() - boolean
]]
```

## Make Window

Create the Home Window
```lua
local Window = SyrexLib:MakeWindow({
  Menu = {
    Title = "Syrex Hub",
  },
  LoadAnim = {
    Active = true,
    Title = ".gg/syrexhub",
    WaitTime = 0.2
  }
})
```
Window Finctions
```lua
--[[
  Window:Destroy() - Void
  
  Window:Visible(false) - boolean
  
  Window:Set(0) - number or Color3
]]
```

## Make Tab

Add a Scroll Tab
```lua
local Tab = Window:MakeTab({
  Name = "Main",
  Image = "rbxassetid://13687780725"
})
```
Tab Functions
```lua
--[[
  Tab:Set("New Name") - Name or Image
  
  Tab:Destroy() - void
   
  Tab:Visible(false) - boolean
]]
```

## Add Tab Separator

Create Scroll Separator
```lua
local Separator = Window:Separator() - Void
```
Separator Functions
```lua
--[[
  Separator:Destroy() - Void
  
  Separator:Visible(false) - boolean
]]
```

## Make Notification

Create Notification
```lua
SyrexLib:MakeNotifi({
  Title = "Syrex Library",
  Text = "Notification Test",
  Time = 5
})
```

## Add Section
Create Section
```lua
local Section = AddSection({"Section"})
```
Section Functions
```lua
--[[
  Section:Set("New Name") - string or Color3
  
  Section:Visible(false) - boolean
  
  Section:Destroy() - void
]]
```

## Add Label

Create Image Label
```lua
local Label = Tab:AddLabel({
  Type = "Text",
  Name = "Text Label"
})
```
Create Text Label
```lua
local Label = Tab:AddLabel({
  Type = "Image",
  Name = "Image Label"
  Image = "rbxassetid://"
})
```
Label Functions
```lua
--[[
  Label:Set("New Name or Image") - Name or Image
  
  Label:Visible(false) - boolean
  
  Label:Destroy() - Void
]]
```

## Add Paragraph

Create Paragraph
```lua
local Paragraph = Tab:AddParagraph({"Paragraph", "Paragraph Test"})
```
Paragraph Functions
```lua
--[[
  Paragraph:Set("New Name", "New Text") - string
  
  Paragraph:Visible(false) - boolean
  
  Paragraph:Destroy() - Void
]]
```

## Add Button

Create Button
```lua
local Button = Tab:AddButton({
  Name = "Button",
  Callback = function()
    
  end
})
```
Button Functions
```lua
--[[
  Button:Set("New Name") - string or function
  
  Button:Visible(false) - boolean
  
  Button:Destroy() - Void
]]
```

## Add Toggle

Create Toggle
```lua
local Toggle = Tab:AddToggle({
  Name = "Toggle",
  Default = false,
  Callback = function(Value)
    
  end
})
```
Toggle Functions
```lua
--[[
  Toggle:Set("New Name") - string or function or boolean
  
  Toggle:Visible(false) - boolean
  
  Toggle:Destroy() - Void
]]
```

## Add Slider

Create Slider
```lua
local Slider = Tab:AddSlider({
  Name = "Slider",
  MinValue = 0,
  MaxValue = 1,
  Default = 0,
  Increase = 0.1,
  Callback = function(Value)
    
  end
})
```
Slider Functions
```lua
--[[
  Slider:Set("New Name") - string or function or number
  
  Slider:Visible(false) - boolean
  
  Slider:Destroy() - Void
]]
```
