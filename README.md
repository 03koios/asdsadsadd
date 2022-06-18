
writefile("Pog.txt","03.s#6260 ")

for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

local sound = Instance.new("Sound", game.Workspace)
sound.SoundId = "rbxassetid://6958727243"
sound.Looped = false
sound:Play()

local Lib = loadstring(game:HttpGet(("https://raw.githubusercontent.com/03sAlt/Ui/main/README.md"),true))()
Lib.prompt('Discord = 03.s#6260', 'Welcome '  .. game.Players.LocalPlayer.Name, 3)


