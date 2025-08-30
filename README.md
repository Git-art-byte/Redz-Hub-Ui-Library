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
