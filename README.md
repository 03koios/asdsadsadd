
writefile("Credits Pog Hub No Carte.txt","Scripter : 03.s#6260 Scripter : Lura#0001 Discord Server : discord.gg/x4gGhjVxXz ")

for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end


game.StarterGui:SetCore("SendNotification", {
Title = "Welcome User"; -- the title (ofc)
Text = game.Players.LocalPlayer.Name; -- what the text says (ofc)
Icon = "https://www.roblox.com/headshot-thumbnail/image?userId=".. game.Players.LocalPlayer.UserId .."&width=420&height=420&format=png"; -- the image if u want. 
Duration = 5; -- how long the notification should in secounds
})

