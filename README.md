local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "monke hub", HidePremium = false, IntroText = "monke hub", SaveConfig = true, ConfigFolder = "OrionTest"})

local PlayerVals = Window:MakeTab({
	Name = "Player Values",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

PlayerVals:AddSlider({
	Name = "WalkSpeed",
	Min = 16,
	Max = 500,
	Default = 5,
	Color = Color3.fromRGB(168,50,50),
	Increment = 1,
	ValueName = "WS",
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
	end    
})

PlayerVals:AddSlider({
	Name = "JumpPower",
	Min = 50,
	Max = 500,
	Default = 5,
	Color = Color3.fromRGB(168,50,50),
	Increment = 1,
	ValueName = "Height",
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value
	end    
})

PlayerVals:AddButton({
	Name = "Noclip",
	Callback = function()
      		loadstring(game:HttpGet("https://raw.githubusercontent.com/monkeyfaggot167/monkehub/refs/heads/main/monkehub"))();
  	end    
})

local Basic = Window:MakeTab({
	Name = "Basic",
	Icon = "rbxassetid://9267089525",
	PremiumOnly = false
})

Basic:AddLabel("Here you Will find scripts that are simple too find.")

Basic:AddButton({
	Name = "Infinite Yield",
	Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
  	end    
})

Basic:AddButton({
	Name = "Aimbot",
	Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/monkeyfaggot167/monkehub/refs/heads/main/aimbot"))()
  	end    
})

Basic:AddButton({
	Name = "LagSwitch",
	Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/ceM63GsX"))()
  	end    
})

PlayerVals:AddButton({
	Name = "ChatSpy",
	Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/xURZB8e7"))()
  	end    
})

PlayerVals:AddButton({
	Name = "PositionFinder",
	Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/monkeyfaggot167/monkehub/refs/heads/main/pos%20finder"))()
  	end    
})
