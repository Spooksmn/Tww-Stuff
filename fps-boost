local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "TWW Fps Booster", HidePremium = false, SaveConfig = true, ConfigFolder = "Tww Fps Boost"})


local Tab = Window:MakeTab({
	Name = "Main",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})


Tab:AddButton({
	Name = "Boost FPS",
	Callback = function()
        local decalsyeeted = true
local g = game
local w = g.Workspace
local l = g.Lighting
local t = w.Terrain
t.WaterWaveSize = 0
t.WaterWaveSpeed = 0
t.WaterReflectance = 0
t.WaterTransparency = 0
l.GlobalShadows = false
l.FogEnd = 9e9
l.Brightness = 0
settings().Rendering.QualityLevel = "Level01"
for i, v in pairs(g:GetDescendants()) do
    if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
        v.Material = "Plastic"
        v.Reflectance = 0
    elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
        v.Transparency = 1
    elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
        v.Lifetime = NumberRange.new(0)
    elseif v:IsA("Explosion") then
        v.BlastPressure = 1
        v.BlastRadius = 1
    elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
        v.Enabled = false
    elseif v:IsA("MeshPart") then
        v.Material = "Plastic"
        v.Reflectance = 0
        v.TextureID = 10385902758728957
    end
end
for i, e in pairs(l:GetChildren()) do
    if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
        e.Enabled = false
    end
end
      		print("button pressed")
  	end    
})

Tab:AddButton({
	Name = "Fullbright",
	Callback = function()
        local lighting = game:GetService("Lighting");
lighting.Ambient = Color3.fromRGB(255, 255, 255);
lighting.Brightness = 1;
lighting.FogEnd = 1e10;
for i, v in pairs(lighting:GetDescendants()) do
	if v:IsA("BloomEffect") or v:IsA("BlurEffect") or v:IsA("ColorCorrectionEffect") or v:IsA("SunRaysEffect") then
		v.Enabled = false;
	end;
end;
lighting.Changed:Connect(function()
	lighting.Ambient = Color3.fromRGB(255, 255, 255);
	lighting.Brightness = 1;
	lighting.FogEnd = 1e10;
end);
spawn(function()
	local character = game:GetService("Players").LocalPlayer.Character;
	while wait() do
		repeat wait() until character ~= nil;
		if not character.HumanoidRootPart:FindFirstChildWhichIsA("PointLight") then
			local headlight = Instance.new("PointLight", character.HumanoidRootPart);
			headlight.Brightness = 1;
			headlight.Range = 60;
		end;
	end;
end);
      		print("button pressed")
  	end    
})
