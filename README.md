 local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()
local win = DiscordLib:Window("DH FAMILY")
local serv = win:Server("DH FAMILY", "")
local btns = serv:Channel("จุดพักใจ")
btns:Button("จุดเกิด", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-964.436218, 45.0011711, -249.601303, 0.0199616645, 6.38246433e-09, -0.999800742, 1.07542686e-09, 1, 6.40520792e-09, 0.999800742, -1.2030712e-09, 0.0199616645)
end)
btns:Button("ปาบอล", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-872.810791, 45.0586815, -150.200668, -1, -5.8495452e-08, -8.85501595e-06, -5.84958464e-08, 1, 4.45712303e-08, 8.85501595e-06, 4.4571749e-08, -1)
end)
btns:Button("สะพาน", function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-809.131287, 44.9417992, -307.303528, -0.017433729, -5.81190598e-08, -0.999848008, -6.3616767e-08, 1, -5.70186494e-08, 0.999848008, 6.26130543e-08, -0.017433729)
end)
local tgls = serv:Channel("AITI-AFK")
tgls:Toggle("AFK-ไม่มีหลุด",false, function(bool)
local args = {
    [1] = false}game:GetService("Players").LocalPlayer.Character.Head.OverHeadAttach.OverHeadGui.Frame.AFK:FireServer(unpack(args))
end)
