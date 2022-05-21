
writefile("Pog Hub Key.txt","Pog")

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


game.StarterGui:SetCore("SendNotification", {
Title = "Credits : 03.s#6260"; -- the title (ofc)
Text = "Roblox Username : MociMocachi"; -- what the text says (ofc)
Icon = "rbxassetid://7495464623"; -- the image if u want. 
Duration = 5; -- how long the notification should in secounds
})


    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "Command Game Universal";
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
	Text = "/e Btools";
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

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Position";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})

    bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "/e Jump";
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

            elseif Msg == "/e Position" then
        setclipboard(tostring(game.Players.LocalPlayer.Character.HumanoidRootPart.Position))
        
                    elseif Msg == "/e Jump" then
        local infiniteJumpButton = Instance.new("TextButton")
local function setInfinityJumpButton()
    local script = Instance.new("LocalScript", infiniteJumpButton)

    infiniteJumpButton.Parent = tab_1
    infiniteJumpButton.Name = "infinityJumpButton"
    infiniteJumpButton.Text = "Infinity Jump [V]"
    infiniteJumpButton.TextScaled = true
    infiniteJumpButton.Font = Enum.Font.Ubuntu
    infiniteJumpButton.BackgroundColor3 = Color3.new(1, 0, 0)
    infiniteJumpButton.Position = UDim2.new(0, 10, 0, 190)
    infiniteJumpButton.Size = UDim2.new(0.9, 0, 0.05, 0)
    infiniteJumpButton.BorderColor3 = Color3.new(1, 1, 1)

    local Mouse = game.Players.LocalPlayer:GetMouse()
    local InfiniteJump = false

    script.Parent.MouseButton1Click:Connect(function()
        if InfiniteJump == false then
            InfiniteJump = true
            script.Parent.BackgroundColor3 = Color3.fromRGB(0, 255, 0)
        else
            InfiniteJump = false
            script.Parent.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
        end
    end)

    Mouse.KeyDown:Connect(function(k)
        if k == "v" then
            if InfiniteJump == false then
                InfiniteJump = true
                script.Parent.BackgroundColor3 = Color3.fromRGB(0, 255, 0)
            else
                InfiniteJump = false
                script.Parent.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
            end
        end
    end)

    game:GetService("UserInputService").JumpRequest:Connect(function()
        if InfiniteJump == true then
            game:GetService "Players".LocalPlayer.Character:FindFirstChildOfClass 'Humanoid'
                :ChangeState("Jumping")
        end
    end)
end
coroutine.wrap(setInfinityJumpButton)()
            bc = BrickColor.new("Green")
game.StarterGui:SetCore("ChatMakeSystemMessage", {
	Text = "InfiniteJump Settings Toggle : V";
	Font = Enum.Font.Cartoon;
	Color = bc.Color;
	FontSize = Enum.FontSize.Size11;	
})
        
      end
  end)
