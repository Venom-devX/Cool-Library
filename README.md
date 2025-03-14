## Library
```lua
local CoolLibrary = loadstring(game:HttpGet("https://raw.githubusercontent.com/Venom-devX/Cool-Library/refs/heads/main/CoolLibrarySource.lua"))()
```
## Creating A Window
```lua
local Window = CoolLibrary:Window("White Title", "Blue Title", "rbxassetid://166652117")
--[[
White Title - Strimg;
Blue Title - String;
Image - RbxAssetId
]]--
```
## Making a Tab
```lua
local Tabs = {
    MainTab = Window:Tab("Main Tab");
    Settings = Window:Tab("Settings Tab");
}
--[[
You also can use:
local Tab = Window:Tab("Tab")
]]--
```
## Making a Section (Mandatory)
```lua
local Section = Tab:Section("It's a section!")
```
## Making a Button
```lua
Section:Button("It's a button!", function()
    print("Hello, World")
end) -- Format: Title, Callback
```
## Making a Toggle
```lua
local Toggle = Section:Toggle("Press this toggle!", function(Value)
    print(Value)
end) -- Format: Title, Callback
```
## Creating a Input Box
```lua
Section:Box("Put something here.", function(Value)
    print(Value) -- Print that has been writen in the box
end) -- Format: Title, Callback
```
## Creating Text Label
```lua
Section:Label("Its a text label") -- Text
```
## Creating a Picker
```lua
Section:Picker("Example Picker", {"Teste", "......"}, function(Value)
    print(Value)
end) -- Format: Title, Options, Callback
```
