_G.autoTep = false;
while _G.autoTep == true do 
game:GetService("ReplicatedStorage").Events.Clicked:FireServer()
wait()
game:GetService("ReplicatedStorage").Events.Sell:FireServer()
wait()
local args = {[1] = "Swords"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait()
local args = {[1] = "Backpacks"}
game:GetService("ReplicatedStorage").Events.BuyAll:FireServer(unpack(args))
wait()
local args = {[1] = game:GetService("ReplicatedStorage").ShopItems.Classes.Paladin}
game:GetService("ReplicatedStorage").Events.BuyItem:FireServer(unpack(args))
wait()
end
