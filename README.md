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


wait(5)
game.StarterGui:SetCore("SendNotification", {
Title = "Credits : 03.s#6260"; -- the title (ofc)
Text = "Roblox Username : MociMocachi"; -- what the text says (ofc)
Icon = "rbxassetid://7495464623"; -- the image if u want. 
Duration = 5; -- how long the notification should in secounds
})
