wait(1)
game.StarterGui:SetCore("SendNotification", {
Title = "AFK!"; -- the title (ofc)
Text = "Anti AFK!"; -- what the text says (ofc)
Icon = "http://www.roblox.com/asset/?id=9460726644";
Duration = 5; 
})
for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

wait(1)
game.StarterGui:SetCore("SendNotification", {
Title = "Credit : 03.s#6260";
Text = "Credit : 03.s#6260"; -- what the text says (ofc)
Icon = "http://www.roblox.com/asset/?id=9460726644"; 
Duration = 5; 
})
