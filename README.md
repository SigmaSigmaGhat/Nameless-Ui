# Nameless UI - Documentation

## Introduction
Nameless UI is a lightweight and customizable UI library for Roblox, designed to provide essential UI elements like buttons, toggles, sliders, and text boxes. It allows developers to create functional user interfaces with minimal effort.

## Features
- Create a draggable UI window
- Add buttons with click events
- Add toggles with on/off states
- Add sliders with adjustable values
- Add text boxes for user input

## Getting Started
### Loading the Library
To use Nameless UI, load it into your script:
```lua
local NamelessUI = loadstring(game:HttpGet("https://pastebin.com/raw/CjERaBhL",true))()
```

### Creating a UI Window
```lua
local Window = NamelessUI:CreateWindow("My UI")
```
This creates a new draggable window with the given title.

## UI Elements
### Adding a Button
```lua
Window:AddButton("Click Me", function()
    print("Button Clicked!")
end)
```
This adds a button labeled "Click Me" that prints a message when clicked.

### Adding a Toggle
```lua
Window:AddToggle("Enable Feature", function(state)
    print("Toggle is now", state and "ON" or "OFF")
end)
```
This creates a toggle switch that calls the function with `true` or `false` depending on its state.

### Adding a Slider
```lua
Window:AddSlider("Volume", 0, 100, function(value)
    print("Volume set to:", value)
end)
```
Creates a slider with a range of `0` to `100`, triggering a function when changed.

### Adding a Text Box
```lua
Window:AddTextBox("Enter Name", function(text)
    print("Entered text:", text)
end)
```
Creates a text box that calls a function with the entered text when the user presses enter.

## Conclusion
Nameless UI simplifies UI creation for Roblox games. You can customize and expand it to fit your needs. If you need more features, feel free to modify the script!

