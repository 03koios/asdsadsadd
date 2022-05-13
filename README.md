wait(1)
game.StarterGui:SetCore("SendNotification", {
Title = "AFK!"; 
Text = "Anti AFK!"; 
Icon = "http://www.roblox.com/asset/?id=9614226681";
Duration = 5; 
})
for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

wait(1)
local bindable = Instance.new("BindableFunction")
function bindable.OnInvoke(response)
	print("else")
	setclipboard("https://discord.gg/x4gGhjVxXz")
end
game:GetService("StarterGui"):SetCore("SendNotification", {
	Title = "Discord Server",
	Icon = "http://www.roblox.com/asset/?id=9614208528"; -- the image if u want. 
	Text = "https://discord.gg/x4gGhjVxXz",
	Duration = 69420,
	Callback = bindable,
	Button1 = "Copy"
})
