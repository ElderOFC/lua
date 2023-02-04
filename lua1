
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Player = game.Players.LocalPlayer
local Window = OrionLib:MakeWindow({Name = "Sistema de Key", HidePremium = true, SaveConfig = true, IntroEnabled = true, IntroText = "Carregando Key...", ConfigFolder = "Key"})

OrionLib:MakeNotification({
    Name = "Logado!",
    Content = "Você está logado como "..Player.Name..".",
    Image = "rbxassetid://4483345998",
    Time = 5
})
OrionLib:MakeNotification({
    Name = "Feita Por Elder#5947!",
    Content = "feita para Kaua",
    Image = "rbxassetid://4483345998",
    Time = 20
})

_G.Key = "4080120" --key
_G.KeyInput = "string"

function MakeScriptHub()
    local Window = OrionLib:MakeWindow({Name = "ElderHub's (_BETA_0.12.1)", HidePremium = true, SaveConfig = true, IntroEnabled = true, IntroText = "Carregando HUB..."})
                -- Outra secção
                local Tab = Window:MakeTab({
                    Name = "Zuar e Farma",
                    Icon = "rbxassetid://4483345998",
                    PremiumOnly = false
                })
                local Section = Tab:AddSection({
                    Name = ":D"
                })
                Tab:AddButton({
                    Name = "Lagar com AURA INTENSA!",
                    Callback = function()
                        _G.settings = {
                            ["LagDupe"] = 2500 -- quantidade de Aura que vai spawnar
                        }
                        
                        local dupe = _G.settings.LagDupe
                        local remote = game:service('ReplicatedStorage'):WaitForChild("RemoteEvent")
                        for i=1,dupe do
                        remote:FireServer({[1] = "Skill_KillingIntent_Start"})
                        remote:FireServer({[1] = "Skill_KillingIntent_End"})
                        end
                      end    
                })
                Tab:AddButton({
                     Name = "Aura de Soul Attack!",
                    Callback = function()
                        
--Soul attack aura basically
local remote = game:service('ReplicatedStorage'):WaitForChild("RemoteEvent")
while wait() do
for i,v in pairs(game.Players:GetPlayers()) do 
remote:FireServer({[1] = "Skill_SoulAttack_Start", [2] = v})
remote:FireServer({[1] = "Skill_SoulAttack_End"})
end
end
                     end   
               })
               Tab:AddButton({
                Name = "Auto Farm Kill (Vilão)!",
               Callback = function()
                --Autofarm for rep lol
_G.settings = {
    ["OnlyDmgVillan"] = false, --leia: true = only damage people with -rep -- true para ganhar reputação boa|||false para ganhar rep má
    ["NotTp"] = "-", --leia: -rep grinding = - , +rep grinding = + .
    ["Wait"] = 15 --leia: tempo pra dar rejoin, se voce nao tomar dano
}
--remotes local do spts
local remote = game:service('ReplicatedStorage'):WaitForChild("RemoteEvent")
remote:FireServer({[1] = "Respawn"})
repeat wait() until game.Players.LocalPlayer.Character ~= nil
wait(5)
--configurações locais
local dmgVillan = _G.settings.OnlyDmgVillan
local wait_time = _G.settings.Wait
local nottp = _G.settings.NotTp
--tp para o jogo(função para ficar dando rejoin)
local Place = 2202352383
local TeleportService = game:GetService("TeleportService")
--printando as funções
local rep = game:GetService("Players").LocalPlayer.PrivateStats.Reputation.Value
print("Sua rep atual = " .. rep)
-- configuração de remotes
remote:FireServer({[1] = "Setting", [2] = "OnlyDmgVillain", [3] = dmgVillan})

--função de spawn para sai em segundos
spawn(function()
wait(wait_time)
TeleportService:Teleport(Place, player)
end)

-- atual autofarm
while true do
game:GetService("RunService").Heartbeat:Wait()
remote:FireServer({[1] = "Skill_SpherePunch", [2] = Vector3.new()}) --spawn de bola de fogo
for i,v in pairs(game.Players:GetPlayers()) do 
    if not v:IsA("Model") then
    if v.Character then
    if v.Character:FindFirstChild("HumanoidRootPart") then
    if not string.find(v.PrivateStats.Reputation.Value, nottp) then
	v.Character.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        if game.Players.LocalPlayer.Character.Humanoid.Health ~= game.Players.LocalPlayer.Character.Humanoid.MaxHealth then 
    TeleportService:Teleport(Place, player)
	end
	end
    end
    end
    end
end
end

                end
               })  
               Tab:AddButton({
                Name = "Auto Farm Kill (Heroi)!",
                Callback = function()
                    --Autofarm for rep lol
_G.settings = {
    ["OnlyDmgVillan"] = true, --leia: true = only damage people with -rep -- true para ganhar reputação boa|||false para ganhar rep má
    ["NotTp"] = "+", --leia: -rep grinding = - , +rep grinding = + .
    ["Wait"] = 15 --leia: tempo pra dar rejoin, se voce nao tomar dano
}
--remotes local do spts
local remote = game:service('ReplicatedStorage'):WaitForChild("RemoteEvent")
remote:FireServer({[1] = "Respawn"})
repeat wait() until game.Players.LocalPlayer.Character ~= nil
wait(5)
--configurações locais
local dmgVillan = _G.settings.OnlyDmgVillan
local wait_time = _G.settings.Wait
local nottp = _G.settings.NotTp
--tp para o jogo(função para ficar dando rejoin)
local Place = 2202352383
local TeleportService = game:GetService("TeleportService")
--printando as funções
local rep = game:GetService("Players").LocalPlayer.PrivateStats.Reputation.Value
print("Sua rep atual = " .. rep)
-- configuração de remotes
remote:FireServer({[1] = "Setting", [2] = "OnlyDmgVillain", [3] = dmgVillan})

--função de spawn para sai em segundos
spawn(function()
wait(wait_time)
TeleportService:Teleport(Place, player)
end)

-- atual autofarm
while true do
game:GetService("RunService").Heartbeat:Wait()
remote:FireServer({[1] = "Skill_SpherePunch", [2] = Vector3.new()}) --spawn de bola de fogo
for i,v in pairs(game.Players:GetPlayers()) do 
    if not v:IsA("Model") then
    if v.Character then
    if v.Character:FindFirstChild("HumanoidRootPart") then
    if not string.find(v.PrivateStats.Reputation.Value, nottp) then
	v.Character.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        if game.Players.LocalPlayer.Character.Humanoid.Health ~= game.Players.LocalPlayer.Character.Humanoid.MaxHealth then 
    TeleportService:Teleport(Place, player)
	end
	end
    end
    end
    end
end
end

                  end    
            })
end

function CorrectKeyNotification()
    OrionLib:MakeNotification({
        Name = "Key Válida!",
        Content = "Pronto, zé ruela!",
        Image = "rbxassetid://4483345998",
        Time = 5
    })
    OrionLib:MakeNotification({
        Name = "RECADO",
        Content = "JÁ PODE FECHAR A KEY HUB",
        Image = "rbxassetid://4483345998",
        Time = 3
    })
end

function IncorrectKeyNotification()
    OrionLib:MakeNotification({
        Name = "Key Inválida!",
        Content = "Animal do caralho, sabe fazer isso não?!",
        Image = "rbxassetid://4483345998",
        Time = 5
    })
end

local Tab = Window:MakeTab({
    Name = "Key",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

Tab:AddTextbox({
    Name = "Coloque a Key",
    Default = "",
    TextDisappear = true,
    Callback = function(value)
        _G.KeyInput = value
    end
})

Tab:AddButton({
    Name = "Clica aqui agora!",
    Callback = function()
        if _G.KeyInput == _G.Key then
            MakeScriptHub()
            CorrectKeyNotification()
            else
                IncorrectKeyNotification()
        end
    end
})

OrionLib:Init()
