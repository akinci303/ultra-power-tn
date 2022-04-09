local library = loadstring(game:HttpGet(('https://raw.githubusercontent.com/AikaV3rm/UiLib/master/Lib.lua')))()
local plrhead = game.Players.LocalPlayer.Character.Head


local uimain = library:CreateWindow("Ultra Power Tycoon")


local woodmaster = uimain:CreateFolder("Wood Master Tycoon")


woodmaster:Button("Get Wood Master",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Get Wood Master"].Door["ActDoor"], 0)
end)

woodmaster:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Wood Master"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

woodmaster:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Wood Master"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

woodmaster:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Wood Master"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

woodmaster:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Wood Master"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local push = uimain:CreateFolder("Push Tycoon")


push:Button("Get Push",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Push.Door["ActDoor"], 0)
end)

push:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons.Push.CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

push:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons.Push:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

push:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons.Push:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

push:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons.Push.Spawn.CFrame * CFrame.new(0,5,0)
end)



local rage = uimain:CreateFolder("Rage Tycoon")


rage:Button("Get Rage",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Rage.Door["ActDoor"], 0)
end)

rage:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Rage"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

rage:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Rage"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

rage:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Rage"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

rage:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Rage"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local eternal = uimain:CreateFolder("Eternal Tycoon")


eternal:Button("Get Eternal",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Eternal.Door["ActDoor"], 0)
end)

eternal:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Eternal"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

eternal:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Eternal"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

eternal:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Eternal"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

eternal:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Eternal"].Spawn.CFrame * CFrame.new(0,5,0)
end)


local sandlord = uimain:CreateFolder("Sand Lord Tycoon")

sandlord:Button("Get Sand Lord",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Sand Lord"].Door["ActDoor"], 0)
end)

sandlord:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sand Lord"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

sandlord:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sand Lord"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

sandlord:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sand Lord"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

sandlord:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Sand Lord"].Spawn.CFrame * CFrame.new(0,5,0)
end)


local deatheye = uimain:CreateFolder("Death Eye Tycoon")

deatheye:Button("Get Death Eye",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Death Eye"].Door["ActDoor"], 0)
end)

deatheye:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Death Eye"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

deatheye:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Death Eye"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

deatheye:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Death Eye"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

deatheye:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Death Eye"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local darkflame = uimain:CreateFolder("Dark Flame Tycoon")

darkflame:Button("Get Dark Flame",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons["Dark Flame"].Door["ActDoor"], 0)
end)

darkflame:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark Flame"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

darkflame:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark Flame"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

darkflame:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Dark Flame"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

darkflame:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Dark Flame"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local sneak = uimain:CreateFolder("Sneak Tycoon")


sneak:Button("Get Sneak",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Sneak.Door["ActDoor"], 0)
end)


sneak:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sneak"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

sneak:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sneak"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

sneak:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Sneak"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

sneak:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Sneak"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local cursed = uimain:CreateFolder("Cursed Tycoon")


cursed:Button("Get Cursed",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Cursed.Door["ActDoor"], 0)
end)

cursed:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Cursed"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

cursed:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Cursed"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

cursed:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Cursed"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

cursed:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Cursed"].Spawn.CFrame * CFrame.new(0,5,0)
end)



local tailed = uimain:CreateFolder("Tailed Tycoon")


tailed:Button("Get Tailed",function()
    firetouchinterest(plrhead, game.Workspace.Tycoons.Tailed.Door["ActDoor"], 0)
end)

tailed:Toggle("Cash AutoGrab",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.2) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Tailed"].CashRegister.Ching:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end
            end
        end
    end
end)

tailed:Button("Get All My Tools",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons["Tailed"]:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

tailed:Toggle("AutoBuy",function(bool)
    shared.toggle = bool
    if shared.toggle == true then
        while wait(.5) do
            if shared.toggle == false then break end
        for i,v in pairs(game:GetService("Workspace").Tycoons["Tailed"]:GetDescendants()) do
             if v.Name == "TouchInterest" and v.Parent then
                if v.Parent.Parent.Name ~= "Robux1" then
                if v.Parent.Parent.Name ~= "Robux2" then
                if v.Parent.Name ~= "Ching" then
                if v.Parent.Parent.Name ~= "LegendaryGear" then
                if v.Parent.Parent.Name ~= "VoidShield" then 
                if v.Parent.Parent.Name ~= "ShopModel" then
                    firetouchinterest(plrhead, v.Parent, 0)
                    wait(0.01)
                    firetouchinterest(plrhead, v.Parent, 1)
                end end end end end end
                end
            end
        end
    end
end)

tailed:Button("TP to Spawn",function()
    plrhead.Parent.HumanoidRootPart.CFrame = game:GetService("Workspace").Tycoons["Tailed"].Spawn.CFrame * CFrame.new(0,5,0)
end)

local others = uimain:CreateFolder("Others")
others:Button("Get All Tools [LOADED!]",function()
        for i,v in pairs(game:GetService("Workspace").Tycoons:GetDescendants()) do
            if v.Name == "TouchInterest" and v.Parent.Name == "Neon"  then
            firetouchinterest(plrhead, v.Parent, 0)
            wait(0.01)
            firetouchinterest(plrhead, v.Parent, 1)
         end
     end
end)

others:Label("Credit to Muzan QLTN",{
    TextSize = 20; -- Self Explaining
    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining
    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining
    
})
others:Label("(me) youtube",{
    TextSize = 20; -- Self Explaining
    TextColor = Color3.fromRGB(255,255,255); -- Self Explaining
    BgColor = Color3.fromRGB(69,69,69); -- Self Explaining
    
})
