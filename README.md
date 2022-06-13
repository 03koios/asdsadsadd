
writefile("Credits Pog Hub No Carte.txt","Scripter : 03.s#6260 Scripter : Lura#0001 Discord Server : discord.gg/x4gGhjVxXz ")

for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

local sound = Instance.new("Sound", game.Workspace)
sound.SoundId = "rbxassetid://6958727243"
sound.Looped = false
sound:Play()

local Notification = loadstring(game:HttpGet("https://raw.githubusercontent.com/03sAlt/tHEE/main/README.md"))()

Notification.Notify("Welcome User", game.Players.LocalPlayer.Name, "https://www.roblox.com/headshot-thumbnail/image?userId=".. game.Players.LocalPlayer.UserId .."&width=420&height=420&format=png", {
Duration = 10,       
Main = {
    Rounding = true,
}
});

