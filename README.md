-- init
local library = loadstring(game:HttpGet("https://gist.githubusercontent.com/koio08199za/5121bfa15c12af9e0dc3ab23745213e5/raw/5e509dc9291b4250cec7f4af79d7c3229c9bac13/Test"))()
local venyx = library.new("HACKNOOB Hub Saber Simulator ", 5013109572)
-- themes
local themes = {
Background = Color3.fromRGB(24, 24, 24),
Glow = Color3.fromRGB(0, 165, 248),
Accent = Color3.fromRGB(10, 10, 10),
LightContrast = Color3.fromRGB(20, 20, 20),
DarkContrast = Color3.fromRGB(14, 14, 14),
TextColor = Color3.fromRGB(0, 183, 255)
}

local page = venyx:addPage("Menu", 5012544693)
local section1 = page:addSection("Credit: HACKNOOB Hub")
local section1 = page:addSection("Discordt: 03s#4358")
local page = venyx:addPage("Auto Farm", 5012544693)
local section2 = page:addSection("Farm")
section2:addToggle("Auto Farm", nil, function(value)
    _G.autoTep = value;
while _G.autoTep == true do
    pcall(function()
game:GetService("ReplicatedStorage").Events.Clicked:FireServer()
wait()
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
if v.ClassName == "Tool" then
    game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
    wait()
end)
end
end
end
end)
section2:addToggle("Auto Sell", nil, function(value)
    _G.autosell = value;
while _G.autosell == true do
    pcall(function()
game:GetService("ReplicatedStorage").Events.Sell:FireServer()
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(530.238342, 183.535995, 149.377792, -0.898786724, -3.59346544e-08, -0.438386172, 1.45196646e-08, 1, -1.11738785e-07, 0.438386172, -1.06794552e-07, -0.898786724)
    end)
end
end)
section2:addToggle("AutoBuy Saber", nil, function(value)
    _G.autoSword = value;
    while _G.autoSword == true do
        pcall(function()
    local args = {[1] = "Swords"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait(2)
        end)
end
end)
section2:addToggle("AutoBuy DNA", nil, function(value)
    _G.autoPack = value;
while _G.autoPack == true do
    pcall(function()
local args = {[1] = "Backpacks"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait()
    end)
end
end)
section2:addToggle("AutoBuy Class", nil, function(value)
    _G.autoClass = value;
while _G.autoClass do wait()
    pcall(function()
    for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Gui.Submenus.Shop.ClassesFrame.Frame:GetChildren()) do
        if v.ClassName == "ImageButton" then
    local args = {[1] = game:GetService("ReplicatedStorage").ShopItems.Classes[tostring(v.Name)]}
    game:GetService("ReplicatedStorage").Events.BuyItem:FireServer(unpack(args))
    end
    end
end)
end
end)
local section2 = page:addSection("Crown")
section2:addToggle("Auto Crown", nil, function(value)
    _G.autoCrown = value;
    while _G.autoCrown == true do
        pcall(function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(792.52819824219, 249.47679138184, 31.638505935669))
wait()
        end)
end
end)
local section2 = page:addSection("Skill")
section2:addToggle("AutoBuy Jump", nil, function(value)
     _G.autoboots = value;
while _G.autoboots == true do 
    pcall(function()
local args = {[1] = "JumpBoosts"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait()
end)
end
end)
section2:addToggle("AutoBuy BOSSHIT", nil, function(value)
    _G.autoBOSS = value;
while _G.autoBOSS == true do 
    pcall(function()
local args = {[1] = "BossBoosts"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait()
end)
end
end)
local page = venyx:addPage("Teleport", 5012544693)
local section3 = page:addSection("Ilsand")
section3:addButton("Button", function()

