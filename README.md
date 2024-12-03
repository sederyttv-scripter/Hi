# Getting Started

# To use the ui library you need this

```lua
local UILibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/sederyttv-scripter/Hi/refs/heads/main/Seder%20UILibrary"))()
```

# To load the UI, (required)

```lua
-- Create a window
local ui = UILibrary:NewWindow("Example Window")
```

# to create a tab or section you can use the section for tabs
```
-- Create a section
local section = UILibrary:NewSection(ui, "TabName")
```

# to create a button 
```
UILibrary:CreateButton(section, "Click Me", function()
    print("Button Pressed!")
end)
```

# to create a toggle
```
UILibrary:CreateToggle(section, "Enable Feature", false, function(value)
    if value then
        print("Feature enabled")
    else
        print("Feature disabled")
    end
end)
```

# to create a dropdown
```
UILibrary:CreateDropdown(section, "Select Option", {"Option 1", "Option 2", "Option 3"}, "Option 1", function(value)
    print("Selected Option:", value)
end)
```

# to create a Slider
```

UILibrary:CreateSlider(section, "Volume", 0, 100, 50, function(value)
    print("Slider Value:", value)
end)
```
