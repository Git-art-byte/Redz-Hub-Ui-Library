# Redz-Hub-Ui-Library

## Library
```lua
local YourLibraryName = loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/RedzLibV5/main/Source.Lua"))()
```

## Window
```lua
local Window = YourLibraryName:MakeWindow({
  Title = "Title",
  SubTitle = "by YourName",
  SaveFolder = "FolderName"
})
```

## Tabs
```lua
local Tab1 = Window:MakeTab({"TabName", "lucideIcon"})
```

## Buttons
```lua
Tab1:AddButton({"ButtonName", function()
  print("Hello World")
end})
```

## Switching Tabs
```lua
Window:SelectTab(Tab1)
```

## Sections
```lua
local Section = Tab1:AddSection({"SectionName"})
```

## Paragraphs
```lua
local Paragraph = Tab1:AddParagraph({"ParagraphName", "This is a Paragraph."})
```

## Toogles
```lua
local Toggle1 = Tab1:AddToggle({
    Name = "Toggle 1",
    Default = false,
    Callback = function(Value)
        print("Toggle 1 state:", Value)
    end
})
```

## Sliders
```lua
Tab1:AddSlider({
  Name = "SliderName",
  Min = 1,
  Max = 10,
  Increase = 1,
  Default = 16,
  Callback = function(Value)
    game.Players.LocalPlayer.Charcater.Humanoid.WalkSpeed = Value
  end
})
```

## Dropdowns
```lua
local DropdownName = Tab1:AddDropdown({
  Name = "Dropdown",
  Options = {"one", "two", "three"},
  Default = "one",
  Callback = function(Value)
    print(Value)
  end
})
```
