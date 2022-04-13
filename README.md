local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("KUY PH*M", "BloodTheme")




local Tab = Window:NewTab("main")

local Section = Tab:NewSection("fram rejoin for stop")
Section:NewToggle("fram", "Click to use fram", function(state)
while wait () do
local plr = game:service"Players".LocalPlayer;
local tween_s = game:service"TweenService";
local info = TweenInfo.new(2,Enum.EasingStyle.Quad);
function tp(...)
   local tic_k = tick();
   local params = {...};
   local cframe = CFrame.new(params[1],params[2],params[3]);
   local tween,err = pcall(function()
       local tween = tween_s:Create(plr.Character["HumanoidRootPart"],info,{CFrame=cframe});
       tween:Play();
   end)
   if not tween then return err end
end
tp(-55.1682892, 71.8159409, 1298.73474);

wait (2)

local plr = game:service"Players".LocalPlayer;
local tween_s = game:service"TweenService";
local info = TweenInfo.new(20,Enum.EasingStyle.Quad);
function tp(...)
   local tic_k = tick();
   local params = {...};
   local cframe = CFrame.new(params[1],params[2],params[3]);
   local tween,err = pcall(function()
       local tween = tween_s:Create(plr.Character["HumanoidRootPart"],info,{CFrame=cframe});
       tween:Play();
   end)
   if not tween then return err end
end
tp(-89.9058228, 35.5401726, 8445.28516);

wait (18)

local plr = game:service"Players".LocalPlayer;
local tween_s = game:service"TweenService";
local info = TweenInfo.new(3,Enum.EasingStyle.Quad);
function tp(...)
   local tic_k = tick();
   local params = {...};
   local cframe = CFrame.new(params[1],params[2],params[3]);
   local tween,err = pcall(function()
       local tween = tween_s:Create(plr.Character["HumanoidRootPart"],info,{CFrame=cframe});
       tween:Play();
   end)
   if not tween then return err end
end
tp(-75.2286987, 45.7501411, 9307.02344);

wait (3)

local plr = game:service"Players".LocalPlayer;
local tween_s = game:service"TweenService";
local info = TweenInfo.new(8,Enum.EasingStyle.Quad);
function tp(...)
   local tic_k = tick();
   local params = {...};
   local cframe = CFrame.new(params[1],params[2],params[3]);
   local tween,err = pcall(function()
       local tween = tween_s:Create(plr.Character["HumanoidRootPart"],info,{CFrame=cframe});
       tween:Play();
   end)
   if not tween then return err end
end
tp(-54.9039154, -360.700012, 9523.64551);

wait (2)

local plr = game:service"Players".LocalPlayer;
local tween_s = game:service"TweenService";
local info = TweenInfo.new(2,Enum.EasingStyle.Quad);
function tp(...)
   local tic_k = tick();
   local params = {...};
   local cframe = CFrame.new(params[1],params[2],params[3]);
   local tween,err = pcall(function()
       local tween = tween_s:Create(plr.Character["HumanoidRootPart"],info,{CFrame=cframe});
       tween:Play();
   end)
   if not tween then return err end
end
tp(-51.9489594, -345.982483, 9497.56055);

wait (7)
end
end)

local Section = Tab:NewSection("fram rejoin for stop")
Section:NewButton("rejoin", "ButtonInfo", function()
local ts = game:GetService("TeleportService")

local p = game:GetService("Players").LocalPlayer

 

ts:Teleport(game.PlaceId, p)
end)


local Tab = Window:NewTab("misc")

local Section = Tab:NewSection("inf jump")
Section:NewToggle("on", "Click to use fram", function(state)
local UIS = game:GetService("UserInputService")
local lp = game.Players.LocalPlayer
local c = lp.Character

UIS.InputBegan:connect(function(input, processed)
c.Humanoid.JumpPower = 50 -- sets the JumpPower from 0 to 50 (default JumpPower)
if processed then return end
if input.KeyCode == Enum.KeyCode.Space then -- if the space key is pressed
game.Players.LocalPlayer.Character.Humanoid:ChangeState(Enum.HumanoidStateType.Jumping)  -- Humanoid.Jump = true does not work, so I used changestate
end
end)
end)
local Section = Tab:NewSection("inf jump")
Section:NewToggle("on", "Click to use fram", function(state)
end)
local Tab = Window:NewTab("CREDIT")
local Section = Tab:NewSection("NUY GOD")


Section:NewKeybind("OFF UI", "KeybindInfo", Enum.KeyCode.RightControl, function()
	Library:ToggleUI()
end)
