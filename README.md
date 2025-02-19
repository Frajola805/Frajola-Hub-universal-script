local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

 local Window = Fluent:CreateWindow({
    Title = "Frajola Hub" .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

 local Tabs = {
    Main = Window:AddTab({ Title = "Main" }),
}

 Fluent:Notify({ Title = "Notificação", Content = "FrajolaHub Executado!" })
 
 Fluent:Notify({ Title = "Aviso", Content = "Acesse meu Discord!" })

Tabs.Main:AddButton({ Title = "HitBox", Callback = function()loadstring(game:HttpGet(('https://pastebin.com/raw/TgWmJEaC'),true))()end })

Tabs.Main:AddButton({ Title = "Esp", Callback = function()loadstring(game:HttpGet('https://raw.githubusercontent.com/Lucasfin000/SpaceHub/main/UESP'))()end })

Tabs.Main:AddButton({ Title = "Inf Jump", Callback = function()local InfiniteJumpEnabled = true
game:GetService("UserInputService").JumpRequest:connect(function()
	if InfiniteJumpEnabled then
		game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")
	end
end)end })

Tabs.Main:AddButton({ Title = "No cooldown", Callback = function()g = hookfunction(wait, function(seconds)
return g(0)
end)end })
