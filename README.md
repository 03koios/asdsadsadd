for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

local bindable = Instance.new("BindableFunction")
function bindable.OnInvoke(response)
	print("else")
	setclipboard("https://discord.gg/x4gGhjVxXz")
end
game:GetService("StarterGui"):SetCore("SendNotification", {
	Title = "Discord Server",
	Icon = "http://www.roblox.com/asset/?id=9614208528"; -- the image if u want. 
	Text = "Discord Server Copy Link?",
	Duration = 2,
	Callback = bindable,
	Button1 = "Copy"
})

local bindable = Instance.new("BindableFunction")
function bindable.OnInvoke(response)
	print("else")
	setclipboard("https://web.roblox.com/groups/14396486/Pog-Hub-No-Carte-Fan-Club#!/about")
end
game:GetService("StarterGui"):SetCore("SendNotification", {
	Title = "Whitelist",
	Icon = "rbxassetid://7495464623"; -- the image if u want. 
	Text = "Roblox Group Whitelist Only",
	Duration = 65464,
	Callback = bindable,
	Button1 = "Copy Roblox Group"
})
