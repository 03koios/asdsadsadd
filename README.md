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

wait(4)
game.StarterGui:SetCore("SendNotification", {
Title = "Key Saved"; 
Text = "Your Key is Save Workspace in Your Executor File"; 
Icon = "rbxassetid://7495464623";
Duration = 3; 
})

