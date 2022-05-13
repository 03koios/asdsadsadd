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
	Text = "Discord Server Copy Link?",
	Duration = 69420,
	Callback = bindable,
	Button1 = "Copy"
})


wait(1)
game.StarterGui:SetCore("SendNotification", {
Title = "Support Executor"; 
Text = "Krnl Synapse Script Ware And More"; 
Icon = "http://www.roblox.com/asset/?id=9615044335";
Duration = 5; 
})
