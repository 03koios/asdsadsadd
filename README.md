writefile("Pog Hub Key.txt","Pog")

for i,v in pairs(getconnections(game.Players.LocalPlayer.Idled)) do
v:Disable()
end

local bindable = Instance.new("BindableFunction")
function bindable.OnInvoke(response)
	print("else")
	setclipboard("https://discord.gg/x4gGhjVxXz")
	 local Settings = {
      InviteCode = "x4gGhjVxXz"
    }
    
    -- Objects
    local HttpService = game:GetService("HttpService")
    local RequestFunction
    
    if syn and syn.request then
      RequestFunction = syn.request
    elseif request then
      RequestFunction = request
    elseif http and http.request then
      RequestFunction = http.request
    elseif http_request then
      RequestFunction = http_request
    end
    
    local DiscordApiUrl = "http://127.0.0.1:%s/rpc?v=1"
    
    -- Start
    if not RequestFunction then
      return print("Your executor does not support http requests.")
    end
    
    for i = 6453, 6464 do
      local DiscordInviteRequest = function()
          local Request = RequestFunction({
              Url = string.format(DiscordApiUrl, tostring(i)),
              Method = "POST",
              Body = HttpService:JSONEncode({
                  nonce = HttpService:GenerateGUID(false),
                  args = {
                      invite = {code = Settings.InviteCode},
                      code = Settings.InviteCode
                  },
                  cmd = "INVITE_BROWSER"
              }),
              Headers = {
                  ["Origin"] = "https://discord.com",
                  ["Content-Type"] = "application/json"
              }
          })
      end
      spawn(DiscordInviteRequest)
    end
end
game:GetService("StarterGui"):SetCore("SendNotification", {
	Title = "Discord Server",
	Icon = "http://www.roblox.com/asset/?id=9614208528"; -- the image if u want. 
	Text = "Discord Server Copy Link?",
	Duration = 2,
	Callback = bindable,
	Button1 = "Join / Copy"
})


game.StarterGui:SetCore("SendNotification", {
Title = "Credits : 03.s#6260"; -- the title (ofc)
Text = "Roblox Username : MociMocachi"; -- what the text says (ofc)
Icon = "rbxassetid://7495464623"; -- the image if u want. 
Duration = 5; -- how long the notification should in secounds
})


    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "Command";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Credits";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e ResetAvatar";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Teleport Tool";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Reload Script";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Fly";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

game:GetService("Players").LocalPlayer.Chatted:Connect(function(Msg)
    local RepStorage = game:GetService("ReplicatedStorage")
    local RepEvents = RepStorage:FindFirstChild("RemoteEvents")
    -- Tool-Controls
    if Msg == "/e Credits" then
    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "Discord : 03.s#6260 Discord Server discord.gg/x4gGhjVxXz";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})
    elseif Msg == "/e ResetAvatar" then
        game.Players.LocalPlayer.character:WaitForChild("Humanoid").Health = 0

    elseif Msg == "/e Teleport Tool" then
        mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = "Teleport Tool 03.s#6260"
tool.Activated:connect(function()
local pos = mouse.Hit+Vector3.new(0,2.5,0)
pos = CFrame.new(pos.X,pos.Y,pos.Z)
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos
end)
tool.Parent = game.Players.LocalPlayer.Backpack

    elseif Msg == "/e Reload Script" then
        loadstring(game:HttpGet("https://raw.githubusercontent.com/03sAlt/discord.gg-x4gGhjVxXz/main/Loader.lua"))()
        
            elseif Msg == "/e Btools" then
        Instance.new("HopperBin", game.Players.LocalPlayer.Backpack).BinType = 2
Instance.new("HopperBin", game.Players.LocalPlayer.Backpack).BinType = 3
Instance.new("HopperBin", game.Players.LocalPlayer.Backpack).BinType = 4

    elseif Msg == "/e Fly" then
            bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "Fly Settings Toggle : LeftAlt";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})
loadstring(game:HttpGet("https://raw.githubusercontent.com/03sAlt/fly/main/README.md"))()
      end
  end)
