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
end
end
end)
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
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(792.52819824219, 249.47679138184, 31.638505935669)
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
section3:addButton("Unlock All", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(501.43447875977, 797.22155761719, 233.96742248535)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(493.88360595703, 2650.8940429688, -357.01654052734)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(700.10186767578, 7089.8540039063, -328.60140991211)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(535.51110839844, 12695.860351563, -237.52551269531)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(543.59429931641, 19436.8984375, -47.553916931152)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(473.58026123047, 26254.3984375, -133.68225097656)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(627.72784423828, 29798.0546875, -26.740255355835)
wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(513.59710693359, 34166.8515625, -158.81550598145)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(609.28125, 38091.95703125, -152.38940429688)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(613.24060058594, 42885.95703125, -219.48497009277)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(633.80181884766, 48846.71875, -233.45980834961)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(539.70989990234, 52640.71875, -217.66375732422)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(540.12780761719, 57624.61328125, -221.39779663086)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(536.89361572266, 62380.625, -225.09158325195)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(538.55456542969, 67085.1796875, -201.17495727539)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(537.46313476563, 72949.2578125, -206.78591918945)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(545.72357177734, 76588.265625, -42.710189819336)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(535.71264648438, 80721.9609375, -50.781688690186)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(517.35900878906, 84819.9921875, -44.044727325439)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(515.28570556641, 90387.3828125, -39.062633514404)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(519.97741699219, 94250.078125, -45.891048431396)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(529.5263671875, 97709.7109375, -40.480838775635)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(526.43035888672, 101246.671875, -45.212100982666)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(605.72137451172, 104245.0390625, -163.57717895508)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(630.11297607422, 108784.4375, -26.313400268555)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(645.84484863281, 113359.8515625, -26.033536911011)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(634.23620605469, 117956.8125, -26.058280944824)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(633.41461181641, 121861.8125, -24.641689300537)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(635.37127685547, 127917.8515625, -25.07767868042)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(764.36633300781, 131086.203125, -62.47240447998)
wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(635.46569824219, 135605.03125, -174.80101013184)
end)
section3:addButton("TPIlsand", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(531.9443359375, 185.84199523926, -37.957084655762)
end)
    local theme = venyx:addPage("Misc", 5012544693)
    local colors = theme:addSection("Keybind")
    colors:addKeybind("Toggle Keybind", Enum.KeyCode.RightControl, function()
    print("Activated Keybind")
    venyx:toggle()
    end, function()
    print("Changed Keybind")
    end)
    local colors = theme:addSection("Colors")
    
    for theme, color in pairs(themes) do -- all in one theme changer, i know, im cool
    colors:addColorPicker(theme, color, function(color3)
    venyx:setTheme(theme, color3)
end)
end
