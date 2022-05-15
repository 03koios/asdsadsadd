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


wait(3)
game.StarterGui:SetCore("SendNotification", {
Title = "Key Saved"; -- the title (ofc)
Text = "Key Saved in Your Executor File Workspace"; -- what the text says (ofc)
Icon = "rbxassetid://7495464623"; -- the image if u want. 
Duration = 5; -- how long the notification should in secounds
})
