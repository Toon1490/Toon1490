--//=================================\\
--|| 	  FE Snake Banisher V3 (SBV3)
--|| 	  Original Script Made by MLG Super Killer (aka Imshuttingdown)
--||       Converted by Epic
--||       (I have no idea where is V1 lul)
--\\=================================//

--Before u ask "Umm hey, i look at the code and it downloads something to my device"
--It just MP3 file bru
--[[ Here are hats (7 hats)
www.roblox.com/catalog/3443038622/International-Fedora-Peru
www.roblox.com/catalog/3656493304/International-Fedora-South-Korea
www.roblox.com/catalog/4819740796/Robox
www.roblox.com/catalog/9867481700/Le-Rouge-Cross-body-Bag-1-0
www.roblox.com/catalog/9867487176/Le-Rouge-Cross-body-Bag-3-0
www.roblox.com/catalog/10775031176/The-Pogo
www.roblox.com/catalog/7548993875/Slasher                                                                                                                                                                                ]]











--==ok lol ==--

local SName = "Mindless%20(Instrumental).mp3"
local SName2 = "SpookyRemix.mp3"
local SName3 = "BWater.mp3"
local SName4 = "ByeBye.mp3"
local SName5 = "Heavensent.mp3"
local SName6 = "RewindTimeSand.mp3"
local SName7 = "StrongerThanYou.mp3"
local SName8 = "Suffering%20Siblings%20(Instrumental).mp3"
local SName9 = "Blessed%20By%20Swords%20(Instrumental).mp3"
if not isfile(SName) then
    game:GetService("StarterGui"):SetCore("SendNotification", { 
	    Title = "Downloading MP3 Files";
	    Text = "Wait...";
	    Icon = "rbxthumb://type=Asset&id=1030775394&w=150&h=150"})
    Duration = 7
    writefile(SName, game:HttpGet("https://drive.google.com/uc?export=download&id=1_tLlYk3QqeKlSSfLoYnPJ1yonaL9Gx9L"))
end
if not isfile(SName2) then
    writefile(SName2, game:HttpGet("https://drive.google.com/uc?export=download&id=16YHpLa0pt9AQ-GUUMpjre7Z9rXt8MRbl"))
end
if not isfile(SName3) then
    writefile(SName3, game:HttpGet("https://drive.google.com/uc?export=download&id=1j1f6mtzO-eMaTWRlslAdYiytviwPl-S-"))
end
if not isfile(SName4) then
    writefile(SName4, game:HttpGet("https://drive.google.com/uc?export=download&id=1fwNYk9GCcp92sG7uklYWPiIHKxAvKd0h"))
end
if not isfile(SName5) then
    writefile(SName5, game:HttpGet("https://drive.google.com/uc?export=download&id=16dPgmiqABZjpad1NVs1hhn85rfFuiIZU"))
end
if not isfile(SName6) then
    writefile(SName6, game:HttpGet("https://drive.google.com/uc?export=download&id=1HZlJqAJ_-Pt9oNQ1LXyPpy7MYBem6nmO"))
end
if not isfile(SName7) then
    writefile(SName7, game:HttpGet("https://drive.google.com/uc?export=download&id=1vr17y5wxI4DfDHPHBiWXYO8R2IdKJrBy"))
end
if not isfile(SName8) then
    writefile(SName8, game:HttpGet("https://drive.google.com/uc?export=download&id=1Iwh4OcU_kdjiVY3L6eRfHOeCI7dcidM9"))
end
if not isfile(SName9) then
    writefile(SName9, game:HttpGet("https://drive.google.com/uc?export=download&id=1j2YSqIkZUWN3eiEA1fow2l9s9bHJOCKj"))
end
game:GetService("StarterGui"):SetCore("SendNotification", { 
	    Title = "Bruh";
	    Text = "Load da Reanimate!";
	    Icon = "rbxthumb://type=Asset&id=1030775394&w=150&h=150"})
    Duration = 7
local FunnyEffects = false
local RemoveAnimate = true
game.Players.LocalPlayer.Character.Animate.Parent = nil
game.Players.LocalPlayer.Character.Humanoid.Animator.Parent = nil
game:GetService("Players").LocalPlayer.Character.Head.Anchored = true
for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
 if v:IsA("BasePart") and v.Name ~="HumanoidRootPart" then
 game:GetService("RunService").Heartbeat:connect(function()
 v.Velocity = Vector3.new(0,35,0)
    wait(0.5)
   end)
  end
end
game.TestService.IsSleepAllowed = false
for i,v in next, game:GetService("Players").LocalPlayer.Character:GetDescendants() do
	if v:IsA("BasePart") then 
		game:GetService("RunService").Heartbeat:connect(function()
			v.Velocity = Vector3.new(-40,0,-10)
			pcall(function()
				v.CanCollide = false
			end)
			pcall(function()
				v.CanQuery = false
			end)
		end)
	end
end
loadstring(game:HttpGet(("https://raw.githubusercontent.com/BloxinStud10/RNTE/main/Free%20Stuff"),true))()
game:GetService("Players").LocalPlayer.Character.Head.Anchored = false
game:GetService("Players").LocalPlayer.Character.PogoStick.Handle["att1_Handle"].Name = "att2_Handle"
game:GetService("Players").LocalPlayer.Character.Back_AccAccessory.Handle["att1_Handle"].Name = "att3_Handle"
setfpscap(120)
function swait()
	game.RunService.Heartbeat:wait()
end
function Swait()
	game.RunService.Heartbeat:wait()
end
local script = game:GetObjects("rbxassetid://8496337680")[1]
local function randomstring()
	local length = math.random(10,20)
	local array = {}
	for i = 1,length do
		array[i] = string.char(math.random(32,126))
	end
	return table.concat(array)
end
local USERNAME = game.Players.LocalPlayer.Name
local Player = game:GetService("Players"):FindFirstChild(USERNAME)

local lplr = game:GetService("Players").LocalPlayer

local Character = lplr.Character


local Humanoid = Character.Humanoid
MRANDOM = math.random
CF = CFrame.new
ANGLES = CFrame.Angles
angles = CFrame.Angles
RAD = math.rad
SIN = math.sin
COS = math.cos
C3 = Color3.new
Sin = math.sin
IT = Instance.new
Rad = math.rad
BRICKC = BrickColor.new
Euler = CFrame.fromEulerAnglesXYZ
EULER = CFrame.fromEulerAnglesXYZ
Cos = math.cos
Cf = CFrame.new
VT = Vector3.new
FuckItImOverTheBeef = table.insert
Cam = workspace.CurrentCamera

local LeftArm = Character["Left Arm"]
local RightArm = Character["Right Arm"]
local LeftLeg = Character["Left Leg"]
local RightLeg = Character["Right Leg"]
local Head = Character.Head
local Torso = Character.Torso
local RootPart = Character.HumanoidRootPart
local RootJoint = RootPart.RootJoint
local Neck = Torso["Neck"]
local Players = Player
local RightShoulder = Torso["Right Shoulder"]
local LeftShoulder = Torso["Left Shoulder"]
local RightHip = Torso["Right Hip"]
local LeftHip = Torso["Left Hip"]
local Effects = Instance.new("Folder", Character)
local AlignedKatana = false
local AlignedGun = false


local shade = Color3.new(248, 0, 0)
local alreadyfixing = false
local pp = false
local function characterfixer()
    --[[]]--
end
local Sound = Instance.new("Sound", Character)

local FONTS = {
	Enum.Font.Antique,
	Enum.Font.Arcade,
	Enum.Font.Arial,
	Enum.Font.ArialBold,
	Enum.Font.Bodoni,
	Enum.Font.Cartoon,
	Enum.Font.Code,
	Enum.Font.Fantasy,
	Enum.Font.Garamond,
	Enum.Font.Highway,
	Enum.Font.Legacy,
	Enum.Font.SciFi,
	Enum.Font.SourceSans,
	Enum.Font.SourceSansBold,
	Enum.Font.SourceSansItalic,
	Enum.Font.SourceSansLight,
	Enum.Font.SourceSansSemibold
	}

--//=================================\\
--||    USEFUL VALUES/FUNCTIONS
--\\=================================//

local attack = false
local ANIM = "Idle"
local attacktype = 1
local delays = false
local play = true
local Torsovelocity = (RootPart.Velocity * Vector3.new(1,0,1)).magnitude 
local sine = 0

local change = 1
local doe = 0
local SINE = 5
local ATTACK = false
local HOLD = true
local Rooted = false
local MODE = "Snake God"
local Hue = 0
local TOBANISH = {}
local laughs = {2011349649,2011349983,2011351501,2011352223,2011355991,2011356475} 
local laugh = #laughs
local TAUNTS = {907329532,907330011,907331307,907331178,907331443,907331784,907331575,907332040,907332235,907332525,907332670,907332856,907332997,907333294,907333406,907329669,907329293,907331038}
local rc0 = CFrame.new() * CFrame.Angles(math.rad(-90),math.rad(0),math.rad(180))
local nc0 = CFrame.new(0,1,0) * CFrame.Angles(math.rad(-90),math.rad(0),math.rad(180))
local rscp = CFrame.new(-.5,0,0) * CFrame.Angles(math.rad(0),math.rad(90),math.rad(0))
local lscp = CFrame.new(.5,0,0) * CFrame.Angles(math.rad(0),math.rad(-90),math.rad(0))
local ROOTC0 = CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(180))
local NECKC0 = CFrame.new(0, 1, 0) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(180))
local RIGHTSHOULDERC0 = CFrame.new(-0.5, 0, 0) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0))
local LEFTSHOULDERC0 = CFrame.new(0.5, 0, 0) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0))
local PlayerSize = 1
local DAMAGEMULTIPLIER = 0
local FT,FRA,FLA,FRL,FLL = Instance.new("SpecialMesh"),Instance.new("SpecialMesh"),Instance.new("SpecialMesh"),Instance.new("SpecialMesh"),Instance.new("SpecialMesh")
FT.MeshId,FT.Scale = "rbxasset://fonts/torso.mesh",Vector3.new(PlayerSize,PlayerSize,PlayerSize)
FRA.MeshId,FRA.Scale = "rbxasset://fonts/rightarm.mesh",Vector3.new(PlayerSize,PlayerSize,PlayerSize)
FLA.MeshId,FLA.Scale = "rbxasset://fonts/leftarm.mesh",Vector3.new(PlayerSize,PlayerSize,PlayerSize)
FRL.MeshId,FRL.Scale = "rbxasset://fonts/rightleg.mesh",Vector3.new(PlayerSize,PlayerSize,PlayerSize)
FLL.MeshId,FLL.Scale = "rbxasset://fonts/leftleg.mesh",Vector3.new(PlayerSize,PlayerSize,PlayerSize)
Animation_Speed = 2
SIZE = 1

Sound.SoundId = syn and getsynasset('Mindless%20(Instrumental).mp3') or getcustomasset('Mindless%20(Instrumental).mp3')
Sound.Volume = 5
Sound.TimePosition = "2.2"
Sound.Pitch = 1
Sound.Looped = true
Sound:Play()

--//=================================\\
--|| 	      SOME FUNCTIONS
--\\=================================//

Debris = game:GetService("Debris")

function MakeForm(PART,TYPE)
	if TYPE == "Cyl" then
		local MSH = IT("CylinderMesh",PART)
	elseif TYPE == "Ball" then
		local MSH = IT("SpecialMesh",PART)
		MSH.MeshType = "Sphere"
	elseif TYPE == "Wedge" then
		local MSH = IT("SpecialMesh",PART)
		MSH.MeshType = "Wedge"
	end
end

function CreatePart(FormFactor, Parent, Material, Reflectance, Transparency, BColor, Name, Size)
	local Part = Create("Part")({
		formFactor = FormFactor,
		Parent = Parent,
		Reflectance = Reflectance,
		Transparency = Transparency,
		CanCollide = false,
		Locked = true,
		BrickColor = BrickColor.new(tostring(BColor)),
		Name = Name,
		Size = Size,
		Material = Material
	})
	RemoveOutlines(Part)
	return Part
end
function CreateMesh(Mesh, Part, MeshType, MeshId, OffSet, Scale)
	local Msh = Create(Mesh)({
		Parent = Part,
		Offset = OffSet,
		Scale = Scale
	})
	if Mesh == "SpecialMesh" then
		Msh.MeshType = MeshType
		Msh.MeshId = MeshId
	end
	return Msh
end
function CreateWeld(Parent, Part0, Part1, C0, C1)
	local Weld = Create("Weld")({
		Parent = Parent,
		Part0 = Part0,
		Part1 = Part1,
		C0 = C0,
		C1 = C1
	})
	return Weld
end

function SpawnTrail2(FROM,TO,BIG)
	local TRAIL = CreatePart(3, Effects, "Neon", 0, 0, BrickColor.Random(), "Trail", VT(45,45,45))           
	MakeForm(TRAIL,"Cyl")
	local DIST = (FROM - TO).Magnitude
	if BIG == true then
		TRAIL.Size = VT(2,DIST,5)
	else
		TRAIL.Size = VT(2,DIST,5)
	end
	TRAIL.CFrame = CFrame.new(FROM, TO) * CFrame.new(0, 0, -DIST/2) * ANGLES(RAD(90),RAD(0),RAD(0))
	coroutine.resume(coroutine.create(function()
		for i = 1, 55 do
			swait()
			TRAIL.Transparency = TRAIL.Transparency + 0.03
		end
		TRAIL:remove()
	end))
end

function SpawnTrail3(FROM,TO,BIG)
	local TRAIL = CreatePart(3, Effects, "Neon", 0, 0, "Really black", "Trail", VT(45,45,45))           
	MakeForm(TRAIL,"Cyl")
	local DIST = (FROM - TO).Magnitude
	if BIG == true then
		TRAIL.Size = VT(2,DIST,5)
	else
		TRAIL.Size = VT(2,DIST,5)
	end
	TRAIL.CFrame = CFrame.new(FROM, TO) * CFrame.new(0, 0, -DIST/2) * ANGLES(RAD(90),RAD(0),RAD(0))
	coroutine.resume(coroutine.create(function()
		for i = 1, 55 do
			swait()
			TRAIL.Transparency = TRAIL.Transparency + 0.03
			TRAIL.Color = BrickColor.Random().Color
		end
		TRAIL:remove()
	end))
end

function DISEMBOWEL(MODEL)
end

function WACKYEFFECT6(Table)
	local TYPE = Table.EffectType or "Sphere"
	local SIZE = Table.Size or VT(1, 1, 1)
	local ENDSIZE = Table.Size2 or VT(0, 0, 0)
	local TRANSPARENCY = Table.Transparency or 0
	local ENDTRANSPARENCY = Table.Transparency2 or 1
	local CFRAME = Table.CFrame or Torso.CFrame
	local MOVEDIRECTION = Table.MoveToPos or nil
	local ROTATION1 = Table.RotationX or 0
	local ROTATION2 = Table.RotationY or 0
	local ROTATION3 = Table.RotationZ or 0
	local MATERIAL = Table.Material --or "Neon"
	local COLOR = Table.Color or C3(1, .7, 0)
	local TIME = Table.Time or 45
	local SOUNDID = Table.SoundID or nil
	local SOUNDPITCH = Table.SoundPitch or nil
	local SOUNDVOLUME = Table.SoundVolume or nil
	local USEBOOMERANGMATH = Table.UseBoomerangMath or false
	local BOOMERANG = Table.Boomerang or 0
	local SIZEBOOMERANG = Table.SizeBoomerang or 0
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND
		local EFFECT = CreatePart(3, Effects, "Neon", 0, TRANSPARENCY, BRICKC("Pearl"), "Effect", VT(1, 1, 1), true)
		EFFECT.Color = BrickColor.Random().Color
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID, EFFECT, SOUNDVOLUME, SOUNDPITCH, false)
		end
		local MSH
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, VT(0, 0, 0))
		elseif TYPE == "Block" or TYPE == "Box" then
			MSH = IT("BlockMesh", EFFECT)
			MSH.Scale = SIZE
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, VT(0, 0, -SIZE.X / 8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "559831844", "", VT(SIZE.X, SIZE.X, 0.1), VT(0, 0, 0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662586858", "", VT(SIZE.X / 10, 0, SIZE.X / 10), VT(0, 0, 0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662585058", "", VT(SIZE.X / 10, 0, SIZE.X / 10), VT(0, 0, 0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "168892432", "", SIZE, VT(0, 0, 0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, VT(0, 0, 0))
		elseif TYPE == "Star" then 
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "2760116123", "", SIZE, VT(0,0,0))   	
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "450656451", "", SIZE, VT(0, 0, 0))
		end
		coroutine.resume(coroutine.create(function()
			if MSH ~= nil then
				local BOOMR1 = 1 + BOOMERANG / 50
				local BOOMR2 = 1 + SIZEBOOMERANG / 50
				local MOVESPEED = nil
				if MOVEDIRECTION ~= nil then
					MOVESPEED = (CFRAME.p - MOVEDIRECTION).Magnitude/TIME
				end
				local GROWTH
				if USEBOOMERANGMATH == true then
					GROWTH = (SIZE - ENDSIZE) * (BOOMR2 + 1)
				else
					GROWTH = SIZE - ENDSIZE
				end
				local TRANS = TRANSPARENCY - ENDTRANSPARENCY
				if TYPE == "Block" then
					EFFECT.CFrame = CFRAME * ANGLES(RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)))
				else
					EFFECT.CFrame = CFRAME
				end
				if USEBOOMERANGMATH == true then
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - VT(GROWTH.X * (1 - LOOP / TIME * BOOMR2), GROWTH.Y * (1 - LOOP / TIME * BOOMR2), GROWTH.Z * (1 - LOOP / TIME * BOOMR2)) * BOOMR2 / TIME
						if TYPE == "Wave" then
							MSH.Offset = VT(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * ANGLES(RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * ANGLES(RAD(ROTATION1), RAD(ROTATION2), RAD(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CF(EFFECT.Position, MOVEDIRECTION) * CF(0, 0, -MOVESPEED * (1 - LOOP / TIME * BOOMR1))
							EFFECT.Orientation = ORI
						end
					end
				else
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - GROWTH / TIME
						if TYPE == "Wave" then
							MSH.Offset = VT(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * ANGLES(RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * ANGLES(RAD(ROTATION1), RAD(ROTATION2), RAD(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CF(EFFECT.Position,MOVEDIRECTION)*CF(0,0,-MOVESPEED)
							EFFECT.Orientation = ORI
						end
					end
				end
				EFFECT.Transparency = 1
				if PLAYSSOUND == false then
					EFFECT:remove()
				else
					repeat
						swait()
					until EFFECT:FindFirstChildOfClass("Sound") == nil
					EFFECT:remove()
				end
			elseif PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat
					swait()
				until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:remove()
			end
		end))
		return EFFECT
	end))
end   

function AOETime2(POSITION,RANGE)
	for index, CHILD in pairs(workspace:GetDescendants()) do
		if CHILD.ClassName == "Model" and CHILD ~= Character then
			local HUM = CHILD:FindFirstChildOfClass("Humanoid")
			if HUM then
				local TORSO = CHILD:FindFirstChild("Torso") or CHILD:FindFirstChild("UpperTorso")
				if TORSO then
					if (TORSO.Position - POSITION).Magnitude <= RANGE then
						DISEMBOWEL(CHILD)
					end
				end
			end
		end
	end
end

local DECAL = IT("Decal")
function MagicRing()
	local RING = CreatePart(3, Effects, "Granite", 0, 1, "Maroon", "MagicRing", VT(0,0,0),true)
	local MESH = IT("BlockMesh",RING)
	local BOTTOMTEXTURE = DECAL:Clone()
	BOTTOMTEXTURE.Parent = RING
	BOTTOMTEXTURE.Face = "Bottom"
	BOTTOMTEXTURE.Name = "BottomTexture"
	local TOPTEXTURE = DECAL:Clone()
	TOPTEXTURE.Parent = RING
	TOPTEXTURE.Face = "Top"
	TOPTEXTURE.Name = "TopTexture"
	BOTTOMTEXTURE.Texture = "http://www.roblox.com/asset/?id=1208118228"
	TOPTEXTURE.Texture = "http://www.roblox.com/asset/?id=1208118228"
	BOTTOMTEXTURE.Color3 = Color3.new(0,0,0)
	TOPTEXTURE.Color3 = Color3.new(0,0,0)
	return RING,MESH,TOPTEXTURE,BOTTOMTEXTURE
end

function MakeRing()
	local RING = CreatePart(3, Effects, "Neon", 0, 1, BRICKC("Pearl"), "MagicRing", VT(0, 0, 0), true)
	local MSH = IT("BlockMesh", RING)
	local TOP = DECAL:Clone()
	local BOTTOM = DECAL:Clone()
	TOP.Parent = RING
	BOTTOM.Parent = RING
	TOP.Face = "Top"
	BOTTOM.Face = "Bottom"
	TOP.Texture = "http://www.roblox.com/asset/?id=121028264"
	BOTTOM.Texture = "http://www.roblox.com/asset/?id=121028264"
	local function REMOVE()
		coroutine.resume(coroutine.create(function()
			local SIZE = MSH.Scale.X
			for i = 1, 35 do
				swait()
				MSH.Scale = MSH.Scale - VT(SIZE, 0, SIZE) / 60
				TOP.Transparency = TOP.Transparency + 0.02857142857142857
				BOTTOM.Transparency = BOTTOM.Transparency + 0.02857142857142857
				RING.CFrame = RING.CFrame * ANGLES(RAD(0), RAD(-5), RAD(0))
			end
			RING:remove()
		end))
	end
	return RING, MSH, REMOVE
end

function ApplyAoE5(POSITION,RANGE,MINDMG,MAXDMG,FLING,INSTAKILL)
	local CHILDREN = workspace:GetDescendants()
	for index, CHILD in pairs(CHILDREN) do
		if CHILD.ClassName == "Model" and CHILD ~= Character and CHILD.Parent ~= Effects then
			local HUM = CHILD:FindFirstChildOfClass("Humanoid")
			if HUM then
				local TORSO = CHILD:FindFirstChild("Torso") or CHILD:FindFirstChild("UpperTorso")
				if TORSO then
					if (TORSO.Position - POSITION).Magnitude <= RANGE then
						if INSTAKILL == true then
						else
							local DMG = MRANDOM(MINDMG,MAXDMG)
						end
						if FLING > 0 then
							for _, c in pairs(CHILD:GetChildren()) do
								if c:IsA("BasePart") then
									local bv = Instance.new("BodyVelocity") 
									bv.maxForce = Vector3.new(1e9, 1e9, 1e9)
									bv.velocity = CFrame.new(POSITION,TORSO.Position).lookVector*FLING
									bv.Parent = c
									Debris:AddItem(bv,0.05)
								end
							end
						end
					end
				end
			end
		end
	end
end

function ApplyDamage(Humanoid,Damage,OneShot)
end

function WACKYEFFECT5(Table)
	local TYPE = (Table.EffectType or "Sphere")
	local SIZE = (Table.Size or VT(1,1,1))
	local ENDSIZE = (Table.Size2 or VT(0,0,0))
	local TRANSPARENCY = (Table.Transparency or 0)
	local ENDTRANSPARENCY = (Table.Transparency2 or 1)
	local CFRAME = (Table.CFrame or Torso.CFrame)
	local MOVEDIRECTION = (Table.MoveToPos or nil)
	local ROTATION1 = (Table.RotationX or 0)
	local ROTATION2 = (Table.RotationY or 0)
	local ROTATION3 = (Table.RotationZ or 0)
	local MATERIAL = (Table.Material or "Neon")
	local COLOR = (Table.Color or BrickColor.Random().Color)
	local TIME = (Table.Time or 45)
	local SOUNDID = (Table.SoundID or nil)
	local SOUNDPITCH = (Table.SoundPitch or nil)
	local SOUNDVOLUME = (Table.SoundVolume or nil)
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND = nil
		local EFFECT = CreatePart(3, Effects, "Neon", 0, 0, BRICKC("Pearl"), "Effect", VT(1,1,1), true)
		EFFECT.Color = BrickColor.Random().Color
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID, EFFECT, SOUNDVOLUME, SOUNDPITCH, false)
		end
		local MSH = nil
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, VT(0,0,0))
		elseif TYPE == "Block" then
			MSH = IT("BlockMesh",EFFECT)
			MSH.Scale = VT(SIZE.X,SIZE.X,SIZE.X)
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, VT(0,0,-SIZE.X/8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "559831844", "", VT(SIZE.X,SIZE.X,0.1), VT(0,0,0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662586858", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662585058", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "1051557", "", SIZE, VT(0,0,0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, VT(0,0,0))
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "9756362", "", SIZE, VT(0,0,0))
		end
		if MSH ~= nil then
			local MOVESPEED = nil
			if MOVEDIRECTION ~= nil then
				MOVESPEED = (CFRAME.p - MOVEDIRECTION).Magnitude/TIME
			end
			local GROWTH = SIZE - ENDSIZE
			local TRANS = TRANSPARENCY - ENDTRANSPARENCY
			if TYPE == "Block" then
				EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
			else
				EFFECT.CFrame = CFRAME
			end
			for LOOP = 1, TIME+1 do
				swait()
				MSH.Scale = MSH.Scale - GROWTH/TIME
				if TYPE == "Wave" then
					MSH.Offset = VT(0,0,-MSH.Scale.X/8)
				end
				EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
				if TYPE == "Block" then
					EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
				else
					EFFECT.CFrame = EFFECT.CFrame*ANGLES(RAD(ROTATION1),RAD(ROTATION2),RAD(ROTATION3))
				end
				if MOVEDIRECTION ~= nil then
					local ORI = EFFECT.Orientation
					EFFECT.CFrame = CF(EFFECT.Position,MOVEDIRECTION)*CF(0,0,-MOVESPEED)
					EFFECT.Orientation = ORI
				end
			end
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				SOUND.Stopped:Connect(function()
					EFFECT:remove()
				end)
			end
		else
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat swait() until SOUND.Playing == false
				EFFECT:remove()
			end
		end
	end))
end

function ShakeCam(Length,Intensity)
	coroutine.resume(coroutine.create(function()
		local intensity = 1 * Intensity
		local rotM = 0.01 * Intensity
		for i = 0, Length, 0.1 do
			swait()
			intensity = intensity - 0.05 * Intensity / Length
			rotM = rotM - 5.0E-4 * Intensity / Length
			Humanoid.CameraOffset = Vector3.new(RAD(MRANDOM(-intensity, intensity)), RAD(MRANDOM(-intensity, intensity)), RAD(MRANDOM(-intensity, intensity)))
			Cam.CFrame = Cam.CFrame * CF(RAD(MRANDOM(-intensity, intensity)), RAD(MRANDOM(-intensity, intensity)), RAD(MRANDOM(-intensity, intensity))) * EULER(RAD(MRANDOM(-intensity, intensity)) * rotM, RAD(MRANDOM(-intensity, intensity)) * rotM, RAD(MRANDOM(-intensity, intensity)) * rotM)
		end
		Humanoid.CameraOffset = Vector3.new(0, 0, 0)
	end))
end

function block(bonuspeed,type,pos,scale,value,value2,value3,color,color3)
	local type = type
	local rng = Instance.new("Part", Effects)
	rng.Anchored = true
	rng.BrickColor = color
	rng.Color = color3
	rng.CanCollide = false
	rng.FormFactor = 3
	rng.Name = "Ring"
	rng.Material = "Neon"
	rng.Size = Vector3.new(1, 1, 1)
	rng.Transparency = 0
	rng.TopSurface = 0
	rng.BottomSurface = 0
	rng.CFrame = pos
	local rngm = Instance.new("SpecialMesh", rng)
	rngm.MeshType = "Brick"
	rngm.Scale = scale
	local scaler2 = 1
	local scaler2b = 1
	local scaler2c = 1
	if type == "Add" then
		scaler2 = 1*value
		scaler2b = 1*value2
		scaler2c = 1*value3
	elseif type == "Divide" then
		scaler2 = 1/value
		scaler2b = 1/value2
		scaler2c = 1/value3
	end
	coroutine.resume(coroutine.create(function()
		for i = 0,10/bonuspeed,0.1 do
			swait()
			if type == "Add" then
				scaler2 = scaler2 - 0.01*value/bonuspeed
				scaler2b = scaler2b - 0.01*value/bonuspeed
				scaler2c = scaler2c - 0.01*value/bonuspeed
			elseif type == "Divide" then
				scaler2 = scaler2 - 0.01/value*bonuspeed
				scaler2b = scaler2b - 0.01/value*bonuspeed
				scaler2c = scaler2c - 0.01/value*bonuspeed
			end
			rng.CFrame = rng.CFrame*CFrame.Angles(math.rad(MRANDOM(-360,360)),math.rad(MRANDOM(-360,360)),math.rad(MRANDOM(-360,360)))
			rng.Transparency = rng.Transparency + 0.01*bonuspeed
			rngm.Scale = rngm.Scale + Vector3.new(scaler2*bonuspeed, scaler2b*bonuspeed, scaler2c*bonuspeed)
		end
		rng:Destroy()
	end))
end

function WACKYEFFECT2(Table)
	local TYPE = Table.EffectType or "Sphere"
	local SIZE = Table.Size or Vector3.new(1, 1, 1)
	local ENDSIZE = Table.Size2 or Vector3.new(0, 0, 0)
	local TRANSPARENCY = Table.Transparency or 0
	local ENDTRANSPARENCY = Table.Transparency2 or 1
	local CFRAME = Table.CFrame or Torso.CFrame
	local MOVEDIRECTION = Table.MoveToPos or nil
	local ROTATION1 = Table.RotationX or 0
	local ROTATION2 = Table.RotationY or 0
	local ROTATION3 = Table.RotationZ or 0
	local MATERIAL = Table.Material --or "Neon"
	local COLOR = Table.Color or Color3.new(1, 1, 1)
	local TIME = Table.Time or 45
	local SOUNDID = Table.SoundID or nil
	local SOUNDPITCH = Table.SoundPitch or nil
	local SOUNDVOLUME = Table.SoundVolume or nil
	local USEBOOMERANGMATH = Table.UseBoomerangMath or false
	local BOOMERANG = Table.Boomerang or 0
	local SIZEBOOMERANG = Table.SizeBoomerang or 0
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND
		local EFFECT = CreatePart(3, Effects, MATERIAL, 0, TRANSPARENCY, BRICKC("Pearl"), "Effect", Vector3.new(1, 1, 1), true)
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID, EFFECT, SOUNDVOLUME, SOUNDPITCH, false)
		end
		EFFECT.Color = COLOR
		local MSH
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Block" or TYPE == "Box" then
			MSH = IT("BlockMesh", EFFECT)
			MSH.Scale = SIZE
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, Vector3.new(0, 0, -SIZE.X / 8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "559831844", "", Vector3.new(SIZE.X, SIZE.X, 0.1), Vector3.new(0, 0, 0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662586858", "", Vector3.new(SIZE.X / 10, 0, SIZE.X / 10), Vector3.new(0, 0, 0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662585058", "", Vector3.new(SIZE.X / 10, 0, SIZE.X / 10), Vector3.new(0, 0, 0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "168892432", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Star" then 
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "2760116123", "", SIZE, Vector3.new(0,0,0))   	
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "450656451", "", SIZE, Vector3.new(0, 0, 0))
		end
		coroutine.resume(coroutine.create(function()
			if MSH ~= nil then
				local BOOMR1 = 1 + BOOMERANG / 50
				local BOOMR2 = 1 + SIZEBOOMERANG / 50
				local MOVESPEED = nil
				if MOVEDIRECTION ~= nil then
					MOVESPEED = (CFRAME.p - MOVEDIRECTION).Magnitude/TIME
				end
				local GROWTH
				if USEBOOMERANGMATH == true then
					GROWTH = (SIZE - ENDSIZE) * (BOOMR2 + 1)
				else
					GROWTH = SIZE - ENDSIZE
				end
				local TRANS = TRANSPARENCY - ENDTRANSPARENCY
				if TYPE == "Block" then
					EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
				else
					EFFECT.CFrame = CFRAME
				end
				if USEBOOMERANGMATH == true then
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - Vector3.new(GROWTH.X * (1 - LOOP / TIME * BOOMR2), GROWTH.Y * (1 - LOOP / TIME * BOOMR2), GROWTH.Z * (1 - LOOP / TIME * BOOMR2)) * BOOMR2 / TIME
						if TYPE == "Wave" then
							MSH.Offset = Vector3.new(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * CFrame.Angles(math.rad(ROTATION1), math.rad(ROTATION2), math.rad(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CFrame.new(EFFECT.Position, MOVEDIRECTION) * CFrame.new(0, 0, -MOVESPEED * (1 - LOOP / TIME * BOOMR1))
							EFFECT.Orientation = ORI
						end
					end
				else
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - GROWTH / TIME
						if TYPE == "Wave" then
							MSH.Offset = Vector3.new(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * CFrame.Angles(math.rad(ROTATION1), math.rad(ROTATION2), math.rad(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CFrame.new(EFFECT.Position,MOVEDIRECTION)*CFrame.new(0,0,-MOVESPEED)
							EFFECT.Orientation = ORI
						end
					end
				end
				EFFECT.Transparency = 1
				if PLAYSSOUND == false then
					EFFECT:remove()
				else
					repeat
						swait()
					until EFFECT:FindFirstChildOfClass("Sound") == nil
					EFFECT:remove()
				end
			elseif PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat
					swait()
				until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:remove()
			end
		end))
		return EFFECT
	end))
end      

function Kill(Char)
end


function CharacterFade(COLOR,TIMER)
end

Character["PogoStick"].Handle.att2_Handle.Parent = RightArm
RightArm.att2_Handle.Rotation = Vector3.new(45, 90, 0)
RightArm.att2_Handle.Position = Vector3.new(0, -2.4, -1.1)  

print'<===================================================>'
warn'|| Original Script made by MLG Super Killer'
warn'|| Converted by Epic'
print'<===================================================>'

function Sloice(KIND, SIZE, WAIT, CFRAME, COLOR, GROW)
	local wave = CreatePart(3, Effects, "Neon", 0, 0.5, BRICKC(COLOR), "Effect", Vector3.new(1, 1, 1), true)
	local mesh
	if KIND == "Base" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "448386996", "", Vector3.new(0, SIZE / 10, SIZE / 10), Vector3.new(0, 0, 0))
	elseif KIND == "Thin" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "662586858", "", Vector3.new(SIZE / 10, 0, SIZE / 10), Vector3.new(0, 0, 0))
	elseif KIND == "Round" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "662585058", "", Vector3.new(SIZE / 10, 0, SIZE / 10), Vector3.new(0, 0, 0))
	end
	wave.CFrame = CFRAME
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, WAIT do
			swait()
			mesh.Scale = mesh.Scale + GROW / 10
			wave.Transparency = wave.Transparency + 0.5 / WAIT
			if wave.Transparency > 0.99 then
				wave:remove()
			end
		end
	end))
end


function AddChildrenToTable(FROM, PARENT, DIST, TABLE)
	for _, c in pairs(PARENT:GetChildren()) do
		if c.ClassName == "Model" then
			if c ~= Character and c:FindFirstChildOfClass("Humanoid") and (c:FindFirstChild("Torso") or c:FindFirstChild("UpperTorso")) then
				local HUMANOID = c:FindFirstChildOfClass("Humanoid")
				local TORSO = c:FindFirstChild("Torso") or c:FindFirstChild("UpperTorso")
				if DIST > (TORSO.Position - FROM).Magnitude then
					table.insert(TABLE, c)
				end
				AddChildrenToTable(FROM, c, DIST, TABLE)
			elseif c.ClassName == "Folder" then
				AddChildrenToTable(FROM, c, DIST, TABLE)
			end
		end
	end
end

function FireArc(Part, ToLocation, AmountOfTime, Height, DoesCourontine)
	if DoesCourontine == false then
		local Direction = CFrame.new(Part.Position, ToLocation)
		local Distance = (Part.Position - ToLocation).magnitude
		for i = 1, AmountOfTime do
			swait()
			Part.CFrame = Direction * CFrame.new(0, AmountOfTime / 200 + (AmountOfTime / Height - i * 2 / Height), -Distance / AmountOfTime)
			Direction = Part.CFrame
		end
		Part:remove()
	elseif DoesCourontine == true then
		coroutine.resume(coroutine.create(function()
			local Direction = CFrame.new(Part.Position, ToLocation)
			local Distance = (Part.Position - ToLocation).magnitude
			for i = 1, AmountOfTime do
				swait()
				Part.CFrame = Direction * CFrame.new(0, AmountOfTime / 200 + (AmountOfTime / Height - i * 2 / Height), -Distance / AmountOfTime)
				Direction = Part.CFrame
			end
			Part:remove()
		end))
	end
end

function Slice2(KIND, SIZE, WAIT, CFRAME, COLOR, GROW)
	local wave = CreatePart(3, Effects, "Neon", 0, 0.5, BrickColor.new(COLOR), "Effect", Vector3.new(1, 1, 1), true)
	local mesh
	if KIND == "Base" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "448386996", "", Vector3.new(0, SIZE / 10, SIZE / 10), Vector3.new(0, 0, 0))
	elseif KIND == "Thin" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "662586858", "", Vector3.new(SIZE / 10, 0, SIZE / 10), Vector3.new(0, 0, 0))
	elseif KIND == "Round" then
		mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "662585058", "", Vector3.new(SIZE / 10, 0, SIZE / 10), Vector3.new(0, 0, 0))
	end
	wave.CFrame = CFRAME
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, WAIT do
			swait()
			mesh.Scale = mesh.Scale + GROW / 10
			wave.Transparency = wave.Transparency + 0.5 / WAIT
			if wave.Transparency > 0.99 then
				wave:remove()
			end
		end
	end))
end

function CreateWave(SIZE, WAIT, CFRAME, DOESROT, ROT, COLOR, GROW)
	local wave = CreatePart(3, Effects, "Neon", 0, 0.5, BrickColor.new(COLOR), "Effect", Vector3.new(0, 0, 0))
	local mesh = CreateMesh2("SpecialMesh", wave, "FileMesh", "20329976", "", SIZE, Vector3.new(0, 0, -SIZE.X / 8))
	wave.CFrame = CFRAME
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, WAIT do
			swait()
			mesh.Scale = mesh.Scale + GROW
			mesh.Offset = Vector3.new(0, 0, -(mesh.Scale.X / 8))
			if DOESROT == true then
				wave.CFrame = wave.CFrame * CFrame.fromEulerAnglesXYZ(0, ROT, 0)
			end
			wave.Transparency = wave.Transparency + 0.5 / WAIT
			if wave.Transparency > 0.99 then
				wave:remove()
			end
		end
	end))
end

function CreateWeldOrSnapOrMotor(TYPE, PARENT, PART0, PART1, C0, C1)
	local NEWWELD = IT(TYPE)
	NEWWELD.Part0 = PART0
	NEWWELD.Part1 = PART1
	NEWWELD.C0 = C0
	NEWWELD.C1 = C1
	NEWWELD.Parent = PARENT
	return NEWWELD
end

function CreateMesh2(MESH, PARENT, MESHTYPE, MESHID, TEXTUREID, SCALE, OFFSET)
	local NEWMESH = IT(MESH)
	if MESH == "SpecialMesh" then
		NEWMESH.MeshType = MESHTYPE
		if MESHID ~= "nil" and MESHID ~= "" then
			NEWMESH.MeshId = "http://www.roblox.com/asset/?id="..MESHID
		end
		if TEXTUREID ~= "nil" and TEXTUREID ~= "" then
			NEWMESH.TextureId = "http://www.roblox.com/asset/?id="..TEXTUREID
		end
	end
	NEWMESH.Offset = OFFSET or VT(0, 0, 0)
	NEWMESH.Scale = SCALE
	NEWMESH.Parent = PARENT
	return NEWMESH
end

function WACKYEFFECT(Table)
	local TYPE = (Table.EffectType or "Sphere")
	local SIZE = (Table.Size or VT(1,1,1))
	local ENDSIZE = (Table.Size2 or VT(0,0,0))
	local TRANSPARENCY = (Table.Transparency or 0)
	local ENDTRANSPARENCY = (Table.Transparency2 or 1)
	local CFRAME = (Table.CFrame or Torso.CFrame)
	local MOVEDIRECTION = (Table.MoveToPos or nil)
	local ROTATION1 = (Table.RotationX or 0)
	local ROTATION2 = (Table.RotationY or 0)
	local ROTATION3 = (Table.RotationZ or 0)
	local MATERIAL = (Table.Material or "Neon")
	local COLOR = (Table.Color or Color3.new(1,1,1))
	local TIME = (Table.Time or 45)
	local SOUNDID = (Table.SoundID or nil)
	local SOUNDPITCH = (Table.SoundPitch or nil)
	local SOUNDVOLUME = (Table.SoundVolume or nil)
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND = nil
		local EFFECT = CreatePart(3, Effects, MATERIAL, 0, TRANSPARENCY, BRICKC("Pearl"), "Effect", VT(1,1,1), true)
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID, EFFECT, SOUNDVOLUME, SOUNDPITCH, false)
		end
		EFFECT.Color = COLOR
		local MSH = nil
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, VT(0,0,0))
		elseif TYPE == "Block" then
			MSH = IT("BlockMesh",EFFECT)
			MSH.Scale = VT(SIZE.X,SIZE.X,SIZE.X)
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, VT(0,0,-SIZE.X/8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "559831844", "", VT(SIZE.X,SIZE.X,0.1), VT(0,0,0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662586858", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662585058", "", VT(SIZE.X/10,0,SIZE.X/10), VT(0,0,0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "1051557", "", SIZE, VT(0,0,0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, VT(0,0,0))
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "9756362", "", SIZE, VT(0,0,0))
		end
		if MSH ~= nil then
			local MOVESPEED = nil
			if MOVEDIRECTION ~= nil then
				MOVESPEED = (CFRAME.p - MOVEDIRECTION).Magnitude/TIME
			end
			local GROWTH = SIZE - ENDSIZE
			local TRANS = TRANSPARENCY - ENDTRANSPARENCY
			if TYPE == "Block" then
				EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
			else
				EFFECT.CFrame = CFRAME
			end
			for LOOP = 1, TIME+1 do
				swait()
				MSH.Scale = MSH.Scale - GROWTH/TIME
				if TYPE == "Wave" then
					MSH.Offset = VT(0,0,-MSH.Scale.X/8)
				end
				EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
				if TYPE == "Block" then
					EFFECT.CFrame = CFRAME*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))
				else
					EFFECT.CFrame = EFFECT.CFrame*ANGLES(RAD(ROTATION1),RAD(ROTATION2),RAD(ROTATION3))
				end
				if MOVEDIRECTION ~= nil then
					local ORI = EFFECT.Orientation
					EFFECT.CFrame = CF(EFFECT.Position,MOVEDIRECTION)*CF(0,0,-MOVESPEED)
					EFFECT.Orientation = ORI
				end
			end
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				SOUND.Stopped:Connect(function()
					EFFECT:remove()
				end)
			end
		else
			if PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat swait() until SOUND.Playing == false
				EFFECT:remove()
			end
		end
	end))
end

function CreatePart(FORMFACTOR, PARENT, MATERIAL, REFLECTANCE, TRANSPARENCY, BRICKCOLOR, NAME, SIZE, ANCHOR)
	local NEWPART = IT("Part")
	NEWPART.formFactor = FORMFACTOR
	NEWPART.Reflectance = REFLECTANCE
	NEWPART.Transparency = TRANSPARENCY
	NEWPART.CanCollide = false
	NEWPART.Locked = true
	NEWPART.Anchored = true
	if ANCHOR == false then
		NEWPART.Anchored = false
	end
	NEWPART.BrickColor = BRICKC(tostring(BRICKCOLOR))
	NEWPART.Name = NAME
	NEWPART.Size = SIZE
	NEWPART.Position = Torso.Position
	NEWPART.Material = MATERIAL
	NEWPART:BreakJoints()
	NEWPART.Parent = PARENT
	return NEWPART
end

function MagicSphere(SIZE,WAIT,CFRAME,COLOR,GROW)
	local wave = CreatePart(3, Effects, "Neon", 0, 0, BRICKC(COLOR), "Effect", Vector3.new(1,1,1), true)
	local mesh = IT("SpecialMesh",wave)
	mesh.MeshType = "Sphere"
	mesh.Scale = SIZE
	mesh.Offset = Vector3.new(0,0,0)
	wave.CFrame = CFRAME
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, WAIT do
			swait()
			mesh.Scale = mesh.Scale + GROW
			wave.Transparency = wave.Transparency + (1/WAIT)
			if wave.Transparency > 0.99 then
				wave:remove()
			end
		end
	end))
end

function printbye(Name)
	local MESSAGES = {"You cannot struggle, ","Your existance is an insult, ","Fade, ","Your existance is not desired, ","You are not permitted here, ","You are not to decide your fate, ","Be gone, ","You are already dead, ","Your live is an anomaly, ","Don't dare to return, ","Why are you resisting, ","You cannot exist here, ","Why are you struggling, ","Your fate was already decided, ","Goodbye, ","You cannot ignore my command, ","You cannot resist my command, ","You already died, "}
	chatfunc(MESSAGES[MRANDOM(1,#MESSAGES)]..Name..".")	
end

function Banish(Foe)

end

--SIN = math.sin
--RAD = math.rad
--ANGLES = CFrame.Angles
--COS = math.cos
--CF = CFrame.new
--C3 = Color3.new
--VT = Vector3.new

function ApplyAoE(POSITION,RANGE,ISBANISH)
	
end

function turnto(position)
	RootPart.CFrame=CFrame.new(RootPart.CFrame.p,VT(position.X,RootPart.Position.Y,position.Z)) * CFrame.new(0, 0, 0)
end

function Raycast(POSITION, DIRECTION, RANGE, IGNOREDECENDANTS)
	return workspace:FindPartOnRay(Ray.new(POSITION, DIRECTION.unit * RANGE), IGNOREDECENDANTS)
end


local Mouse = lplr:GetMouse()
local mouse = Mouse

if lplr.Name == USERNAME then
	workspace.CurrentCamera.CameraSubject = Humanoid
	workspace.CurrentCamera:GetPropertyChangedSignal("CameraSubject"):Connect(function()
		if not alreadyfixing and workspace.CurrentCamera.CameraSubject ~= Humanoid then
			workspace.CurrentCamera.CameraSubject = Humanoid
		end
	end)
end
spawn(function()
	
	
	local TS = game:GetService("TweenService")
	local PS = game:GetService("PhysicsService")
	
	ArtificialHB = Instance.new("BindableEvent",script)
	ArtificialHB.Name = "ArtificialHB"
	
	script:WaitForChild("ArtificialHB")
	
	frame = 1/60
	tf = 0
	allowframeloss = false
	tossremainder = false
	lastframe = tick()
	script.ArtificialHB:Fire()
	
	game:GetService("RunService").Heartbeat:Connect(function(s,p)
		tf = tf + s
		if tf >= frame then
			if allowframeloss then
				ArtificialHB:Fire()
				lastframe = tick()
			else
				for i = 1,math.floor(tf / frame) do
					ArtificialHB:Fire()
				end
				lastframe = tick()
			end
			if tossremainder then
				tf = 0
			else
				tf = tf - frame * math.floor(tf / frame)
			end
		end
	end)
end)
function QFCF(cf)
	local mx,my,mz,m00,m01,m02,m10,m11,m12,m20,m21,m22 = cf:components()
	local trace = m00 + m11 + m22
	if trace > 0 then 
		local s = math.sqrt(1 + trace)
		local recip = 0.5 / s
		return (m21 - m12) * recip,(m02 - m20) * recip,(m10 - m01) * recip,s * 0.5
	else
		local i = 0
		if m11 > m00 then
			i = 1
		end
		if m22 > (i == 0 and m00 or m11) then
			i = 2
		end
		if i == 0 then
			local s = math.sqrt(m00 - m11 - m22 + 1)
			local recip = 0.5 / s
			return 0.5 * s,(m10 + m01) * recip,(m20 + m02) * recip,(m21 - m12) * recip
		elseif i == 1 then
			local s = math.sqrt(m11 - m22 - m00 + 1)
			local recip = 0.5 / s
			return (m01 + m10) * recip,0.5 * s,(m21 + m12) * recip,(m02 - m20) * recip
		elseif i == 2 then
			local s = math.sqrt(m22 - m00 - m11 + 1)
			local recip = 0.5 / s return (m02 + m20) * recip,(m12 + m21) * recip,0.5 * s,(m10 - m01) * recip
		end
	end
end

function QTCF(px,py,pz,x,y,z,w)
	local xs,ys,zs = x + x,y + y,z + z
	local wx,wy,wz = w * xs,w * ys,w * zs
	local xx = x * xs
	local xy = x * ys
	local xz = x * zs
	local yy = y * ys
	local yz = y * zs
	local zz = z * zs
	return CFrame.new(px,py,pz,1 - (yy + zz),xy - wz,xz + wy,xy + wz,1 - (xx + zz),yz - wx,xz - wy,yz + wx,1 - (xx + yy))
end

function QS(a,b,t)
	local cosTheta = a[1] * b[1] + a[2] * b[2] + a[3] * b[3] + a[4] * b[4]
	local startInterp,finishInterp;
	if cosTheta >= 0.0001 then
		if (1 - cosTheta) > 0.0001 then
			local theta = math.acos(cosTheta)
			local invSinTheta = 1 / math.sin(theta)
			startInterp = math.sin((1 - t) * theta) * invSinTheta
			finishInterp = math.sin(t * theta) * invSinTheta
		else
			startInterp = 1 - t
			finishInterp = t
		end
	else
		if (1 + cosTheta) > 0.0001 then
			local theta = math.acos(-cosTheta)
			local invSinTheta = 1 / math.sin(theta)
			startInterp = math.sin((t - 1) * theta) * invSinTheta
			finishInterp = math.sin(t * theta) * invSinTheta
		else
			startInterp = t - 1
			finishInterp = t
		end
	end
	return a[1] * startInterp + b[1] * finishInterp,a[2] * startInterp + b[2] * finishInterp,a[3] * startInterp + b[3] * finishInterp,a[4] * startInterp + b[4] * finishInterp
end

function Clerp(a,b,t)
	local qa = {QFCF(a)}
	local qb = {QFCF(b)}
	local ax,ay,az = a.x,a.y,a.z
	local bx,by,bz = b.x,b.y,b.z
	local _t = 1 - t
	return QTCF(_t * ax + t * bx,_t * ay + t * by,_t * az + t * bz,QS(qa,qb,t))
end

ArtificialHB = Instance.new("BindableEvent",script)
ArtificialHB.Name = "Heartbeat"

script:WaitForChild("Heartbeat")

frame = 1 / 30
tf = 0
allowframeloss = false
tossremainder = false
lastframe = tick()
script.Heartbeat:Fire()

game:GetService("RunService").Heartbeat:Connect(function(s,p)
	tf = tf + s
	if tf >= frame then
		if allowframeloss then
			script.Heartbeat:Fire()
			lastframe = tick()
		else
			for i = 1,math.floor(tf / frame) do
				script.Heartbeat:Fire()
			end
			lastframe = tick()
		end
		if tossremainder then
			tf = 0
		else
			tf = tf - frame * math.floor(tf / frame)
		end
	end
end)

function swait(num)
	if num == 0 or num == nil then
		ArtificialHB.Event:Wait()
	else
		for i = 0,num do
			ArtificialHB.Event:Wait()
		end
	end
end

function CreateMesh(MESH,PARENT,MESHTYPE,MESHID,TEXTUREID,SCALE,OFFSET)
	local NEWMESH = Instance.new(MESH)
	if MESH == "SpecialMesh" then
		NEWMESH.MeshType = MESHTYPE
		if MESHID ~= "nil" and MESHID ~= "" then
			NEWMESH.MeshId = "rbxassetid://"..MESHID
		end
		if TEXTUREID ~= "nil" and TEXTUREID ~= "" then
			NEWMESH.TextureId = "rbxassetid://"..TEXTUREID
		end
	end
	NEWMESH.Offset = OFFSET or Vector3.new()
	NEWMESH.Scale = SCALE
	NEWMESH.Parent = PARENT
	return NEWMESH
end

local S = Instance.new("Sound")
function CreateSound(ID,PARENT,VOLUME,PITCH,DOESLOOP)
	local NEWSOUND = nil
	coroutine.resume(coroutine.create(function()
		NEWSOUND = S:Clone()
		NEWSOUND.Parent = PARENT
		NEWSOUND.Volume = VOLUME
		NEWSOUND.Pitch = PITCH
		NEWSOUND.SoundId = "rbxassetid://"..ID
		NEWSOUND:play()
		if DOESLOOP == true then
			NEWSOUND.Looped = true
		else
			coroutine.resume(coroutine.create(function()
				pcall(function()
					repeat swait() until NEWSOUND.Playing == false
					NEWSOUND:Destroy()
				end)
			end))
		end
	end))
	return NEWSOUND
end

function rayCast(Position,Direction,Range,Ignore)
	return workspace:FindPartOnRay(Ray.new(Position,Direction.unit * (Range or 999.999)),Ignore) 
end 		

function Effect(Table)
	local TYPE = (Table.EffectType or "Sphere")
	local SIZE = (Table.Size or Vector3.new(1,1,1))
	local ENDSIZE = (Table.Size2 or Vector3.new())
	local TRANSPARENCY = (Table.Transparency or 0)
	local ENDTRANSPARENCY = (Table.Transparency2 or 1)
	local CFRAME = (Table.CFrame or Torso.CFrame)
	local MOVEDIRECTION = (Table.MoveToPos or nil)
	local ROTATION1 = (Table.RotationX or 0)
	local ROTATION2 = (Table.RotationY or 0)
	local ROTATION3 = (Table.RotationZ or 0)
	local MATERIAL = (Table.Material or "Neon")
	local COLOR = (Table.Color or shade)
	local hOK,sOK,vOK = Color3.toHSV(COLOR)
	local TIME = (Table.Time or 45)
	local SOUNDID = (Table.SoundID or nil)
	local SOUNDPITCH = (Table.SoundPitch or nil)
	local SOUNDVOLUME = (Table.SoundVolume or nil)
	local USEBOOMERANGMATH = (Table.UseBoomerangMath or false)
	local BOOMERANG = (Table.Boomerang or 0)
	local SIZEBOOMERANG = (Table.SizeBoomerang or 0)
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND = nil
		local EFFECT = CreatePart(3,Effects,MATERIAL,0,TRANSPARENCY,shade,"Effect",Vector3.new(1,1,1),true)
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID,EFFECT,SOUNDVOLUME,SOUNDPITCH,false)
		end
		EFFECT.Color = COLOR
		local MSH = nil
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"Sphere","","",SIZE,Vector3.new())
		elseif TYPE == "Block" or TYPE == "Box" then
			MSH = Instance.new("BlockMesh",EFFECT)
			MSH.Scale = SIZE
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","20329976","",SIZE,Vector3.new(0,0,-SIZE.X/8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","559831844","",Vector3.new(SIZE.X,SIZE.X,0.1),Vector3.new())
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","662586858","",Vector3.new(SIZE.X/10,0,SIZE.X/10),Vector3.new())
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","662585058","",Vector3.new(SIZE.X/10,0,SIZE.X/10),Vector3.new())
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","168892432","",SIZE,Vector3.new())
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","4770583","",SIZE,Vector3.new())
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh",EFFECT,"FileMesh","9756362","",SIZE,Vector3.new())
		end
		if MSH ~= nil then
			local BOOMR1 = 1+BOOMERANG/50
			local BOOMR2 = 1+SIZEBOOMERANG/50
			local MOVESPEED = nil
			if MOVEDIRECTION ~= nil then
				if USEBOOMERANGMATH == true then
					MOVESPEED = ((CFRAME.p - MOVEDIRECTION).Magnitude/TIME)*BOOMR1
				else
					MOVESPEED = ((CFRAME.p - MOVEDIRECTION).Magnitude/TIME)
				end
			end
			local GROWTH = nil
			if USEBOOMERANGMATH == true then
				GROWTH = (SIZE - ENDSIZE)*(BOOMR2+1)
			else
				GROWTH = (SIZE - ENDSIZE)
			end
			local TRANS = TRANSPARENCY - ENDTRANSPARENCY
			if TYPE == "Block" then
				EFFECT.CFrame = CFRAME*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360)))
			else
				EFFECT.CFrame = CFRAME
			end
			if USEBOOMERANGMATH == true then
				for LOOP = 1,TIME+1 do
					swait()
					MSH.Scale = MSH.Scale - (Vector3.new((GROWTH.X)*((1 - (LOOP/TIME)*BOOMR2)),(GROWTH.Y)*((1 - (LOOP/TIME)*BOOMR2)),(GROWTH.Z)*((1 - (LOOP/TIME)*BOOMR2)))*BOOMR2)/TIME
					if TYPE == "Wave" then
						MSH.Offset = Vector3.new(0,0,-MSH.Scale.Z/8)
					end
					EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
					if TYPE == "Block" then
						EFFECT.CFrame = CFRAME*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360)))
					else
						EFFECT.CFrame = EFFECT.CFrame*CFrame.Angles(math.rad(ROTATION1),math.rad(ROTATION2),math.rad(ROTATION3))
					end
					if MOVEDIRECTION ~= nil then
						local ORI = EFFECT.Orientation
						EFFECT.CFrame = CFrame.new(EFFECT.Position,MOVEDIRECTION)*CFrame.new(0,0,-(MOVESPEED)*((1 - (LOOP/TIME)*BOOMR1)))
						EFFECT.Orientation = ORI
					end
				end
			else
				for LOOP = 1,TIME+1 do
					swait()
					MSH.Scale = MSH.Scale - GROWTH/TIME
					if TYPE == "Wave" then
						MSH.Offset = Vector3.new(0,0,-MSH.Scale.Z/8)
					end
					EFFECT.Transparency = EFFECT.Transparency - TRANS/TIME
					if TYPE == "Block" then
						EFFECT.CFrame = CFRAME*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360)))
					else
						EFFECT.CFrame = EFFECT.CFrame*CFrame.Angles(math.rad(ROTATION1),math.rad(ROTATION2),math.rad(ROTATION3))
					end
					if MOVEDIRECTION ~= nil then
						local ORI = EFFECT.Orientation
						EFFECT.CFrame = CFrame.new(EFFECT.Position,MOVEDIRECTION)*CFrame.new(0,0,-MOVESPEED)
						EFFECT.Orientation = ORI
					end
				end
			end
			EFFECT.Transparency = 1
			if PLAYSSOUND == false then
				EFFECT:Destroy()
			else
				repeat swait() until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:Destroy()
			end
		else
			if PLAYSSOUND == false then
				EFFECT:Destroy()
			else
				repeat swait() until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:Destroy()
			end
		end
	end))
end

coroutine.resume(coroutine.create(function()
	while true do
		for i = 0,1,(1/60) do
			swait()
			if not alreadyfixing then
	
			end
		end
	end
end))



function bosschatfunc(text,color,watval)
	for i,v in pairs(game:GetService("Players"):GetPlayers()) do
		coroutine.resume(coroutine.create(function()
			if v.PlayerGui:FindFirstChild("Dialog")~= nil then
				v.PlayerGui:FindFirstChild("Dialog"):destroy()
			end
			local scrg = Instance.new("ScreenGui",v.PlayerGui)
			scrg.Name = "Dialog"
			local txtlb = Instance.new("TextLabel",scrg)
			txtlb.Text = ""
			txtlb.Font = "Bodoni"
			txtlb.TextColor3 = Color3.new(0,0,0)
			txtlb.TextStrokeTransparency = 0
			txtlb.BackgroundTransparency = 0.75
			txtlb.BackgroundColor3 = Color3.new(0,0,0)
			txtlb.TextStrokeColor3 = color
			txtlb.TextScaled = true
			txtlb.Size = UDim2.new(1,0,0.25,0)
			txtlb.TextXAlignment = "Left"
			txtlb.Position = UDim2.new(0,0,0.75 + 1,0)
			local txtlb2 = Instance.new("TextLabel",scrg)
			txtlb2.Text = "Snake Banisher V3:"
			txtlb2.Font = "Arcade"
			txtlb2.TextColor3 = Color3.new(0,0,0)
			txtlb2.TextStrokeTransparency = 0
			txtlb2.BackgroundTransparency = 1
			txtlb2.TextStrokeColor3 = color
			txtlb2.TextSize = 40
			txtlb2.Size = UDim2.new(1,0,0.25,0)
			txtlb2.TextXAlignment = "Left"
			txtlb2.Position = UDim2.new(0,0,1,0)
			local fvalen = 0.55
			local fval = -0.49
			coroutine.resume(coroutine.create(function()
				while true do
					swait()
					if MODE == "Sanity" then
						txtlb.Rotation = math.random(-1,1)
						txtlb2.Rotation = math.random(-1,1)
						txtlb.Position = txtlb.Position + UDim2.new(0,math.random(-1,1)/5,0,math.random(-1,1)/5)
						txtlb2.Position = txtlb2.Position + UDim2.new(0,math.random(-1,1)/5,0,math.random(-1,1)/5)
						txtlb.TextStrokeColor3 = BrickColor.random().Color
						txtlb2.TextStrokeColor3 = BrickColor.random().Color
					end
				end
			end))
			coroutine.resume(coroutine.create(function()
				while true do
					swait()
					if scrg.Parent ~= nil then
						fvalen = fvalen - 0.0001
					elseif scrg.Parent == nil then
						break
					end
				end
			end))
			local flol = 1.75
			local flil = 1.6
			coroutine.resume(coroutine.create(function()
				for i = 0, 9 do
					swait()
					fval = fval + 0.05
					flol = flol - 0.1
					flil = flil - 0.1
					txtlb.Text = ""
					txtlb.Position = UDim2.new(0,0,flol,0)
					txtlb2.Position = UDim2.new(0,0,flil,0)
				end
				txtlb.Text = text
				wait(watval)
				local valinc = 0
				for i = 0, 99 do
					swait()
					valinc = valinc + 0.0001
					flol = flol + valinc
					flil = flil + valinc
					txtlb.Rotation = txtlb.Rotation + valinc*20
					txtlb2.Rotation = txtlb2.Rotation - valinc*50
					txtlb.Position = UDim2.new(0,0,flol,0)
					txtlb2.Position = UDim2.new(0,0,flil,0)
					txtlb.TextStrokeTransparency = txtlb.TextStrokeTransparency + 0.01
					txtlb.TextTransparency = txtlb.TextTransparency + 0.01
					txtlb2.TextStrokeTransparency = txtlb2.TextStrokeTransparency + 0.01
					txtlb2.TextTransparency = txtlb2.TextTransparency + 0.01
					txtlb.BackgroundTransparency = txtlb.BackgroundTransparency + 0.0025
				end
				scrg:Destroy()
			end))
		end))
	end
end

function warnedpeople2(whom)
	for i,v in pairs(game:GetService("Players"):GetPlayers()) do
		coroutine.resume(coroutine.create(function()
			if v.PlayerGui:FindFirstChild("ARRIVAL")~= nil then
				v.PlayerGui:FindFirstChild("ARRIVAL"):destroy()
			end
			local droppingFrame = false
			local scrg = Instance.new("ScreenGui",v.PlayerGui)
			scrg.Name = "ARRIVAL"
			local mainFrame = Instance.new("Frame", scrg)
			mainFrame.Name = "MainFrame"
			mainFrame.BackgroundTransparency = 1
			mainFrame.BorderSizePixel = 0
			mainFrame.Size = UDim2.new(1, 0, -0.013, 100)
			mainFrame.Position = UDim2.new(0, 0, 0.365, 0)
			local TextFrame = Instance.new("TextLabel",mainFrame)
			TextFrame.Name = "TextFrame"
			TextFrame.Font = "Arcade"
			TextFrame.Text = ""
			TextFrame.TextScaled = true
			TextFrame.TextSize = 9
			TextFrame.TextStrokeTransparency = 1
			TextFrame.BackgroundTransparency = 1
			TextFrame.TextColor3 = Color3.new(Sound.PlaybackLoudness/500,0,0)
			TextFrame.TextStrokeColor3 = Color3.new(0, 0, 0)
			TextFrame.Size = UDim2.new(1, 0, 0, 92)
			TextFrame.Position = UDim2.new(0, 0, 0, 0)
			local fvalen = 0.55
			local fval = -0.49
			coroutine.resume(coroutine.create(function()
				while true do
					swait()
					mainFrame.BackgroundColor3 = Color3.new(0,0,0)
					mainFrame.BorderColor3 = Color3.new(0, 0, 0)
					if(not droppingFrame)then
						mainFrame.Rotation = 0 - 2 * math.cos(SINE / 24)
					end
					TextFrame.TextStrokeTransparency = 1
				end
			end))
			for i = 1,string.len(whom),1 do
				TextFrame.Text = string.sub(whom,1,i)
				wait(0.1)
			end
			wait(0.1)
			droppingFrame = true
			mainFrame.Rotation = 0
			local vinc2 = 1
			for i = 0, 99 do
				swait()
				vinc2 = vinc2 + 0.25
				mainFrame.Position = mainFrame.Position + UDim2.new(0,0,0.0005*vinc2,0)
			end
			scrg:Destroy()
		end))
	end
end

function warnedkarma(whom)
	for i,v in pairs(game:GetService("Players"):GetPlayers()) do
		coroutine.resume(coroutine.create(function()
			if v.PlayerGui:FindFirstChild("ARRIVAL")~= nil then
				v.PlayerGui:FindFirstChild("ARRIVAL"):destroy()
			end
			local droppingFrame = false
			local scrg = Instance.new("ScreenGui",v.PlayerGui)
			scrg.Name = "ARRIVAL"
			local mainFrame = Instance.new("Frame", scrg)
			mainFrame.Name = "MainFrame"
			mainFrame.BackgroundTransparency = 1
			mainFrame.BorderSizePixel = 0
			mainFrame.Size = UDim2.new(1, 0, -0.013, 100)
			mainFrame.Position = UDim2.new(0, 0, 0.365, 0)
			local TextFrame = Instance.new("TextLabel",mainFrame)
			TextFrame.Name = "TextFrame"
			TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
			TextFrame.Text = ""
			TextFrame.TextScaled = true
			TextFrame.TextSize = 9
			TextFrame.TextStrokeTransparency = 1
			TextFrame.BackgroundTransparency = 1
			TextFrame.TextColor3 = BrickColor.Random().Color
			TextFrame.TextStrokeColor3 = BrickColor.Random().Color
			TextFrame.Size = UDim2.new(1, 0, 0, 92)
			TextFrame.Position = UDim2.new(0, 0, 0, 0)
			local fvalen = 0.55
			local fval = -0.49
			coroutine.resume(coroutine.create(function()
				while true do
					swait()
					TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
					TextFrame.TextColor3 = BrickColor.Random().Color
					mainFrame.BackgroundColor3 = Color3.new(0,0,0)
					mainFrame.BorderColor3 = Color3.new(0, 0, 0)
					if(not droppingFrame)then
				        TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
					    TextFrame.TextColor3 = BrickColor.Random().Color
						mainFrame.Rotation = 0 - 2 * math.cos(SINE / 24)
					end
					TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
					TextFrame.TextColor3 = BrickColor.Random().Color
					TextFrame.TextStrokeTransparency = 1
				end
			end))
			TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
			TextFrame.TextColor3 = BrickColor.Random().Color
			for i = 1,string.len(whom),1 do
		        TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
				TextFrame.Text = string.sub(whom,1,i)
				wait(0.25)
				TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
				TextFrame.TextColor3 = BrickColor.Random().Color
				TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
				TextFrame.TextColor3 = BrickColor.Random().Color
				TextFrame.Font = FONTS[MRANDOM(1, #FONTS)]
				TextFrame.TextColor3 = BrickColor.Random().Color
			end
			wait(0.1)
			droppingFrame = true
			mainFrame.Rotation = 0 - 2 * math.cos(SINE / 24)
			local vinc2 = 1
			for i = 0, 99 do
				swait()
				vinc2 = vinc2 + 0.25
				mainFrame.Position = mainFrame.Position + UDim2.new(0,0,0.0005*vinc2,0)
			end
			scrg:Destroy()
		end))
	end
end

game:GetService("StarterGui"):SetCore("SendNotification", { 
	    Title = "Converted by Epic";
	    Text = "Finally a script leak for so long";
	    Icon = "rbxthumb://type=Asset&id=1030775394&w=150&h=150"})
    Duration = 10

function warnedpeople(text)
	for i,v in pairs(game:GetService("Players"):GetPlayers()) do
		coroutine.resume(coroutine.create(function()
			if v.PlayerGui:FindFirstChild("Spinny")~= nil then
				v.PlayerGui:FindFirstChild("Spinny"):destroy()
			end
			local scrg = Instance.new("ScreenGui",v.PlayerGui)
			scrg.Name = "Spinny"
			local wobble = Instance.new("Frame",scrg)
			wobble.Name = "Wobble"
			wobble.BackgroundTransparency = 0.5
			wobble.Size = UDim2.new(1.1,0,1.1,0)
			wobble.Position = UDim2.new(-0.08,0,0.943,0)
			local wobble2 = Instance.new("Frame",scrg)
			wobble2.Name = "wobble2"
			wobble2.BackgroundTransparency = 0.5
			wobble2.Size = UDim2.new(1.1,0,0.09,0)
			wobble2.Position = UDim2.new(-0.08,0,0.878,0)
			local Visuals = Instance.new("Frame",scrg)
			Visuals.Name = "Visuals"
			Visuals.BackgroundTransparency = 0.3
			Visuals.Size = UDim2.new(0,100,0,100)
			Visuals.Position = UDim2.new(0.462,0,0.826,0)
			local glow = Instance.new("ImageLabel",scrg)
			glow.Name = "glow"
			glow.BackgroundTransparency = 1
			glow.ImageTransparency = 1
			glow.Image = "rbxassetid://2344870656"
			glow.Size = UDim2.new(0,0,0,0)
			glow.Position = UDim2.new(0.026,0,-0.235,0)
			local Visuals2 = Instance.new("Frame",scrg)
			Visuals2.Name = "Visuals2"
			Visuals2.BackgroundTransparency = 0.3
			Visuals2.Size = UDim2.new(0,50,0,50)
			Visuals2.Position = UDim2.new(0.48,0,0.867,0)
			local TextFrame = Instance.new("TextLabel",scrg)
			TextFrame.Name = "Farmer"
			TextFrame.Font = "Arcade"
			TextFrame.Text = text
			TextFrame.TextScaled = true
			TextFrame.TextSize = 60
			TextFrame.BackgroundTransparency = 1
			TextFrame.Size = UDim2.new(0.8,0,0,42)
			TextFrame.Position = UDim2.new(0.11,0,0.867,0)
			local fvalen = 0.55
			local fval = -0.49
			coroutine.resume(coroutine.create(function()
				while true do
					swait()
					TextFrame.TextColor3 = Color3.new(0.4,0,0)
					TextFrame.TextStrokeColor3 = Color3.new(0, 0, 0)
					TextFrame.TextStrokeTransparency = 1
					TextFrame.Rotation = 0 + MRANDOM(-3, 3)
					TextFrame.Position = UDim2.new(0.11, 0 + MRANDOM(-3, 3), 0.867, 0 + MRANDOM(-3, 3))
					TextFrame.Font = Enum.Font.Arcade
					glow.ImageColor3 = Color3.new(0, 0, 0)
					wobble.Rotation = 0 - 2 * math.cos(SINE / 24)
					wobble2.Rotation = 0 - 2 * math.cos(SINE / 30)
					wobble2.BackgroundColor3 = Color3.new(0.1,0.1,0.1)
					wobble2.BorderColor3 = Color3.new(0.4,0,0)
					wobble2.BorderSizePixel = 2
					Visuals.Rotation = Visuals.Rotation + MRANDOM(-5, 5)
					Visuals2.Rotation = Visuals2.Rotation + MRANDOM(-10, 10)
					Visuals.BackgroundColor3 = Color3.new(0.1,0.1,0.1)
					Visuals.BorderColor3 = Color3.new(0.4,0,0)
					Visuals2.BackgroundColor3 = Color3.new(0.1,0.1,0.1)
					Visuals2.BorderColor3 = Color3.new(0.4,0,0)
					wobble.BackgroundColor3 = Color3.new(0.1,0.1,0.1)
					wobble.BorderColor3 = Color3.new(0.4,0,0)
					wobble.BorderSizePixel = 2
				end
			end))
			coroutine.resume(coroutine.create(function()
				for i = 0, 205 do
					swait()
				end
				scrg:Destroy()
			end))
		end))
	end
end


function ApplyAoEpp(POSITION,RANGE)
	for index, CHILD in pairs(workspace:GetDescendants()) do
		if CHILD.ClassName == "Model" and CHILD ~= Character then
			local HUM = CHILD:FindFirstChildOfClass("Humanoid")
			if HUM then
				local TORSO = CHILD:FindFirstChild("Torso") or CHILD:FindFirstChild("UpperTorso")
				if TORSO then
					if (TORSO.Position - POSITION).Magnitude <= RANGE then
						Killpp(CHILD)
					end
				end
			end
		end
	end
end

function MagicSpherepp(size,waitt,cframe,color)
	local wave = CreatePart(3, Effects, "Neon", 0, 1, BRICKC(color), "Effect", Vector3.new(1,1,1))
	local mesh = IT("SpecialMesh",wave)
	mesh.MeshType = "Sphere"
	mesh.Scale = Vector3.new(size,size,size)
	mesh.Offset = Vector3.new(0,0,0)
	wave.CFrame = cframe
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, waitt do
			swait()
			mesh.Scale = mesh.Scale - Vector3.new(size/waitt,size/waitt,size/waitt)
			wave.Transparency = wave.Transparency - (1/waitt)
		end
		wave:remove()
	end))
end

function CheckTableForString(Table, String)
	for i, v in pairs(Table) do
		if string.find(string.lower(String), string.lower(v)) then
			return true
		end
	end
	return false
end

function CheckIntangible(Hit)
	local ProjectileNames = {"Water", "Arrow", "Projectile", "Effect", "Rail", "Lightning", "Bullet"}
	if Hit and Hit.Parent then
		if ((not Hit.CanCollide or CheckTableForString(ProjectileNames, Hit.Name)) and not Hit.Parent:FindFirstChild("Humanoid")) then
			return true
		end
	end
	return false
end

function CastZapRay(StartPos, Vec, Length, Ignore, DelayIfHit)
	local Direction = CFrame.new(StartPos, Vec).lookVector
	local Ignore = ((type(Ignore) == "table" and Ignore) or {Ignore})
	local RayHit, RayPos, RayNormal = game:GetService("Workspace"):FindPartOnRayWithIgnoreList(Ray.new(StartPos, Direction * Length), Ignore)
	if RayHit and CheckIntangible(RayHit) then
		if DelayIfHit then
			wait()
		end
		RayHit, RayPos, RayNormal = CastZapRay((RayPos + (Vec * 0.01)), Vec, (Length - ((StartPos - RayPos).magnitude)), Ignore, DelayIfHit)
	end
	return RayHit, RayPos, RayNormal
end

function CreateRing(SIZE,DOESROT,ROT,WAIT,CFRAME,COLOR,GROW)
	local wave = CreatePart(3, Effects, "Neon", 0, 0.5, BRICKC(COLOR), "Effect", VT(0,0,0))
	local mesh = IT("SpecialMesh",wave)
	mesh.MeshType = "FileMesh"
	mesh.MeshId = "http://www.roblox.com/asset/?id=3270017"
	mesh.Scale = SIZE
	mesh.Offset = VT(0,0,0)
	wave.CFrame = CFRAME
	coroutine.resume(coroutine.create(function(PART)
		for i = 1, WAIT do
			Swait()
			mesh.Scale = mesh.Scale + GROW
			if DOESROT == true then
				wave.CFrame = wave.CFrame * CFrame.fromEulerAnglesXYZ(0,ROT,0)
			end
			wave.Transparency = wave.Transparency + (0.5/WAIT)
			if wave.Transparency > 0.99 then
				wave:remove()
			end
		end
	end))
end

function WACKYEFFECTpp(Table)
	local TYPE = Table.EffectType or "Sphere"
	local SIZE = Table.Size or Vector3.new(1, 1, 1)
	local ENDSIZE = Table.Size2 or Vector3.new(0, 0, 0)
	local TRANSPARENCY = Table.Transparency or 0
	local ENDTRANSPARENCY = Table.Transparency2 or 1
	local CFRAME = Table.CFrame or Torso.CFrame
	local MOVEDIRECTION = Table.MoveToPos or nil
	local ROTATION1 = Table.RotationX or 0
	local ROTATION2 = Table.RotationY or 0
	local ROTATION3 = Table.RotationZ or 0
	local MATERIAL = Table.Material --or "Neon"
	local COLOR = Table.Color or Color3.new(1, 1, 1)
	local TIME = Table.Time or 45
	local SOUNDID = Table.SoundID or nil
	local SOUNDPITCH = Table.SoundPitch or nil
	local SOUNDVOLUME = Table.SoundVolume or nil
	local USEBOOMERANGMATH = Table.UseBoomerangMath or false
	local BOOMERANG = Table.Boomerang or 0
	local SIZEBOOMERANG = Table.SizeBoomerang or 0
	coroutine.resume(coroutine.create(function()
		local PLAYSSOUND = false
		local SOUND
		local EFFECT = CreatePart(3, Effects, MATERIAL, 0, TRANSPARENCY, BRICKC("Pearl"), "Effect", Vector3.new(1, 1, 1), true)
		if SOUNDID ~= nil and SOUNDPITCH ~= nil and SOUNDVOLUME ~= nil then
			PLAYSSOUND = true
			SOUND = CreateSound(SOUNDID, EFFECT, SOUNDVOLUME, SOUNDPITCH, false)
		end
		EFFECT.Color = COLOR
		local MSH
		if TYPE == "Sphere" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "Sphere", "", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Block" or TYPE == "Box" then
			MSH = IT("BlockMesh", EFFECT)
			MSH.Scale = SIZE
		elseif TYPE == "Wave" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "20329976", "", SIZE, Vector3.new(0, 0, -SIZE.X / 8))
		elseif TYPE == "Ring" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "559831844", "", Vector3.new(SIZE.X, SIZE.X, 0.1), Vector3.new(0, 0, 0))
		elseif TYPE == "Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662586858", "", Vector3.new(SIZE.X / 10, 0, SIZE.X / 10), Vector3.new(0, 0, 0))
		elseif TYPE == "Round Slash" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "662585058", "", Vector3.new(SIZE.X / 10, 0, SIZE.X / 10), Vector3.new(0, 0, 0))
		elseif TYPE == "Swirl" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "168892432", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Skull" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "4770583", "", SIZE, Vector3.new(0, 0, 0))
		elseif TYPE == "Star" then 
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "2760116123", "", SIZE, Vector3.new(0,0,0))   	
		elseif TYPE == "Crystal" then
			MSH = CreateMesh2("SpecialMesh", EFFECT, "FileMesh", "450656451", "", SIZE, Vector3.new(0, 0, 0))
		end
		coroutine.resume(coroutine.create(function()
			if MSH ~= nil then
				local BOOMR1 = 1 + BOOMERANG / 50
				local BOOMR2 = 1 + SIZEBOOMERANG / 50
				local MOVESPEED = nil
				if MOVEDIRECTION ~= nil then
					MOVESPEED = (CFRAME.p - MOVEDIRECTION).Magnitude/TIME
				end
				local GROWTH
				if USEBOOMERANGMATH == true then
					GROWTH = (SIZE - ENDSIZE) * (BOOMR2 + 1)
				else
					GROWTH = SIZE - ENDSIZE
				end
				local TRANS = TRANSPARENCY - ENDTRANSPARENCY
				if TYPE == "Block" then
					EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
				else
					EFFECT.CFrame = CFRAME
				end
				if USEBOOMERANGMATH == true then
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - Vector3.new(GROWTH.X * (1 - LOOP / TIME * BOOMR2), GROWTH.Y * (1 - LOOP / TIME * BOOMR2), GROWTH.Z * (1 - LOOP / TIME * BOOMR2)) * BOOMR2 / TIME
						if TYPE == "Wave" then
							MSH.Offset = Vector3.new(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * CFrame.Angles(math.rad(ROTATION1), math.rad(ROTATION2), math.rad(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CF(EFFECT.Position, MOVEDIRECTION) * CFrame.new(0, 0, -MOVESPEED * (1 - LOOP / TIME * BOOMR1))
							EFFECT.Orientation = ORI
						end
					end
				else
					for LOOP = 1, TIME + 1 do
						swait()
						MSH.Scale = MSH.Scale - GROWTH / TIME
						if TYPE == "Wave" then
							MSH.Offset = Vector3.new(0, 0, -MSH.Scale.Z / 8)
						end
						EFFECT.Transparency = EFFECT.Transparency - TRANS / TIME
						if TYPE == "Block" then
							EFFECT.CFrame = CFRAME * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)))
						else
							EFFECT.CFrame = EFFECT.CFrame * CFrame.Angles(math.rad(ROTATION1), math.rad(ROTATION2), math.rad(ROTATION3))
						end
						if MOVEDIRECTION ~= nil then
							local ORI = EFFECT.Orientation
							EFFECT.CFrame = CFrame.new(EFFECT.Position,MOVEDIRECTION)*CFrame.new(0,0,-MOVESPEED)
							EFFECT.Orientation = ORI
						end
					end
				end
				EFFECT.Transparency = 1
				if PLAYSSOUND == false then
					EFFECT:remove()
				else
					repeat
						swait()
					until EFFECT:FindFirstChildOfClass("Sound") == nil
					EFFECT:remove()
				end
			elseif PLAYSSOUND == false then
				EFFECT:remove()
			else
				repeat
					swait()
				until EFFECT:FindFirstChildOfClass("Sound") == nil
				EFFECT:remove()
			end
		end))
		return EFFECT
	end))
end   

function Killpp(dude)
	--[[]]
end

function chatfunc(text)
	local chat = coroutine.wrap(function()
		local oldthing = RealRoot:FindFirstChild("TalkingBillBoard")
		if oldthing then
			oldthing:Destroy()
		end
		local naeeym2 = Instance.new("BillboardGui",RealRoot)
		naeeym2.Size = UDim2.new(0,9999,2,0)
		naeeym2.StudsOffset = Vector3.new(0,4.5,0)
		naeeym2.Adornee = Character.HumanoidRootPart
		naeeym2.Name = "TalkingBillBoard"
		local tecks2 = Instance.new("TextLabel",naeeym2)
		tecks2.BackgroundTransparency = 1
		tecks2.BorderSizePixel = 0
		tecks2.Text = ""
		tecks2.Font = "SciFi"
		tecks2.TextScaled = true
		tecks2.TextStrokeTransparency = 0
		coroutine.resume(coroutine.create(function()
			while tecks2:IsDescendantOf(game) do
				local hBRUH,sBRUH,vBRUH = Color3.toHSV(Torso.NeonParts.Color)
				tecks2.TextColor3 = Color3.fromHSV(hBRUH,sBRUH,vBRUH/2)
				swait()
			end
		end))
		tecks2.TextStrokeColor3 = shade
		tecks2.Size = UDim2.new(1,0,1,0)
		local tecks3 = Instance.new("TextLabel",naeeym2)
		tecks3.BackgroundTransparency = 1
		tecks3.BorderSizePixel = 0
		tecks3.Text = ""
		tecks3.Font = "Antique"
		tecks3.TextScaled = true
		tecks3.TextStrokeTransparency = 0
		coroutine.resume(coroutine.create(function()
			while tecks3:IsDescendantOf(game) do
				tecks3.TextColor3 = Torso.NeonParts.Color
				swait()
			end
		end))
		tecks3.TextStrokeColor3 = shade
		tecks3.Size = UDim2.new(1,0,1,0)
		coroutine.resume(coroutine.create(function()
			while naeeym2 ~= nil do
				swait()
				tecks2.Position = UDim2.new(0,math.random(-3,3),0,math.random(-3,3)) 
				tecks3.Position = UDim2.new(0,math.random(-3,3),0,math.random(-3,3)) 
				
			end
		end))
		for i = 1,string.len(text) do
			CreateSound(4740147336,RealRoot,5,1)
			swait(2)
			tecks2.Text = string.sub(text,1,i)
			tecks3.Text = string.sub(text,1,i)
		end
		swait(120)
		for i = 1,50 do
			swait()
			tecks2.Position = tecks2.Position - UDim2.new(0,math.random(-3,3),0,math.random(-3,3))
			tecks3.Position = tecks2.Position - UDim2.new(0,math.random(-3,3),0,math.random(-3,3)) 
			tecks2.Rotation = tecks2.Rotation + math.random(-2,2)
			tecks3.Rotation = tecks3.Rotation + math.random(-2,2)
			tecks2.TextStrokeTransparency = i/50
			tecks2.TextTransparency = tecks2.TextStrokeTransparency
			tecks3.TextStrokeTransparency = tecks2.TextStrokeTransparency
			tecks3.TextTransparency = tecks2.TextStrokeTransparency
		end
		naeeym2:Destroy()
	end)
	--chat()
end
function onChatted(msg)
	chatfunc(msg)
end

Player.Chatted:connect(onChatted)

function CreateWeld(parent,part0,part1,C1X,C1Y,C1Z,C1Xa,C1Ya,C1Za,C0X,C0Y,C0Z,C0Xa,C0Ya,C0Za)
	local weld = Instance.new("Weld")
	weld.Parent = parent
	weld.Part0 = part0
	weld.Part1 = part1
	weld.C1 = CFrame.new(C1X,C1Y,C1Z)*CFrame.Angles(C1Xa,C1Ya,C1Za)
	weld.C0 = CFrame.new(C0X,C0Y,C0Z)*CFrame.Angles(C0Xa,C0Ya,C0Za)
	return weld
end


--//=================================\\
--||	ATTACK FUNCTIONS AND STUFF
--\\=================================//

function SnakeGod()
	ATTACK = true
	Rooted = true
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-50)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(60)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(-25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-90)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(90)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-50)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(60)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(-25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-90)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(90)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-50)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(60)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 10, 1, false)
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0 + 0.35 * math.cos(SINE / 2)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0 + ((1) - 1)) * CFrame.Angles(math.rad(5), math.rad(-25), math.rad(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.25, 0.5, -0.5) * CFrame.Angles(math.rad(100), math.rad(0), math.rad(-90)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.25, 0.35, -0.35) * CFrame.Angles(math.rad(70), math.rad(0), math.rad(90)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1 - 0.35 * math.cos(SINE / 2), -0.01) * CFrame.Angles(math.rad(0), math.rad(-90), math.rad(0)) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(0)), 0.15 / Animation_Speed)
	end
	local HITFLOOR,HITPOS = Raycast(RootPart.Position, (CFrame.new(RootPart.Position, RootPart.Position + Vector3.new(0, -1, 0))).lookVector, 25*SIZE, Character)
	WACKYEFFECT({Time = 60, EffectType = "Wave", Size = Vector3.new(12,0.55,12)*SIZE, Size2 = Vector3.new(12,0.55,12), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(HITPOS), MoveToPos = nil, RotationX = 0, RotationY = 15, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = 1, SoundVolume = 6})

	WACKYEFFECT({Time = 60, EffectType = "Sphere", Size = Vector3.new(0.5,0.55,0.5), Size2 = Vector3.new(0.5,4,0.5), Transparency = 0, Transparency2 = 1, CFrame = Head.CFrame*CFrame.new(0.4, 0.2, -0.8), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1, 0, 0), SoundID = 743521450, SoundPitch = 1.15, SoundVolume = 6})
	WACKYEFFECT({Time = 60, EffectType = "Sphere", Size = Vector3.new(0.55,0.5,0.5), Size2 = Vector3.new(4,0.5,0.5), Transparency = 0, Transparency2 = 1, CFrame = Head.CFrame*CFrame.new(0.4, 0.2, -0.8), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1, 0, 0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	
	WACKYEFFECT({Time = 150, EffectType = "Wave", Size = Vector3.new(62,35,62)*SIZE, Size2 = Vector3.new(62,35,62), Transparency = 1, Transparency2 = 1, CFrame = CFrame.new(HITPOS), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 1259054947, SoundPitch = 1, SoundVolume = 6})

	WACKYEFFECT({Time = 180, EffectType = "Block", Size = Vector3.new(24,24,24)*1.5, Size2 = Vector3.new(0,8,0), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame*CFrame.new(0,-1,0)*CFrame.Angles(math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = BrickColor.new"Really black".Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})
	MODE = "Snake God"
	Sound.SoundId = syn and getsynasset('Eminem%20_%20Godzilla%20%28Lyrics%29%20FT.%20Juice%20WRLD.mp3') or getcustomasset('Eminem%20_%20Godzilla%20%28Lyrics%29%20FT.%20Juice%20WRLD.mp3')
    Sound.Volume = 5
    Sound.TimePosition = "2.2"
    Sound.Pitch = 1
    Sound.Looped = true
    Sound:Play()
	ATTACK = false
	Rooted = false
	
	
	
end

function Spooky() 
	ATTACK = true
	Rooted = true
	for i = 0, 4, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.15,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-15),RAD(-20)),.1)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.1)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,0.25,-0.05) * ANGLES(RAD(-20),RAD(0),RAD(30)),.1)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-30)),.1)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.8,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(30)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-5),RAD(10),RAD(-20)),.1)
	end

	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(150,5,150), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(160,10,160), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 1, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(170,5,170), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 2, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(180,10,180), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 3, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(190,5,190), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 4, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(200,10,200), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	for i = 0, 2, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.5,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-25),RAD(30)),.8)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.8)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,-0.25,-0.5) * ANGLES(RAD(30),RAD(0),RAD(50)),.8)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-50)),.8)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.6,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(75)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-35),RAD(10),RAD(-50)),.8)
	end
	MODE = "Scary"
	Sound.SoundId = syn and getsynasset('SpookyRemix.mp3') or getcustomasset('SpookyRemix.mp3')
    Sound.Volume = 4
    Sound.TimePosition = "1"
    Sound.Pitch = 1
    Sound.Looped = true
    Sound:Play()
	ATTACK = false
	Rooted = false
	
end

function test() 
	ATTACK = true
	Rooted = true
	for i = 0, 4, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.15,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-15),RAD(-20)),.1)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.1)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,0.25,-0.05) * ANGLES(RAD(-20),RAD(0),RAD(30)),.1)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-30)),.1)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.8,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(30)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-5),RAD(10),RAD(-20)),.1)
	end
	CreateSound(824687369, Torso, 10, 0.9, false)
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(150,5,150), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(160,10,160), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 1, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(170,5,170), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 2, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(180,10,180), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 3, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(190,5,190), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 4, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(200,10,200), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	for i = 0, 2, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.5,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-25),RAD(30)),.8)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.8)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,-0.25,-0.5) * ANGLES(RAD(30),RAD(0),RAD(50)),.8)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-50)),.8)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.6,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(75)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-35),RAD(10),RAD(-50)),.8)
	end
	MODE = "test"
	Sound.SoundId = syn and getsynasset('BWater.mp3') or getcustomasset('BWater.mp3')
    Sound.Volume = 4
    Sound.Pitch = 0.98
    Sound.TimePosition = "1"
    Sound.Looped = true
    Sound:Play()
	ATTACK = false
	Rooted = false

end

function NIGHTMARE()
	ATTACK = true
	Rooted = true
	for i = 0, 4, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.15,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-15),RAD(-20)),.1)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.1)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,0.25,-0.05) * ANGLES(RAD(-20),RAD(0),RAD(30)),.1)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-30)),.1)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.8,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(30)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-5),RAD(10),RAD(-20)),.1)
	end
	CreateSound(824687369, Torso, 10, 0.9, false)
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(150,5,150), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(160,10,160), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 1, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(170,5,170), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 2, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(180,10,180), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 3, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(190,5,190), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 4, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(200,10,200), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	for i = 0, 2, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.5,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-25),RAD(30)),.8)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.8)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,-0.25,-0.5) * ANGLES(RAD(30),RAD(0),RAD(50)),.8)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-50)),.8)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.6,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(75)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-35),RAD(10),RAD(-50)),.8)
	end
	MODE = "ByeBye"
	Sound.SoundId = syn and getsynasset('ByeBye.mp3') or getcustomasset('ByeBye.mp3')
    Sound.Volume = 8.5
    Sound.Pitch = "0.55"
    Sound.PlaybackSpeed = "0.9"
    Sound.TimePosition = "136"
    Sound.Looped = true
    Sound:Play()
	ATTACK = false
	Rooted = false
	
	
	
end

function katana() 
	ATTACK = true
	Rooted = true
	for i = 0, 4, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.15,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-15),RAD(-20)),.1)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.1)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,0.25,-0.05) * ANGLES(RAD(-20),RAD(0),RAD(30)),.1)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-30)),.1)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.8,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(30)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-5),RAD(10),RAD(-20)),.1)
	end
	CreateSound(824687369, Torso, 10, 0.9, false)
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(150,5,150), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(160,10,160), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 1, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(170,5,170), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 2, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(180,10,180), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 3, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(190,5,190), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 4, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	WACKYEFFECT({Time = 50, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(200,10,200), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,0,1), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil , SoundPitch = 1.2, SoundVolume = 4})
	for i = 0, 2, 0.1 do
		swait()
		RightHip.C0 = Clerp(RightHip.C0, CF(1,-0.5,-0.5) * ANGLES(RAD(0),RAD(90),RAD(0)) * ANGLES(RAD(-3),RAD(-25),RAD(30)),.8)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1,-1,0) * ANGLES(RAD(0),RAD(-90),RAD(0)) * ANGLES(RAD(-3),RAD(1),RAD(20)),.8)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0,-0.25,-0.5) * ANGLES(RAD(30),RAD(0),RAD(50)),.8)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * ANGLES(RAD(20),RAD(0),RAD(-50)),.8)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.45,0.6,-0.15) * ANGLES(RAD(35),RAD(-10),RAD(75)),.8)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4,0.5,0.1) * ANGLES(RAD(-35),RAD(10),RAD(-50)),.8)
	end
	MODE = "Katana"
	Character["Back_AccAccessory"].Handle.att3_Handle.Parent = RightArm
    RightArm.att3_Handle.Rotation = Vector3.new(-125, -85, 180)
    RightArm.att3_Handle.Position = Vector3.new(-0.1, -0.7, -1.8)
	Sound.SoundId = syn and getsynasset('Heavensent.mp3') or getcustomasset('Heavensent.mp3')
    Sound.Volume = 4.5
    Sound.TimePosition = "8.2"
    Sound.Pitch = 1
    Sound.Looped = true
    Sound:Play()
	ATTACK = false
	Rooted = false
	
	
	
end

function memeGod() 
	ATTACK = true
	Rooted = true
	
	
	Sound.SoundId = syn and getsynasset('RewindTimeSand.mp3') or getcustomasset('RewindTimeSand.mp3')
    Sound.Volume = 4
    Sound.TimePosition = "1"
    Sound.Pitch = 1
    Sound.Looped = true
    Sound:Play()
	for i = 0, 9, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(0.75, 0.5 + 0.05 * SIN(SINE / 12), -0.7) * ANGLES(RAD(0), RAD(0), RAD(-95)) * ANGLES(RAD(5), RAD(90), RAD(0)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-0.75, 0.35 + 0.05 * SIN(SINE / 12), -0.6) * ANGLES(RAD(0), RAD(0), RAD(92)) * ANGLES(RAD(0), RAD(90), RAD(0)) * LEFTSHOULDERC0, 1 / Animation_Speed)
	end
	MODE = "meme"
	warnedpeople("Now Concentrate")
	wait(0.5)
	for i = 0, 9, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0 * Sin(SINE / 30), 0.025 * Cos(SINE / 20)) * RIGHTSHOULDERC0 * angles(Rad(0), Rad(0), Rad(90)), 0.1)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-12)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
	end
	warnedpeople("On how it makes you feel")
	wait(2.3)
	warnedpeople("Now let your hand drift across the canvas")
	wait(1)
	warnedpeople2("Rewind Time Everybody.")
	ATTACK = false
	Rooted = false
	refec.Enabled = false
end

function karma()
	ATTACK = true
	Rooted = true
	Character.Humanoid.WalkSpeed = 0
    
	for i=0, 0.3, 0.01 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(12)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-12)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
	end
	warnedpeople("But RAGE.")
	
	for i=0, 0.6, 0.01 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(30+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15))), 0.35 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(160+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(-30+MRANDOM(-15,15)))* RIGHTSHOULDERC0, 0.35 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(160+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(30+MRANDOM(-15,15))) * LEFTSHOULDERC0, 0.35 / Animation_Speed)
	end
	
	for i=0, 0.6, 0.01 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 , 0 , -0.7) * ANGLES(RAD(MRANDOM(-15,15)), RAD(MRANDOM(-15,15)), RAD(MRANDOM(-15,15))), 0.35 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(30+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15))), 0.35 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(160+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(-30+MRANDOM(-15,15)))* RIGHTSHOULDERC0, 0.35 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(160+MRANDOM(-15,15)), RAD(0+MRANDOM(-15,15)), RAD(30+MRANDOM(-15,15))) * LEFTSHOULDERC0, 0.35 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5, -0.5) * ANGLES(RAD(0), RAD(0), RAD(0)) * ANGLES(RAD(0), RAD(90), RAD(0)), 0.35 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 , 0) * ANGLES(RAD(-60), RAD(0), RAD(0)) * ANGLES(RAD(0), RAD(-90), RAD(0)), 0.35 / Animation_Speed)
	end
	ShakeCam(2,100)
	Character.Humanoid.WalkSpeed = 18
	MODE = "Suffering"
	ATTACK = false
	Rooted = false
	

end

function h3ll()
	ATTACK = true
	Rooted = true
	MODE = "HELL"
	Sound.SoundId = syn and getsynasset('StrongerThanYou.mp3') or getcustomasset('StrongerThanYou.mp3')
    Sound.Volume = 4
    Sound.TimePosition = "0"
    Sound.Pitch = 1
    Sound.Looped = true
    Sound:Play()
	for i = 0, 9, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(0.75, 0.5 + 0.05 * SIN(SINE / 12), -0.7) * ANGLES(RAD(0), RAD(0), RAD(-95)) * ANGLES(RAD(5), RAD(90), RAD(0)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-0.75, 0.35 + 0.05 * SIN(SINE / 12), -0.6) * ANGLES(RAD(0), RAD(0), RAD(92)) * ANGLES(RAD(0), RAD(90), RAD(0)) * LEFTSHOULDERC0, 1 / Animation_Speed)
	end
	warnedpeople("It's a beautiful day outside.")
	wait(1.3)
	warnedpeople("Birds are singing, flowers are blooming")
	wait(2.1)
	warnedpeople("On days like this.. Kids like you..")
	wait(0.6)
	for i = 0, 9, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0 * Sin(SINE / 30), 0.025 * Cos(SINE / 20)) * RIGHTSHOULDERC0 * angles(Rad(0), Rad(0), Rad(90)), 0.1)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-12)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
	end
	warnedpeople2("Should be burning in hell.")
	wait(1.9)
	for i = 0, 9, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, -0.1 + 0.1 * Cos(SINE / 20)) * angles(Rad(0), Rad(0), Rad(0)), 0.15/3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * angles(Rad(0), Rad(0), Rad(0)), 0.3/3)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, 1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.9 - 0.1 * Cos(SINE / 20), 0.025 * Cos(SINE / 20)) * Euler(0, -1.6, 0) * angles(Rad(-2.5), Rad(0), Rad(0)), 0.15/3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(12)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-12)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
	end
	ATTACK = false
	Rooted = false
	warnedpeople("Turn around kid, It'd be a crime.")
	wait(2.75)
	warnedpeople("I'd don't wanna have to go back on the promise I made for you.")
	wait(3)
	warnedpeople("So don't step over that line.")
	wait(1.8)
	warnedpeople("A real strain you're gonna have a bad time")
	wait(2.5)
	warnedpeople("but kids like you don't play by the rules")
	wait(2)
	warnedpeople("but guys like me, it ant easy to be played for fools")
	wait(2.1)
	warnedpeople("So, let's go, let the room get chiller")
	wait(2.4)
	warnedpeople("Let's go, dirty brother killer")
	wait(8.5)
	warnedpeople2("But i think you'll just keep dying.")
end

function sit()
	ATTACK = true
	Rooted = true
	local LOOP = true
	KEY = Mouse.KeyDown:connect(function(NEWKEY)
		if NEWKEY == "n" then
			KEY:Disconnect()
			LOOP = false
		end
	end)
	repeat
		for i = 0, 0.4, 0.1 / Animation_Speed do
			swait()
			if LOOP == false then
				break
			end
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, -1.70) * ANGLES(RAD(-40), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.3, 0.10) * ANGLES(RAD(-40), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
			LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.3, 0.10) * ANGLES(RAD(-40), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
			RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(45), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(45), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		end
	until LOOP == false
	ATTACK = false
	Rooted = false
end

function fuck_it()
	ATTACK = true
	Rooted = true
	for i=0, 1.2, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(35), RAD(0), RAD(0)), 0.25 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.25) - 1)) * ANGLES(RAD(35), RAD(0), RAD(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.3, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(200)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.3, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-200)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5 - 0.05 * COS(SINE / 12), -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.8 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 6, 1, false)
	for i=0, 1, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(35), RAD(0), RAD(0)), 0.25 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.25) - 1)) * ANGLES(RAD(35), RAD(0), RAD(25)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.3, 0.5, 0) * ANGLES(RAD(-40), RAD(50), RAD(200)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.3, 0.5, 0) * ANGLES(RAD(40), RAD(50), RAD(-200)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5 - 0.05 * COS(SINE / 12), -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.8 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end	
	for i=0, 1, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(35), RAD(0), RAD(0)), 0.25 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.25) - 1)) * ANGLES(RAD(35), RAD(0), RAD(-25)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.3, 0.5, 0) * ANGLES(RAD(40), RAD(-50), RAD(200)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.3, 0.5, 0) * ANGLES(RAD(-40), RAD(-50), RAD(-200)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5 - 0.05 * COS(SINE / 12), -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.8 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	CreateSound(363808674, Torso, 6, 1, false)
	WACKYEFFECT({Time = 85, EffectType = "Block", Size = VT(0.55,0.55,0.55), Size2 = VT(55,55,55), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0)*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = BRICKC"Really red".Color, SoundID = 743499393, SoundPitch = 0.8, SoundVolume = 10})
	for i=0, 0.5, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(35), RAD(0), RAD(0)), 0.25 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.25) - 1)) * ANGLES(RAD(-35), RAD(0), RAD(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(-40), RAD(0), RAD(40)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-40), RAD(0), RAD(-40)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5 - 0.05 * COS(SINE / 12), -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.8 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	WACKYEFFECT({Time = 120, EffectType = "Swirl", Size = Vector3.new(40.55,40.55,40.55), Size2 = Vector3.new(95,95,95), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 120, EffectType = "Slash", Size = Vector3.new(3.55,3.5,3.5), Size2 = Vector3.new(130,3.5,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 120, EffectType = "Slash", Size = Vector3.new(3.5,3.5,3.55), Size2 = Vector3.new(3.5,3.5,130), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 120, EffectType = "Swirl", Size = Vector3.new(3.5,3.55,3.5), Size2 = Vector3.new(3.5,130,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 55, EffectType = "Sphere", Size = Vector3.new(3.55,3.55,3.55), Size2 = Vector3.new(95,95,95), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.55,3.5,3.5), Size2 = Vector3.new(130,3.5,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.5,3.55), Size2 = Vector3.new(3.5,3.5,130), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.55,3.5), Size2 = Vector3.new(3.5,130,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	wait(0.8)
	WACKYEFFECT({Time = 55, EffectType = "Sphere", Size = Vector3.new(3.55,3.55,3.55), Size2 = Vector3.new(95,95,95), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.55,3.5,3.5), Size2 = Vector3.new(130,3.5,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.5,3.55), Size2 = Vector3.new(3.5,3.5,130), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.55,3.5), Size2 = Vector3.new(3.5,130,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	wait(0.8)
	WACKYEFFECT({Time = 55, EffectType = "Sphere", Size = Vector3.new(3.55,3.55,3.55), Size2 = Vector3.new(95,95,95), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.55,3.5,3.5), Size2 = Vector3.new(130,3.5,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.5,3.55), Size2 = Vector3.new(3.5,3.5,130), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.55,3.5), Size2 = Vector3.new(3.5,130,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	wait(0.8)
	WACKYEFFECT({Time = 55, EffectType = "Sphere", Size = Vector3.new(3.55,3.55,3.55), Size2 = Vector3.new(95,95,95), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 743521450, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.55,3.5,3.5), Size2 = Vector3.new(130,3.5,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.5,3.55), Size2 = Vector3.new(3.5,3.5,130), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	WACKYEFFECT({Time = 70, EffectType = "Sphere", Size = Vector3.new(3.5,3.55,3.5), Size2 = Vector3.new(3.5,130,3.5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0, 0, 0), MoveToPos = nil, RotationX = 30, RotationY = 30, RotationZ = 30, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 0, SoundPitch = 0.95, SoundVolume = 6})
	
	
	MODE = "fuck"
	
	ATTACK = false
	Rooted = false
	
	
	
end

local ULTTAUNTS = {
	"907332997",
	"907332670",
	"907330103"
}

function Penumbric_DeathRay2()
	ATTACK = true
	local GYRO = IT("BodyGyro", RootPart)
	GYRO.D = 15
	GYRO.P = 2000
	GYRO.MaxTorque = VT(0, 4000000, 0)
	repeat
		local HIT,POS = CastProperRay(RightArm.Position, Mouse.Hit.p, 1000, Character)
		SpawnTrail3(RightArm.Position,POS)
		if HIT ~= nil then
			if HIT.Parent ~= workspace and HIT.Parent.ClassName ~= "Folder" then
				AOETime2(POS,55)
			end
		end
		AOETime2(POS,8)
		for i=0, 0.2, 0.1 / Animation_Speed do
			swait()
			Humanoid.CameraOffset = VT(MRANDOM(-50,50)/2.5,MRANDOM(-50,50)/2.5,MRANDOM(-50,50)/2.5)/30
			GYRO.cframe = CF(RootPart.Position, Mouse.Hit.p)
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(90)), 0.5 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-90)), 0.5 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90), RAD(0), RAD(90)) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
			LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5*SIZE, 0.5*SIZE, 0*SIZE) * ANGLES(RAD(0), RAD(0), RAD(-5)) * LEFTSHOULDERC0, 0.8 / Animation_Speed)
			RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		end
		WACKYEFFECT6({Time = 25, EffectType = "Box", Size = VT(2,0,2), Size2 = VT(6,7.5,6)/2, Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = RightArm.CFrame*CF(0,0,0).p, RotationX = 0, RotationY = -15, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		WACKYEFFECT6({Time = 25, EffectType = "Box", Size = VT(2,0,2), Size2 = VT(6,6.5,6)/2, Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 231917744, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 5})
		WACKYEFFECT6({Time = 25, EffectType = "Box", Size = VT(3,0,3), Size2 = VT(6,6.5,6), Transparency = 0, Transparency2 = 1, CFrame = CF(POS,RightArm.Position) * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = nil, RotationX = 0, RotationY = -5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT6({Time = 25, EffectType = "Box", Size = VT(3,0,3), Size2 = VT(6,6.5,6), Transparency = 0, Transparency2 = 1, CFrame = CF(POS,RightArm.Position) * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT6({Time = 25, EffectType = "Round Slash", Size = VT(1,0,1)/74, Size2 = VT(4,4.5,4)/74, Transparency = 0, Transparency2 = 1, CFrame = CF(POS,RightArm.Position) * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = nil, RotationX = 0, RotationY = -5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8, UseBoomerangMath = true, Boomerang = 12, SizeBoomerang = 45})
		WACKYEFFECT6({Time = 25, EffectType = "Round Slash", Size = VT(1,0,1)/74, Size2 = VT(4,4.5,4)/74, Transparency = 0, Transparency2 = 1, CFrame = CF(POS,RightArm.Position) * ANGLES(RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360)), RAD(MRANDOM(-360,360))), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8, UseBoomerangMath = true, Boomerang = 12, SizeBoomerang = 45})
	until KEYHOLD == false
	Humanoid.CameraOffset = VT(0,0,0)
	GYRO:remove()	
	ATTACK = false
end

function Karma_Beam()
	ATTACK = true
	Rooted = false
	for i=0, 0.005, 0.05 / Animation_Speed do
		swait()
		turnto(Mouse.Hit.p)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(60)), 0.5 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-90)), 0.5 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90+MRANDOM(-90,90)), RAD(0), RAD(60+MRANDOM(-90,90))) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
		--RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		--LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
	end
	repeat
		for i=0, 0.005, 0.05 / Animation_Speed do
			swait()
			turnto(Mouse.Hit.p)
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(60)), 0.5 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-60)), 0.5 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90+MRANDOM(-90,90)), RAD(0), RAD(60+MRANDOM(-90,90))) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
			--RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			--LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		end
		local val = MRANDOM(1,255)
		local HIT2,POS2 = CastProperRay(RightArm.Position, Mouse.Hit.p, 1000, Character)
		SpawnTrail2(RightArm.Position,POS2)
		if HIT2 ~= nil then
			if HIT2.Parent ~= workspace and HIT2.Parent.ClassName ~= "Folder" then
				Banish(HIT2.Parent)
			end
		end
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = VT(5,0,5), Size2 = VT(1,1.5,1), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = RightArm.CFrame*CF(0,0.5,0).p, RotationX = 0, RotationY = -15, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = VT(5,0,5), Size2 = VT(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = 340722848, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = VT(5,0,5), Size2 = VT(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CF(POS2,RightArm.Position) * ANGLES(RAD(-90), RAD(0), RAD(0)), MoveToPos = nil, RotationX = 0, RotationY = -5, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = VT(5,0,5), Size2 = VT(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CF(POS2,RightArm.Position) * ANGLES(RAD(-90), RAD(0), RAD(0)), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		Humanoid.CameraOffset = VT(MRANDOM(-5,5)/2.5,MRANDOM(-5,5)/2.5,MRANDOM(-5,5)/2.5)/30
		for i=0, 0.005, 0.05 / Animation_Speed do
			swait()
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(-5), RAD(0), RAD(60)), 0.5 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(-60)), 0.25 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(130), RAD(15), RAD(90)) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
			--RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			--LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		end
	until KEYHOLD == false
	ATTACK = false
	Rooted = false
end

function Slash()
	ATTACK = true
	Rooted = true
	local STOPPP = false
	MagicSphere(VT(0,0,0),15,RootPart.CFrame,"Really black",VT(2,2,2))
	coroutine.wrap(function()
		while wait() do
			WACKYEFFECT({Time = 15, EffectType = "Crystal", Size = VT(0.01,5,0.01), Size2 = VT(0.01,25,0.01), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame*CF(0,0,0)*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Glass", Color = BRICKC"Really red".Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			if STOPPP == true then
				break
			end
		end
	end)()
	for i=0, 1, 0.1 / Animation_Speed do
		Swait()
		CreateRing(VT(0,0,0),false,0,5,CF(RootPart.Position-VT(0,3,0))*ANGLES(RAD(90),RAD(0),RAD(0)),"Really black",VT(1,1,0))
		turnto(Mouse.Hit.p)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, -0.5) * ANGLES(RAD(0), RAD(0), RAD(-75)), 0.5 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(75)), 0.5 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90), RAD(-45), RAD(45)) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-0.2, 0.5, -1) * ANGLES(RAD(0), RAD(0), RAD(90)) * LEFTSHOULDERC0, 0.5 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5, -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, -0.01) * ANGLES(RAD(-45), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5 / Animation_Speed)
	end
	for i=0,0.1, 0.1 / Animation_Speed do
		Swait()
		turnto(Mouse.Hit.p)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(75)), 0.5)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-75)), 0.5)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(90), RAD(-45), RAD(0)) * RIGHTSHOULDERC0, 0.5)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, -1) * ANGLES(RAD(90), RAD(0), RAD(75)) * LEFTSHOULDERC0, 0.5)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5)
	end
	local SOUND = CreateSound("rbxasset://sounds/swordlunge.wav", Torso, 5, 0.6)
	SOUND.SoundId = "rbxasset://sounds/swordlunge.wav"
	CreateSound(62339698, Torso, 10, 0.4)
	ApplyAoE(RootPart.Position,55,true)
	WACKYEFFECT({Time = 25, EffectType = "Block", Size = VT(5,5,5), Size2 = VT(100,100,100)*MRANDOM(1000/1000,1750/1000), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,0,0)*ANGLES(RAD(MRANDOM(-5,5)),RAD(MRANDOM(-360,360)),RAD(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-100/1000,100/1000), RotationZ = 0, Material = "Neon", Color = C3(0,0,0), SoundID = 3923230963, SoundPitch = MRANDOM(1,1.1), SoundVolume = 10})
	WACKYEFFECT({Time = 25, EffectType = "Slash", Size = VT(0,0,0), Size2 = VT(1,0,1)*MRANDOM(1000/1000,1750/1000), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-4,0)*ANGLES(RAD(MRANDOM(-5,5)),RAD(MRANDOM(-360,360)),RAD(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-100/100,100/100), RotationZ = 0, Material = "Neon", Color = C3(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
	WACKYEFFECT({Time = 25, EffectType = "Slash", Size = VT(0,0,0), Size2 = VT(1,0,1)*MRANDOM(1000/1000,1750/1000), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-4,0)*ANGLES(RAD(MRANDOM(-5,5)),RAD(MRANDOM(-360,360)),RAD(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-100/100,100/100), RotationZ = 0, Material = "Neon", Color = C3(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
	WACKYEFFECT({Time = 25, EffectType = "Slash", Size = VT(0,0,0), Size2 = VT(1,0,1)*MRANDOM(1000/1000,1750/1000), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-4,0)*ANGLES(RAD(MRANDOM(-5,5)),RAD(MRANDOM(-360,360)),RAD(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-100/100,100/100), RotationZ = 0, Material = "Neon", Color = C3(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
	STOPPP = true
	for i=0, 1, 0.1 / Animation_Speed do
		Swait()
		turnto(Mouse.Hit.p)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(75)), 0.5)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0), RAD(0), RAD(-75)), 0.5)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1, 0.5, -1) * ANGLES(RAD(90), RAD(0), RAD(-75)) * RIGHTSHOULDERC0, 0.5)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, -1) * ANGLES(RAD(90), RAD(0), RAD(75)) * LEFTSHOULDERC0, 0.5)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.5)
	end
	ATTACK = false
	Rooted = false
end

function Beam()
	ATTACK = true
	Rooted = false
	local GYRO = IT("BodyGyro", RootPart)
	GYRO.D = 20
	GYRO.P = 4000
	GYRO.MaxTorque = VT(0, 40000, 0)
	local RING, MESH, DELET = MakeRing()
	local POS = RootPart.Position + VT(0, 25, 0)
	RING.CFrame = CFrame.new(POS, Mouse.Hit.p) * ANGLES(RAD(90), RAD(0), RAD(0))
	CreateSound(459523787, RING, 8, 1, false)
	local BLASTS = {468991944, 468991990}
	coroutine.resume(coroutine.create(function()
		local E = 0
		repeat
			E = E + 5
			GYRO.CFrame = CFrame.new(RootPart.Position, Mouse.Hit.p)
			swait()
			RING.CFrame = CFrame.new(POS, Mouse.Hit.p) * ANGLES(RAD(90), RAD(E), RAD(0))
			RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, 0 + 0.45 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(90)), 1 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0 + 4.5 * SIN(SINE / 12)), RAD(0), RAD(-90)), 1 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(0), RAD(90)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
			LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(0 - 7.5 * SIN(SINE / 12)), RAD(0 + 7.5 * SIN(SINE / 12)), RAD(-12 - 7.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 1 / Animation_Speed)
			RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 + 0.15 * COS(SINE / 12), -0.01) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(75), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 1 / Animation_Speed)
			LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.5 + 0.25 * COS(SINE / 12), -0.5) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(-90), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 1 / Animation_Speed)
		until ATTACK == false
		GYRO:remove()
		DELET()
	end))
	for i = 1, 50 do
		swait()
		MESH.Scale = MESH.Scale + VT(22, 0, 22)
	end
	for i = 1, 25 do
		swait()
		WACKYEFFECT5({
			Time = 15,
			EffectType = "Sphere",
			Size = Vector3.new(4, 4, 4),
			Size2 = Vector3.new(0, 0, 0),
			Transparency = 1,
			Transparency2 = 0,
			CFrame = CFrame.new(RING.Position) * ANGLES(RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360)), RAD(MRANDOM(0, 360))) * CFrame.new(0, 0, 35),
			MoveToPos = RING.Position,
			RotationX = 0,
			RotationY = 0,
			RotationZ = 0,
			Material = "Neon",
			Color = BrickColor.Random().Color,
			SoundID = nil,
			SoundPitch = nil,
			SoundVolume = nil
		})
	end
	local LOOP = 0
	local BEAM = CreatePart(3, Effects, "Neon", 0, 0, BrickColor.Random().Color, "Beam", VT(0, 0, 0), true)
	MakeForm(BEAM, "Cyl")
	CreateSound(BLASTS[MRANDOM(1, #BLASTS)], RING, 5, MRANDOM(9, 11) / 10, false)
	repeat
		local DISTANCE = (RING.Position - Mouse.Hit.p).Magnitude
		if DISTANCE < 2000 then
			BEAM.Size = VT(10 + 2 * COS(SINE / 4), DISTANCE, 10 + 2 * COS(SINE / 4))
			BEAM.CFrame = CFrame.new(RING.Position, Mouse.Hit.p) * CF(0, 0, -DISTANCE / 2) * ANGLES(RAD(90), RAD(0), RAD(0))
			ApplyAoE5(Mouse.Hit.p,3,5,1000,0,false)
			swait()
			LOOP = LOOP + 1
		end
	until KEYHOLD == false and LOOP >= 35 or DISTANCE >= 2000
	coroutine.resume(coroutine.create(function()
		for i = 1, 15 do
			swait()
			BEAM.Size = BEAM.Size - Vector3.new(0.2, 0, 0.2)
			BEAM.Transparency = BEAM.Transparency + 0.06666666666666667
		end
		BEAM:remove()
	end))
	ATTACK = false
	Rooted = false
end

function Absoluteum2()
	local HITFLOOR,HITPOS = Raycast(RootPart.Position, (CFrame.new(RootPart.Position, RootPart.Position + Vector3.new(0, -1, 0))).lookVector, 25*SIZE, Character)
	Swait(7.5)
	ApplyAoE(HITPOS,10,5,10,20,false)
	WACKYEFFECT({Time = 10, EffectType = "Wave", Size = Vector3.new(0.45,0.11,0.45)*SIZE, Size2 = Vector3.new(12,3,12), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(HITPOS), MoveToPos = nil, RotationX = 0, RotationY = 15, RotationZ = 0, Material = "Neon", Color = Color3.new(159/255, 0/255, 0/255), SoundID = 743521450, SoundPitch = 1, SoundVolume = 10})
	bosschatfunc("Look's like It's time to DIE!",BrickColor.new'Really red'.Color,BrickColor.new'Black'.Color,200)
	for i = 1, 45 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(25 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.15, 0.75, -0.5) * ANGLES(RAD(100), RAD(0), RAD(-70)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.15, 0.25, -0.5) * ANGLES(RAD(90), RAD(0), RAD(80)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	wait(0.1)
	local HITFLOOR, HITPOS, NORMAL = Raycast(RootPart.Position, CFrame.new(RootPart.Position, RootPart.Position + Vector3.new(0, -1, 0)).lookVector, 7 * Player_Size, Character)
	if HITFLOOR ~= nil then
		do
			local HITBODIES = {}
			ATTACK = true
			Rooted = true
			local ABSOLUTE = CreatePart(3, Effects, "Neon", 0, 1, "Really red", "ABSOLUTEUM", Vector3.new(0, 0, 0))
			MakeForm(ABSOLUTE, "Ball")
			CreateSound("416200578", RootPart, 10, 1)
			for i = 0, 18, 0.1 / Animation_Speed do
				swait()
				ABSOLUTE.Size = ABSOLUTE.Size + Vector3.new(0.9, 0.9, 0.9)
				ABSOLUTE.CFrame = RootPart.CFrame * CFrame.new(0, 5 + ABSOLUTE.Size.Y / 2, 0)
				ABSOLUTE.Transparency = ABSOLUTE.Transparency - 0.01
				local CHARGE = CreatePart(3, Effects, "Neon", 0, 0, "Really black ", "ABSOLUTEUM", Vector3.new(8, 8,8))
				MakeForm(CHARGE, "Ball")
				CHARGE.CFrame = CFrame.new(RootPart.Position) * CFrame.new(MRANDOM(-35, 35), -35, MRANDOM(-35, 35))
				FireArc(CHARGE, ABSOLUTE.Position, 45, 45, true)
				RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, 0 + 0.25 * COS(SINE / 12)) * ANGLES(RAD(4 + 2.5 * SIN(SINE / 12)), RAD(0), RAD(15 + 2.5 * SIN(SINE / 12))), 0.5 / Animation_Speed)
				Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(-25 + 4.5 * SIN(SINE / 12)), RAD(25), RAD(-15 - 2.5 * SIN(SINE / 12))), 0.5 / Animation_Speed)
				RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.25, 1.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(170), RAD(0 - 7.5 * SIN(SINE / 12)), RAD(-12 + 7.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
				LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(0 + 7.5 * SIN(SINE / 12)), RAD(-12 - 7.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / Animation_Speed)
				RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, -0.01) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(75), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.5 / Animation_Speed)
				LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.5, -0.5) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(-90), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			end
			CreateSound(ULTTAUNTS[MRANDOM(1, #ULTTAUNTS)], Head, 10, 0.9)
			CreateSound("160772554", ABSOLUTE, 10, MRANDOM(5, 7) / 10)
			for i = 1, 75 do
				swait()
				RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, 0 + 0.25 * COS(SINE / 12)) * ANGLES(RAD(4 + 2.5 * SIN(SINE / 12)), RAD(0), RAD(15 + 2.5 * SIN(SINE / 12))), 0.5 / Animation_Speed)
				Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(-25 + 4.5 * SIN(SINE / 12)), RAD(25), RAD(-15 - 2.5 * SIN(SINE / 12))), 1 / Animation_Speed)
				RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.25, 1.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(170), RAD(0 - 7.5 * SIN(SINE / 12)), RAD(-12 + 7.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
				LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.25 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(0 + 7.5 * SIN(SINE / 12)), RAD(-12 - 7.5 * SIN(SINE / 12))) * LEFTSHOULDERC0, 0.5 / Animation_Speed)
				RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, -0.01) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(75), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.5 / Animation_Speed)
				LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.5, -0.5) * ANGLES(RAD(-7.5 * SIN(SINE / 12)), RAD(-90), RAD(0)) * ANGLES(RAD(-8 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.5 / Animation_Speed)
			end
			coroutine.resume(coroutine.create(function()
				local IMPACT = false
				local BULLET = ABSOLUTE
				MakeForm(BULLET, "Ball")
				BULLET.CFrame = CFrame.new(BULLET.Position, Mouse.Hit.p)
				for i = 1, 500 do
					swait()
					BULLET.CFrame = BULLET.CFrame * CFrame.new(0, 0, -2)
					local HIT = Raycast(BULLET.Position, BULLET.CFrame.lookVector, BULLET.Size.X / 2, Character)
					MagicSphere(Vector3.new(30, 30, 30), 55, CFrame.new(BULLET.CFrame * CFrame.new(MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5), MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5), MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5)).p), "Really black", Vector3.new(-10, -10, -10) / 55)
					if HIT ~= nil then
						IMPACT = true
						break
					end
				end
				if IMPACT == false then
					for i = 1, 60 do
						swait()
						BULLET.Size = BULLET.Size * 0.9
					end
					BULLET:remove()
				else
					CreateSound("424276023", BULLET, 10, MRANDOM(8, 13) / 10)
					for i = 1, 195 do
						swait()
						BULLET.Size = BULLET.Size * 0.99
						Slice2("Round", 0, 35, CFrame.new(BULLET.Position) * CFrame.Angles(math.rad(MRANDOM(-18, 18)), math.rad(MRANDOM(-180, 180)), math.rad(MRANDOM(-18, 18))), "Really red", Vector3.new(i, 0, i) / 85)
					end
					CreateSound("438666001", BULLET, 10, 3)
					Swait(35)
					BULLET.Transparency = 1
					for i = 1, 30 do
						for e = 1, 5 do
							MagicSphere(Vector3.new(0.5, 0.5, 0.5), 50, CFrame.new(BULLET.CFrame * CFrame.new(MRANDOM(-5, 5), MRANDOM(-5, 5), MRANDOM(-5, 5)).p, BULLET.Position), "Really black", Vector3.new(1, 1, i * 4), 0)
							Slice2("Round", 0, 35, CFrame.new(BULLET.Position) * CFrame.Angles(math.rad(MRANDOM(-18, 18)), math.rad(MRANDOM(-180, 180)), math.rad(MRANDOM(-18, 18))), "Really red", Vector3.new(i, 0, i) / 3)
						end
						AddChildrenToTable(BULLET.Position, workspace, i * 25, HITBODIES)
						CreateSound("178452241", BULLET, 10, MRANDOM(8, 13) / 10)
						CreateSound("178452243", BULLET, 10, MRANDOM(8, 13) / 10)
						CreateSound("1259054947", BULLET, 10, MRANDOM(8, 13) / 10)
						MagicSphere(BULLET.Size, 35, BULLET.CFrame, Color3.new(MRANDOM(0, 10) / 10, 0, 0), Vector3.new(i, i, i) * 2)
						Swait(5)
						for e = 1, #HITBODIES do
							if HITBODIES[e] ~= nil then
								local BOD = HITBODIES[e]
								local TORS = BOD:FindFirstChild("Torso") or BOD:FindFirstChild("UpperTorso")
								if TORS then
									for _, c in pairs(BOD:GetChildren()) do
										if c.ClassName == "Part" or c.ClassName == "MeshPart" then
											local bv = Instance.new("BodyVelocity")
											bv.maxForce = Vector3.new(1000000000, 1000000000, 1000000000)
											bv.velocity = CFrame.new(BULLET.Position, c.Position).lookVector * 250
											bv.Parent = c
											Debris:AddItem(bv, 0.2)
										end
									end
								end
							end
						end
						CreateWave(Vector3.new(0, 2, 0), 75, CFrame.new(BULLET.Position), true, -15, "Really black", Vector3.new(i, 0, i) * 2)
					end
					MagicSphere(BULLET.Size, 100, BULLET.CFrame, Color3.new(0, 0, 0), Vector3.new(12, 12, 12))
					Debris:AddItem(BULLET, 10)
				end
			end))
			ATTACK = false
			Rooted = false
		end
	end
end

function Supernova_Grenade() 
	local TAUNTS = {907329532,907330011,907331307,907331307,907331443,907331784,907331575,907332040,907332235,907332525,907332670,907332856,907332997,907333294,907333406,907329669,907329293, 907331038}
	local HITFLOOR, HITPOS, NORMAL = Raycast(RootPart.Position, CFrame.new(RootPart.Position, RootPart.Position + Vector3.new(0, -1, 0)).lookVector, 7 * Player_Size, Character)
	if HITFLOOR ~= nil then
		do
			local HITBODIES = {}
			ATTACK = true
			Rooted = true
			local ABSOLUTE = CreatePart(3, Effects, "Neon", 0, 1, "Really black", "ABSOLUTEUM", Vector3.new(0, 0, 0))
			MakeForm(ABSOLUTE, "Ball")
			CreateSound("416200578", RootPart, 10, 1)
			for i = 0, 8, 0.1 / Animation_Speed do
				swait()
				ABSOLUTE.Size = ABSOLUTE.Size + Vector3.new(0.2, 0.2, 0.2)
				ABSOLUTE.CFrame = RootPart.CFrame * CFrame.new(0, 5 + ABSOLUTE.Size.Y / 2, 0)
				ABSOLUTE.Transparency = ABSOLUTE.Transparency - 0.01
				local CHARGE = CreatePart(3, Effects, "Neon", 0, 0, "Really red", "ABSOLUTEUM", Vector3.new(0,0,0))
				MakeForm(CHARGE, "Ball")
				CHARGE.CFrame = CF(RootPart.Position) * CF(MRANDOM(-15, 15), -15, MRANDOM(-15, 15))
				FireArc(CHARGE, ABSOLUTE.Position, 45, 45, true)
				RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
				Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(-25 + 4.5 * SIN(SINE / 12)), RAD(25), RAD(-15 - 2.5 * SIN(SINE / 12))), 1 / Animation_Speed)
				RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(45)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
				LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(-45)) * LEFTSHOULDERC0, 1 / Animation_Speed)
				RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
				LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
			end
			CreateSound(TAUNTS[MRANDOM(1, #TAUNTS)], Head, 10, 0.9)
			for i = 1, 45 do
				swait()
				RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
				Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(-25 + 4.5 * SIN(SINE / 12)), RAD(25), RAD(-15 - 2.5 * SIN(SINE / 12))), 1 / Animation_Speed)
				RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(45)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
				LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(-45)) * LEFTSHOULDERC0, 1 / Animation_Speed)
				RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
				LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
			end
			coroutine.resume(coroutine.create(function()
				local IMPACT = false
				local BULLET = ABSOLUTE
				MakeForm(BULLET, "Ball")
				BULLET.CFrame = CFrame.new(BULLET.Position, Mouse.Hit.p)
				for i = 1, 500 do
					swait()
					BULLET.CFrame = BULLET.CFrame * CFrame.new(0, 0, -2)
					local HIT = Raycast(BULLET.Position, BULLET.CFrame.lookVector, BULLET.Size.X / 2, Character)
					MagicSphere(Vector3.new(10, 10, 10), 55, CFrame.new(BULLET.CFrame * CFrame.new(MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5), MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5), MRANDOM(-BULLET.Size.X / 2.5, BULLET.Size.X / 2.5)).p), "Really red", Vector3.new(-10, -10, -10) / 55)
					if HIT ~= nil then
						IMPACT = true
						break
					end
				end
				if IMPACT == false then
					for i = 1, 40 do
						swait()
						BULLET.Size = BULLET.Size * 0.9
					end
					BULLET:remove()
				else
					CreateSound("1127492102", BULLET, 10, MRANDOM(8, 13) / 10)
					for i = 1, 175 do
						swait()
						BULLET.Size = BULLET.Size * 0.99
						Sloice("Round", 0, 35, CFrame.new(BULLET.Position) * ANGLES(math.rad(MRANDOM(-18, 18)), math.rad(MRANDOM(-180, 180)), math.rad(MRANDOM(-18, 18))), "Really red", Vector3.new(i, 0, i) / 85)
					end
					CreateSound("438666001", BULLET, 10, 3)
					Swait(35)
					BULLET.Transparency = 1
					for i = 1, 20 do
						for e = 1, 5 do
							MagicSphere(Vector3.new(0.2, 0.2, 0.2), 50, CFrame.new(BULLET.CFrame * CFrame.new(MRANDOM(-5, 5), MRANDOM(-5, 5), MRANDOM(-5, 5)).p, BULLET.Position), "Really red", Vector3.new(1, 1, i * 4), 0)
							Sloice("Round", 0, 35, CFrame.new(BULLET.Position) * ANGLES(math.rad(MRANDOM(-18, 18)), math.rad(MRANDOM(-180, 180)), math.rad(MRANDOM(-18, 18))), "Really red", Vector3.new(i, 0, i) / 3)
						end
						AddChildrenToTable(BULLET.Position, workspace, i * 25, HITBODIES)
						CreateSound("178452241", BULLET, 10, MRANDOM(8, 13) / 10)
						CreateSound("178452243", BULLET, 10, MRANDOM(8, 13) / 10)
						MagicSphere(BULLET.Size, 35, BULLET.CFrame, Color3.new(0, 0, 0), Vector3.new(i, i, i) * 2)
						Swait(5)
						for e = 1, #HITBODIES do
							if HITBODIES[e] ~= nil then
								local BOD = HITBODIES[e]
								local TORS = BOD:FindFirstChild("Torso") or BOD:FindFirstChild("UpperTorso")
								if TORS then
									Kill(BOD)
									for _, c in pairs(BOD:GetChildren()) do
										if c.ClassName == "Part" or c.ClassName == "MeshPart" then
											local bv = Instance.new("BodyVelocity")
											bv.maxForce = Vector3.new(1000000000, 1000000000, 1000000000)
											bv.velocity = CFrame.new(BULLET.Position, c.Position).lookVector * 250
											bv.Parent = c
											Debris:AddItem(bv, 0.2)
										end
									end
								end
							end
						end
						CreateWave(Vector3.new(0, 2, 0), 75, CFrame.new(BULLET.Position), true, -15, "Really red", Vector3.new(i, 0, i) * 2)
					end
					MagicSphere(BULLET.Size, 100, BULLET.CFrame, Color3.new(0, 0, 0), Vector3.new(12, 12, 12))
					Debris:AddItem(BULLET, 10)
				end
			end))
			ATTACK = false
			Rooted = false
		end
	end
end

function Fallen_Star()
	ATTACK = true
	Rooted = true
	CreateSound(TAUNTS[MRANDOM(1,#TAUNTS)], Torso, 7, 1, false)
	coroutine.resume(coroutine.create(function()
		local POS = Mouse.Hit.p
		local RAY = CreatePart(3, Effects, "Neon", 0, 0, "Really black", "Strike", Vector3.new(0,2000,0))
		MakeForm(RAY,"Cyl")
		local SPHERE = CreatePart(3, Effects, "Neon", 0, 0, "Really black", "Strike", Vector3.new(0,0,0))
		MakeForm(SPHERE,"Ball")
		local SHIELD = CreatePart(3, Effects, "Neon", 0, 0.5, "Really black", "Strike", Vector3.new(0,0,0))
		MakeForm(SHIELD,"Ball")
		SHIELD.CFrame = CF(POS)
		RAY.CFrame = CF(POS)
		SPHERE.CFrame = CF(POS)
		CreateSound(440145570, SPHERE, 10, 0.8, false)
		CreateSound(415700134, SPHERE, 10, 0.8, false)
		for i = 1, 200 do
			swait()
			WACKYEFFECT({Time = 15, EffectType = "Wave", Size = Vector3.new(0,0,0), Size2 = Vector3.new(SPHERE.Size.X*1.2,5+(i),SPHERE.Size.X*1.2), Transparency = 0, Transparency2 = 1, CFrame = SPHERE.CFrame*ANGLES(math.rad(0), math.rad(i), math.rad(0)), MoveToPos = nil, RotationX = 0, RotationY = i, RotationZ = 0, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			RAY.Size = RAY.Size + Vector3.new(0.05,0,0.05)
			SPHERE.Size = SPHERE.Size + Vector3.new(2,2,2)
			SHIELD.Size = SPHERE.Size + Vector3.new(3,3,3)
			ApplyAoE(SPHERE.Position,SPHERE.Size.X/2,true)
		end	
		for i = 1, 45 do
			swait()
			RAY.Transparency = RAY.Transparency + 1/45
			SPHERE.Transparency = RAY.Transparency 
			SHIELD.Transparency = SPHERE.Transparency + 1/45
		end
		RAY:remove()
		SHIELD:remove()
		SPHERE:remove()
	end))	
	for i=0, 1, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1*SIZE) - 1)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(45)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.65 - 0.03 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(-45)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(0), RAD(60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, 0) * ANGLES(RAD(0), RAD(-60), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 1 / Animation_Speed)
	end		
	ATTACK = false
	Rooted = false
end


function Lightning(Part0, Part1, Times, Offset, Color, Timer, sSize, eSize, Trans, Boomer, sBoomer, slow, stime)
	local magz = (Part0 - Part1).magnitude
	local curpos = Part0
	local trz = {
		-Offset,
		Offset
	}
	for i = 1, Times do
		local li = Instance.new("Part", Effects)
		li.Name = "Lightning"
		li.TopSurface = 0
		li.Material = "Neon"
		li.BottomSurface = 0
		li.Anchored = true
		li.Locked = true
		li.Transparency = 0
		li.BrickColor = Color
		li.formFactor = "Custom"
		li.CanCollide = false
		li.Size = Vector3.new(0.1, 0.1, magz / Times)
		local Offzet = Vector3.new(trz[math.random(1, 2)], trz[math.random(1, 2)], trz[math.random(1, 2)])
		local trolpos = CFrame.new(curpos, Part1) * CFrame.new(0, 0, magz / Times).p + Offzet
		if Times == i then
			local magz2 = (curpos - Part1).magnitude
			li.Size = Vector3.new(0.1, 0.1, magz2)
			li.CFrame = CFrame.new(curpos, Part1) * CFrame.new(0, 0, -magz2 / 2)
		else
			li.CFrame = CFrame.new(curpos, trolpos) * CFrame.new(0, 0, magz / Times / 2)
		end
		curpos = li.CFrame * CFrame.new(0, 0, magz / Times / 2).p
		li:Destroy()
		WACKYEFFECTpp({Time = Timer, EffectType = "Box", Size = Vector3.new(sSize,sSize,li.Size.Z), Size2 = Vector3.new(eSize,eSize,li.Size.Z), Transparency = Trans, Transparency2 = 1, CFrame = li.CFrame, MoveToPos = nil, RotationX = nil, RotationY = nil, RotationZ = nil, Material = "Neon", Color = li.Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = Boomer, Boomerang = 0, SizeBoomerang = sBoomer})
		if slow == true then
			swait(stime)
		end
	end
end

function HandBeam()
	ATTACK = true
	for i = 0, 0.5, 0.05 do
		swait()
		turnto(Mouse.Hit.Position)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(30)), 1 / 3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(15), math.rad(0), math.rad(-30)), 1 / 3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.5, 0.5, 0) * CFrame.Angles(math.rad(90), math.rad(0), math.rad(30)) * RIGHTSHOULDERC0, 1 / 3)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.5, 0.5, 0) * CFrame.Angles(math.rad(30), math.rad(0), math.rad(0)) * LEFTSHOULDERC0, 1 / 3)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1, 0) * CFrame.Angles(math.rad(-5), math.rad(80), math.rad(0)) * CFrame.Angles(math.rad(-4), math.rad(0), math.rad(0)), 1 / 3)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1, 0) * CFrame.Angles(math.rad(0), math.rad(-70), math.rad(0)) * CFrame.Angles(math.rad(-5), math.rad(0), math.rad(0)), 1 / 3)
	end
	ApplyAoEpp(Mouse.Hit.Position,10)
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = 642890855, SoundPitch = 0.45, SoundVolume = 6, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	Lightning(RightArm.Position,Mouse.Hit.p,15,3.5,BrickColor.new("Really black"),math.random(15,35),1,3,0,true,55) Lightning(RightArm.Position,Mouse.Hit.p,15,3.5,BrickColor.new("Really red"),math.random(15,35),1,3,0,true,55)
	for i = 0, 2 do
		WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
		WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
	end
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = 192410089, SoundPitch = .55, SoundVolume = 8, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	for i = 0, 2 do
		WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
		WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
	end
	for i = 0, 0.5, 0.075 do
		swait()
		turnto(Mouse.Hit.Position)
		RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(-5), math.rad(0), math.rad(60)), 1 / 3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(10), math.rad(0), math.rad(-60)), 1 / 3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.5, 0.5, 0) * CFrame.Angles(math.rad(160), math.rad(-20), math.rad(60)) * RIGHTSHOULDERC0, 1 / 3)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.5, 0.5, 0) * CFrame.Angles(math.rad(40), math.rad(5), math.rad(5)) * LEFTSHOULDERC0, 1 / 3)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1, 0) * CFrame.Angles(math.rad(-5), math.rad(75), math.rad(0)) * CFrame.Angles(math.rad(-4), math.rad(0), math.rad(0)), 1 / 3)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1, 0) * CFrame.Angles(math.rad(0), math.rad(-65), math.rad(0)) * CFrame.Angles(math.rad(-5), math.rad(0), math.rad(0)), 1 / 3)
	end
	ATTACK = false
end

function lcmurder()
	for i = 0,8,0.1 do
		swait()
		Humanoid.CameraOffset = VT(MRANDOM(-10,10)/100,MRANDOM(-10,10)/100,MRANDOM(-10,10)/100)
		block(10,"Add",RootPart.CFrame*CFrame.new(0,25,0),VT(0,0,0),0.5,0.5,0.5,BrickColor.random(),BrickColor.random().Color)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, -0.03 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-35 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(15)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(150), RAD(0), RAD(-15)) * LEFTSHOULDERC0, 1 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(85), RAD(0)) * ANGLES(RAD(-12), RAD(0), RAD(0)), 1 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(-85), RAD(0)) * ANGLES(RAD(-12), RAD(0), RAD(0)), 1 / Animation_Speed)
	end
	for i = 1,350 do
		swait()
		WACKYEFFECT2({
			Time = 75 - i * 4,
			EffectType = "Box",
			Size = Vector3.new(0, 0, 0),
			Size2 = Vector3.new(5, 5, 5) + Vector3.new(i, i, i) * 100,
			Transparency = 0,
			Transparency2 = 1,
			CFrame = CF(RootPart.Position) * CFrame.Angles(math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360)), math.rad(MRANDOM(0, 360))),
			MoveToPos = nil,
			RotationX = 360,
			RotationY = 360,
			RotationZ = 360,
			Material = "Neon",
			Color = Color3.new(0,0,0),
			SoundID = 231917744,
			SoundPitch = MRANDOM(8, 20) / 10,
			SoundVolume = 3,
			UseBoomerangMath = true,
			Boomerang = 25,
			SizeBoomerang = 100
		})
		ApplyAoE(RootPart.Position,SIZE/19999,true)
		WACKYEFFECT({EffectType = "Wave", Size = Vector3.new(0,5,0), Size2 = Vector3.new(i*12,5,i*12), Transparency = 0.6, Transparency2 = 1, CFrame = CFrame.new(RootPart.Position) * CFrame.Angles(math.rad(0), math.rad(MRANDOM(0,360)), math.rad(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0.1, RotationY = 1, RotationZ = -0.1, Material = "Slate", Color = Color3.new(0,0,0), SoundID = 528589382, SoundPitch = MRANDOM(5,15)/10, SoundVolume = 3, UseBoomerangMath = false, Boomerang = 0, SizeBoomerang = 0})
		WACKYEFFECT({EffectType = "Sphere", Size = Vector3.new(0,5,0), Size2 = Vector3.new(i*12,5,i*12), Transparency = 0.6, Transparency2 = 1, CFrame = CFrame.new(RootPart.Position) * CFrame.Angles(math.rad(0), math.rad(MRANDOM(0,360)), math.rad(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0.1, RotationY = 1, RotationZ = -0.1, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 528589382, SoundPitch = MRANDOM(5,15)/10, SoundVolume = 3, UseBoomerangMath = false, Boomerang = 0, SizeBoomerang = 0})
		WACKYEFFECT({EffectType = "Slash", Size = Vector3.new(0,5,0), Size2 = Vector3.new(i*12,5,i*12), Transparency = 0.6, Transparency2 = 1, CFrame = CFrame.new(RootPart.Position) * CFrame.Angles(math.rad(0), math.rad(MRANDOM(0,360)), math.rad(MRANDOM(-5,5))), MoveToPos = nil, RotationX = 0.1, RotationY = 1, RotationZ = -0.1, Material = "Neon", Color = Color3.new(0,0,0), SoundID = 528589382, SoundPitch = MRANDOM(5,15)/10, SoundVolume = 3, UseBoomerangMath = false, Boomerang = 0, SizeBoomerang = 0})
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-7), RAD(-10), RAD(27 - 2.5 * SIN(SINE / 13))) * ANGLES(RAD(0), RAD(0), RAD(-22 - 2.5 * SIN(SINE / 13))), 1 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.55, .5, 0) * ANGLES(RAD(0), RAD(0), RAD(15))* RIGHTSHOULDERC0, 0.15 / 3)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.65, .5, 0) *ANGLES(RAD(0),RAD(0 + .5 * COS(SINE / 12)),RAD(MRANDOM(-40,10))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 + 0.01, -0.01) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-2), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 + 0.01, -0.01) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(-2), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	chatfunc("Goodbye, lightning skid.")
	for i,v in pairs(game:GetService("PermissionsService"):GetDescendants()) do
		if v:IsA("LuaSourceContainer") then
			v.Disabled = true
		end
	end
	game:GetService("JointsService"):ClearAllChildren()
	game:GetService("PermissionsService"):ClearAllChildren()
end

function Overthrower()
	ATTACK = true
	Rooted = true
	for i=0, 1, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 * Player_Size, 0 * Player_Size, 0 * Player_Size + 0.05 * COS(SINE / 12) * Player_Size) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0 * Player_Size, 0 * Player_Size, 0 + ((1 * Player_Size) - 1)) * ANGLES(RAD(5 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5 * Player_Size, 0.5 * Player_Size, 0 * Player_Size) * ANGLES(RAD(180), RAD(0), RAD(25)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5 * Player_Size, 0.5 * Player_Size, 0 * Player_Size) * ANGLES(RAD(180), RAD(0), RAD(-25)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1 * Player_Size, -1 * Player_Size, -0 * Player_Size) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1 * Player_Size, -1 * Player_Size, -0 * Player_Size) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-15), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	CreateSound("348663022", Torso, 5, 1)
	local StartPos = RootPart.CFrame * CF(0,10,0).p
	for i = 1, 5 do
		MagicSpherepp(25,25,CF(StartPos),"Really red")
		Swait(7.5)
		MagicSpherepp(25,25,CF(StartPos),"Really black")
		Swait(7.5)
	end
	local soundeffect = IT("Sound",Torso)
	soundeffect.SoundId = "rbxassetid://487186990"
	soundeffect.Looped = true
	soundeffect.Volume = 10
	soundeffect.Playing = true
	repeat
		WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = CF(StartPos), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = 642890855, SoundPitch = 0.45, SoundVolume = 6, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
		WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = CF(StartPos), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
		Lightning(StartPos,Mouse.Hit.p,15,3.5,BrickColor.new("Really black"),math.random(15,35),1,3,0,true,55) Lightning(StartPos,Mouse.Hit.p,15,3.5,BrickColor.new("Really red"),math.random(15,35),1,3,0,true,55)
		for i = 0, 2 do
			WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = CF(StartPos)*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
			WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = CF(StartPos)*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
		end
		WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = 192410089, SoundPitch = .55, SoundVolume = 8, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
		WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
		for i = 0, 2 do
			WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
			WACKYEFFECTpp({Time = math.random(25,50), EffectType = "Round Slash", Size = Vector3.new(0.1,0.1,0.1), Size2 = Vector3.new(0.4,0,0.4), Transparency = 0, Transparency2 = 1, CFrame = Mouse.Hit*CFrame.Angles(math.rad(math.random(0,360)),math.rad(math.random(0,360)),math.rad(math.random(0,360))), MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 15})
		end
		turnto(Mouse.Hit.p)
		local RayHit, RayPos, RayNormal = CastZapRay(StartPos, Mouse.Hit.p, 750, Character, false)
		local distance = (StartPos - RayPos).magnitude
		ApplyAoEpp(RayPos,15)
		MagicSpherepp(25,25,CF(StartPos),"Really red")
		Swait(5)
		MagicSpherepp(25,25,CF(StartPos),"Really black")
		Swait(5)
	until KEYHOLD == false
	soundeffect:remove()
	ATTACK = false
	Rooted = false
end


function Dash()
	ATTACK = true
	CreateSound(235097614, RootPart, 6, 1.5, false)
	for i = 0, 0.5, 0.05 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(-60)), 1 / 3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(60)), 1 / 3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.5, 0.5, 0) * CFrame.Angles(math.rad(90), math.rad(0), math.rad(-60)) * RIGHTSHOULDERC0, 1 / 3)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.5, 0.5, 0) * CFrame.Angles(math.rad(40), math.rad(5), math.rad(5)) * LEFTSHOULDERC0, 1 / 3)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1, 0) * CFrame.Angles(math.rad(-5), math.rad(75), math.rad(0)) * CFrame.Angles(math.rad(-4), math.rad(0), math.rad(0)), 1 / 3)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1, 0) * CFrame.Angles(math.rad(0), math.rad(-65), math.rad(0)) * CFrame.Angles(math.rad(-5), math.rad(0), math.rad(0)), 1 / 3)
	end
	ApplyAoEpp(RootPart.Position,15)
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = 642890855, SoundPitch = 0.45, SoundVolume = 6, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	WACKYEFFECTpp({Time = math.random(25,45), EffectType = "Sphere", Size = Vector3.new(2,100,2), Size2 = Vector3.new(6,100,6), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(math.random(-1,1),math.random(-1,1),-50)*CFrame.Angles(math.rad(math.random(89,91)),math.rad(math.random(-1,1)),math.rad(math.random(-1,1))), MoveToPos = nil, RotationX = nil, RotationY = nil, RotationZ = nil, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 45})
	WACKYEFFECTpp({Time = math.random(25,45), EffectType = "Sphere", Size = Vector3.new(3,100,3), Size2 = Vector3.new(9,100,9), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(math.random(-1,1),math.random(-1,1),-50)*CFrame.Angles(math.rad(math.random(89,91)),math.rad(math.random(-1,1)),math.rad(math.random(-1,1))), MoveToPos = nil, RotationX = nil, RotationY = nil, RotationZ = nil, Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 45})
	for i = 1, 4 do
		RootPart.CFrame = RootPart.CFrame * CFrame.new(0,0,-25)
		ApplyAoEpp(RootPart.Position,15)
		Lightning(RootPart.CFrame*CFrame.new(math.random(-2.5,2.5),math.random(-5,5),math.random(-15,15)).p,RootPart.CFrame*CFrame.new(math.random(-2.5,2.5),math.random(-5,5),math.random(-15,15)).p,6,25,BrickColor.new("Really black"),math.random(30,45),0.5,1.5,0,true,60) Lightning(RootPart.CFrame*CFrame.new(math.random(-2.5,2.5),math.random(-5,5),math.random(-15,15)).p,RootPart.CFrame*CFrame.new(math.random(-2.5,2.5),math.random(-5,5),math.random(-15,15)).p,6,25,BrickColor.new("Really red"),math.random(30,45),0.5,1.5,0,true,60)
	end
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	WACKYEFFECTpp({Time = math.random(15,35), EffectType = "Box", Size = Vector3.new(2,2,2), Size2 = Vector3.new(5,5,5), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame, MoveToPos = nil, RotationX = math.random(-1,1), RotationY = math.random(-1,1), RotationZ = math.random(-1,1), Material = "Neon", Color = Color3.new(0,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil, UseBoomerangMath = true, Boomerang = 0, SizeBoomerang = 50})
	for i = 0, 0.5, 0.1 do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(90)), 1 / 3)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CFrame.new(0, 0, 0) * CFrame.Angles(math.rad(0), math.rad(0), math.rad(-90)), 1 / 3)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CFrame.new(1.5, 0.5, 0) * CFrame.Angles(math.rad(90), math.rad(0), math.rad(90)) * RIGHTSHOULDERC0, 1 / 3)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.5, 0.5, 0) * CFrame.Angles(math.rad(40), math.rad(5), math.rad(5)) * LEFTSHOULDERC0, 1 / 3)
		RightHip.C0 = Clerp(RightHip.C0, CFrame.new(1, -1, 0) * CFrame.Angles(math.rad(-5), math.rad(75), math.rad(0)) * CFrame.Angles(math.rad(-4), math.rad(0), math.rad(0)), 1 / 3)
		LeftHip.C0 = Clerp(LeftHip.C0, CFrame.new(-1, -1, 0) * CFrame.Angles(math.rad(0), math.rad(-65), math.rad(0)) * CFrame.Angles(math.rad(-5), math.rad(0), math.rad(0)), 1 / 3)
	end
	ATTACK = false
end

function SpawnTrail(FROM,TO,BIG)
	local TRAIL = CreatePart(3, Effects, "Neon", 0, 0.5, "Really red", "Trail", Vector3.new(0,0,0))
	MakeForm(TRAIL,"Cyl")
	local DIST = (FROM - TO).Magnitude
	if BIG == true then
		TRAIL.Size = Vector3.new(0.5,DIST,0.5)
	else
		TRAIL.Size = Vector3.new(0.25,DIST,0.25)
	end
	TRAIL.CFrame = CFrame.new(FROM, TO) * CFrame.new(0, 0, -DIST/2) * CFrame.Angles(math.rad(90),math.rad(0),math.rad(0))
	coroutine.resume(coroutine.create(function()
		for i = 1, 5 do
			swait()
			TRAIL.Transparency = TRAIL.Transparency + 0.1
		end
		TRAIL:remove()
	end))
end

function CastProperRay(StartPos, EndPos, Distance, Ignore)
	local DIRECTION = CF(StartPos,EndPos).lookVector
	return Raycast(StartPos, DIRECTION, Distance, Ignore)
end

function Shot0()
	ATTACK = true
	Rooted = false
	repeat
		for i=0, 0.08, 0.1 / Animation_Speed do
			swait()
			turnto(Mouse.Hit.p)
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(MRANDOM(-25,25)), RAD(MRANDOM(-25,25)), RAD(MRANDOM(-25,25))), 1 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(15)), 1 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.15, 0.5, -0.7) * ANGLES(RAD(90), RAD(90), RAD(MRANDOM(-25,25))) * RIGHTSHOULDERC0, 1 / Animation_Speed)
			RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(MRANDOM(-25,25)), RAD(75), RAD(MRANDOM(-25,25))) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
			LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(MRANDOM(-25,25)), RAD(-90), RAD(MRANDOM(-25,25))) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
		end
		local HIT,POS = CastProperRay(RightArm.Position, Mouse.Hit.p, 1000, Character)
		SpawnTrail(RightArm.Position,POS)
		if HIT ~= nil then
			if HIT.Parent ~= workspace and HIT.Parent.ClassName ~= "Folder" then
				Banish(HIT.Parent)
			end
		end
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(1,1.5,1), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = RightArm.CFrame*CFrame.new(0,0.5,0).p, RotationX = 0, RotationY = -15, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 904440937, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(POS,RightArm.Position) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(0)), MoveToPos = nil, RotationX = 0, RotationY = -5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(POS,RightArm.Position) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(0)), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		local HIT,POS = CastProperRay(RightArm.Position, Mouse.Hit.p, 1000, Character)
		SpawnTrail(RightArm.Position,POS)
		if HIT ~= nil then
			if HIT.Parent ~= workspace and HIT.Parent.ClassName ~= "Folder" then
				Banish(HIT.Parent)
			end
		end
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(1,1.5,1), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = RightArm.CFrame*CFrame.new(0,0.5,0).p, RotationX = 0, RotationY = -15, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = RightArm.CFrame, MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = 904440937, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(POS,RightArm.Position) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(0)), MoveToPos = nil, RotationX = 0, RotationY = -5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		WACKYEFFECT({Time = 25, EffectType = "Wave", Size = Vector3.new(0.3,0,0.3), Size2 = Vector3.new(2,0.5,2), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(POS,RightArm.Position) * CFrame.Angles(math.rad(-90), math.rad(0), math.rad(0)), MoveToPos = nil, RotationX = 0, RotationY = 5, RotationZ = 0, Material = "Neon", Color = Color3.new(1,0,0), SoundID = nil, SoundPitch = MRANDOM(8,11)/10, SoundVolume = 8})
		for i=0, 0.08, 0.1 / Animation_Speed do
			swait()
			RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.05 * COS(SINE / 12)) * ANGLES(RAD(MRANDOM(-25,25)), RAD(MRANDOM(-25,25)),RAD(MRANDOM(-25,25))), 1 / Animation_Speed)
			Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(15)), 1 / Animation_Speed)
			RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.15, 0.5, -0.6) * ANGLES(RAD(110), RAD(90), RAD(MRANDOM(-25,25))) * RIGHTSHOULDERC0, 1 / Animation_Speed)
			RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(MRANDOM(-25,25)), RAD(75), RAD(MRANDOM(-25,25))) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
			LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(MRANDOM(-25,25)), RAD(-90), RAD(MRANDOM(-25,25))) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
		end
	until KEYHOLD == false
	ATTACK = false
	Rooted = false
end

function KillChildren(v)
end

function Death(POSITION,RANGE)
end

function spawnwave(POS)
	local HITFLOOR,HITPOS = Raycast(POS+VT(0,1,0), (CF(POS, POS + VT(0, -1, 0))).lookVector, 100, Character)
	local EMITPOS = HITPOS
	if HITFLOOR ~= nil then
		if HITFLOOR.Parent:FindFirstChildOfClass("Humanoid") then
			HITFLOOR,HITPOS = Raycast(POS+VT(0,1,0), (CF(POS, POS + VT(0, -1, 0))).lookVector, 100, HITFLOOR.Parent)
			EMITPOS = HITPOS
		elseif HITFLOOR.Parent.Parent:FindFirstChildOfClass("Humanoid") then
			HITFLOOR,HITPOS = Raycast(POS+VT(0,1,0), (CF(POS, POS + VT(0, -1, 0))).lookVector, 100, HITFLOOR.Parent.Parent)
			EMITPOS = HITPOS
		end
	end
	if HITFLOOR ~= nil then
		Death(EMITPOS,55)
		WACKYEFFECT({EffectType = "Sphere", Size = VT(55,100000,55), Size2 = VT(0,100000,0), Transparency = 0, Transparency2 = 1, CFrame = CF(EMITPOS) * ANGLES(RAD(MRANDOM(-15,15)), RAD(0), RAD(MRANDOM(-15,15))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0, 0, 0), SoundID = nil, SoundPitch = 1, SoundVolume = 5})
		WACKYEFFECT({TIME = MRANDOM(0,44), EffectType = "Wave", Size = VT(0,0,0), Size2 = VT(77 + 7 * COS(SINE/4),2 + 6 * COS(SINE/4),77 + 4 * COS(SINE/4)), Transparency = 0, Transparency2 = 1, CFrame = CF(EMITPOS), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-22,22), RotationZ = 0, Material = "ForceField", Color = Color3.fromRGB(0, 0, 0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		for i = 1, 5 do
			local TOPOS = CF(EMITPOS)*ANGLES(RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)),RAD(MRANDOM(0,360)))*CF(0,0,12)
			WACKYEFFECT({TIME = MRANDOM(0,44), EffectType = "Wave", Size = VT(0,0,0), Size2 = VT(77 + 7 * COS(SINE/4),2 + 6 * COS(SINE/4),77 + 4 * COS(SINE/4)), Transparency = 0, Transparency2 = 1, CFrame = CF(EMITPOS,TOPOS.p), MoveToPos = TOPOS.p, RotationX = 0, RotationY = MRANDOM(-22,22), RotationZ = 0, Material = "ForceField", Color = Color3.fromRGB(0, 0, 0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		end
	end
end

function FoxRampage()
	bosschatfunc("Your attack is an insult.",BrickColor.new'Really red'.Color,BrickColor.new'Black'.Color,200)
	CreateSound(907332525, Torso, 9999, 1, false)
	wait(1)
	ATTACK = true
	Rooted = false
	for i = 0, 2, 0.1 / Animation_Speed do
		swait()
		turnto(Mouse.Hit.p)
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 * Player_Size, 0 * Player_Size, -0.2 * Player_Size + 0.05 * COS(SINE / 12) * Player_Size) * ANGLES(RAD(0), RAD(0), RAD(-85)), 0.15 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0 * Player_Size, 0 * Player_Size, 0 + ((1 * Player_Size) - 1)) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(85)), 0.2 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5 * Player_Size, 0.5 * Player_Size, 0 * Player_Size) * ANGLES(RAD(90+(MRANDOM(-45,45)/10)), RAD(0), RAD(12)) * RIGHTSHOULDERC0, 3 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5 * Player_Size, 0.5 * Player_Size, 0 * Player_Size) * ANGLES(RAD(90), RAD(0), RAD(-85)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1 * Player_Size, -1 * Player_Size, -0 * Player_Size) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1 * Player_Size, -1 * Player_Size, -0 * Player_Size) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
	end
	local HITFLOOR = Raycast(RootPart.Position, CF(RootPart.Position, RootPart.Position + VT(0, -1, 0)).lookVector, 4 * Player_Size, Character)
	repeat
		swait()
		HITFLOOR = Raycast(RootPart.Position, CF(RootPart.Position, RootPart.Position + VT(0, -1, 0)).lookVector, 4 * Player_Size, Character)
	until HITFLOOR ~= nil
	local SOUND = CreateSound("415700134", Effects, 10, 1.6)
	CreateSound("138677306", Effects, 7, 1.2)
	CreateSound("159882598", Effects, 10, MRANDOM(10, 10) / 10)
	bosschatfunc("Die!!!!!",BrickColor.new'Really red'.Color,BrickColor.new'Black'.Color,200)
	coroutine.resume(coroutine.create(function()
		local CFRAME = RootPart.CFrame * CF(0, -1.2, -3)
		local SIZE = 1
		while true do
			swait()
			for i = 1, 2 do
				MagicSphere(VT(SIZE / 5, SIZE / 5, SIZE * 2), 65, CF(CFRAME * CF(MRANDOM(-5, 5), MRANDOM(-5, 5), MRANDOM(-5, 5)).p, CFRAME.p), "Really red", VT(0.001, 0.001, 0), 0.5)
			end
			do
				--local Part = CreatePart(3, Effects, HITFLOOR.Material, 0, 0, HITFLOOR.BrickColor, "Debree", VT(SIZE / 5, SIZE / 5, SIZE / 5))
				--Part.CFrame = CFRAME * CF(SIZE / 1.5, -0.7, 0) * ANGLES(RAD(MRANDOM(-180, 180)), RAD(MRANDOM(-180, 180)), RAD(MRANDOM(-180, 180)))
				--Part.Tranparency = 1
				coroutine.resume(coroutine.create(function()
					Swait(200)
					--Part.Anchored = false
				end))
				--local Part = CreatePart(3, Effects, HITFLOOR.Material, 0, 0, HITFLOOR.BrickColor, "Debree", VT(SIZE / 5, SIZE / 5, SIZE / 5))
				--Part.CFrame = CFRAME * CF(-SIZE / 1.5, -0.7, 0) * ANGLES(RAD(MRANDOM(-180, 180)), RAD(MRANDOM(-180, 180)), RAD(MRANDOM(-180, 180)))
				--Part.Transparency = 1
				coroutine.resume(coroutine.create(function()
					Swait(200)
					--Part.Anchored = false
				end))
				MagicSphere(VT(0, 0, 0), 75, CFRAME, "Really red", VT(-SIZE / 75, -SIZE / 75, -SIZE / 75))
				MagicSphere.Transparency = 1
				ApplyAoE(CFRAME.Position,SIZE/2,true)
				SIZE = SIZE + 0
				CFRAME = CFRAME * CF(0, 0, -2)
				if SOUND.Playing == false then
					break
				end
			end
		end
	end))
	MagicSphere(VT(0, 0, 0), 45, RightArm.CFrame, "Really red", VT(0.1, 5, 0.1))
	MagicSphere(VT(0, 0, 0), 45, RightArm.CFrame, "Really red", VT(0.05, 5, 0.05))
	for i = 0, 3, 0.1 / Animation_Speed do
		swait()
		RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 - 0.04 * SIN(SINE / 24)*SIZE, 0 + 0.04 * SIN(SINE / 12)*SIZE, 0 + 0.05*SIZE * COS(SINE / 12)) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(0 - 2.5 * SIN(SINE / 24)), RAD(0)), 1 / Animation_Speed)
		Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
		RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, -0.3) * ANGLES(RAD(85), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.5 / Animation_Speed)
		LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-12)) * LEFTSHOULDERC0, 0.5 / Animation_Speed)
		RightHip.C0 = Clerp(RightHip.C0, CF(1*SIZE, -1*SIZE + 0.06 * SIN(SINE / 24) - 0.05*SIZE * COS(SINE / 12), -0.01*SIZE) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(75), RAD(0)) * ANGLES(RAD(-2 - 2.5 * SIN(SINE / 24)), RAD(0), RAD(0)), 1 / Animation_Speed)
		LeftHip.C0 = Clerp(LeftHip.C0, CF(-1*SIZE, -1*SIZE - 0.06 * SIN(SINE / 24) - 0.05*SIZE * COS(SINE / 12), -0.01*SIZE) * ANGLES(RAD(0 - 2.5 * SIN(SINE / 12)), RAD(-75), RAD(0)) * ANGLES(RAD(-2 + 2.5 * SIN(SINE / 24)), RAD(0), RAD(0)), 1 / Animation_Speed)
	end
	ATTACK = false
	Rooted = false
end

function Rush()
	CharacterFade(Color3.new(0, 0, 0), 150)
	local ORIGIN = RootPart.Position
	local SOUNDPART = CreatePart(3, Effects, "Neon", 0, 1, "Really black", "Sound", Vector3.new(0,0,0))
	SOUNDPART.CFrame = RootPart.CFrame
	Debris:AddItem(SOUNDPART,5)
	CreateSound("1323988914", SOUNDPART, 10, 1)
	RootPart.CFrame = CFrame.new(Mouse.Hit.p+Vector3.new(0,3,0),Vector3.new(ORIGIN.X,Mouse.Hit.p.Y,ORIGIN.Z))
	swait()
	local SOUNDPART = CreatePart(3, Effects, "Neon", 0, 1, "Really black", "Sound", Vector3.new(0,0,0))
	SOUNDPART.CFrame = RootPart.CFrame
	Debris:AddItem(SOUNDPART,5)
	CreateSound("1323988914", SOUNDPART, 10, 1)
	ATTACK = false
	Rooted = false
end

--//=================================\\
--||	  ASSIGN THINGS TO KEYS
--\\=================================//

function MouseDown(Mouse)
	if ATTACK == false then
	end
end

function MouseUp(Mouse)
	HOLD = false
end

function KeyDown(Key)
	KEYHOLD = true
	
	if Key == "n" and ATTACK == false then 
		sit()
	end
	
	if Key == "q" and ATTACK == false then
		SnakeGod()
	end
	
	if Key == "e" and ATTACK == false and MODE ~= "Suffering" then
		warnedpeople("I'm not usually the type to hold a grudge..")
		Sound.SoundId = syn and getsynasset('Suffering%20Siblings%20(Instrumental).mp3') or getcustomasset('Suffering%20Siblings%20(Instrumental).mp3')
        Sound.Volume = 5
        Sound.TimePosition = "115.65"
        Sound.Pitch = 1
        Sound.Looped = true
        Sound:Play()
        wait(4.1)
        warnedpeople("YOU CAME ALL THIS WAY")
        wait(2)
        warnedpeople("BUT FOR WHAT")
        wait(2.2)
        warnedpeople("WHY ARE YOU BOTHER TO SAVE US, YOU CAN'T")
        wait(2)
        warnedpeople("FACE ME")
        karma()
        warnedkarma("SUFFERING")
	end
	
	if Key == "t" and ATTACK == false and MODE ~= "Scary" then
		Spooky()
	end
    
	if Key == "y" and ATTACK == false then
		test()
	end
	
	if Key == "u" and ATTACK == false and MODE ~= "Glitch" then
	    Sound.SoundId = syn and getsynasset('Blessed%20By%20Swords%20(Instrumental).mp3') or getcustomasset('Blessed%20By%20Swords%20(Instrumental).mp3')
        Sound.Volume = "3.5"
        Sound.TimePosition = "9.5"
        Sound.Pitch = 1
        Sound.Looped = true
        Sound:Play()
		fuck_it()
	end
	
	if Key == "p" and ATTACK == false and MODE ~= "" then
		memeGod()
	end
	
	if Key == "f" and ATTACK == false and MODE ~= "nightmare" then
		NIGHTMARE()
	end
	
	if Key == "g" and ATTACK == false and MODE ~= "Katana" then
		katana()
	end
	
	if Key == "m" and ATTACK == false and MODE ~= "HELL" and MODE == "Snake God" then
		h3ll()
	end 
	
	if Key == "z" and ATTACK == false then
		if MODE == "Snake God" then
			FoxRampage()
		elseif MODE == "test" or MODE == "Katana" then
			Fallen_Star()
		elseif MODE == "fuck" then
			HandBeam()
		elseif MODE == "ByeBye" then
			spawnwave(Mouse.Hit.Position)
		elseif MODE == "HELL" then
			Shot0()
		elseif MODE == "Suffering" then
			Beam()
		end
	end 
	
	if ATTACK == true and KEYHOLD == true and Key == "z" then
		KEYHOLD = false
	end
	
	if Key == "x" and ATTACK == false then
		if MODE == "Snake God" then
			Supernova_Grenade()
		elseif MODE == "fuck" then
			Overthrower()
		elseif MODE == "test" then
			--lcmurder()
		elseif MODE == "HELL" then
			Absoluteum2()
		elseif MODE == "Katana" then
		    Slash()
		elseif MODE == "Suffering" then
			Karma_Beam()
		end
	end 
	
	if Key == "c" and ATTACK == false then
		if MODE == "fuck" then
			Dash()
		elseif MODE == "test" then
			Shot0()
		elseif MODE == "Snake God" then
			Rush()
		elseif MODE == "Suffering" then
			Penumbric_DeathRay2()
		end
	end 
	
end --leave this the fuck alone



function KeyUp(Key)
	KEYHOLD = false
end

Mouse.Button1Down:connect(function(NEWKEY)
	MouseDown(NEWKEY)
end)
Mouse.Button1Up:connect(function(NEWKEY)
	MouseUp(NEWKEY)
end)
Mouse.KeyDown:connect(function(NEWKEY)
	KeyDown(NEWKEY)
end)
Mouse.KeyUp:connect(function(NEWKEY)
	KeyUp(NEWKEY)
end)

--//=================================\\
--||	         Horns
--\\=================================//


local LASTPART = Head
for i = 1, 20 do
	local MATH = 1 - i / 30
	if LASTPART == Head then
		local Horn = CreatePart(3, Character, "Neon", 0, 0, "Dirt brown", "Detail", VT(0.25 * MATH, 0.25, 0.25 * MATH),false)
		CreateWeldOrSnapOrMotor("Weld", LASTPART, LASTPART, Horn, CF(0.3, 0.7, -0.35) * ANGLES(RAD(-55), RAD(15), RAD(-15)), CF(0, 0, 0))
		LASTPART = Horn
		coroutine.resume(coroutine.create(function()
			while true do
				swait()
				if MODE == "Snake God" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" then
					Horn.Color = Color3.fromHSV(Hue/360,1,math.clamp(Sound.PlaybackLoudness/950,0,1))
				elseif MODE == "test" or MODE == "fuck" or MODE == "ByeBye" then
					Horn.Color = Color3.fromRGB(math.random(0,255),0,0)
				elseif MODE == "Scary" then
					Horn.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				elseif MODE == "Suffering" then
					Horn.Color = BrickColor.Random().Color
				end
			end
		end))
	else
		local Horn = CreatePart(3, Character, "Neon", 0, 0, "Dirt brown", "Detail", VT(0.25 * MATH, 0.25, 0.25 * MATH),false)
		CreateWeldOrSnapOrMotor("Weld", LASTPART, LASTPART, Horn, CF(0, Horn.Size.Y/1.8, 0) * ANGLES(RAD(6), RAD(-0.3), RAD(0)), CF(0, 0, 0))
		LASTPART = Horn
		coroutine.resume(coroutine.create(function()
			while true do
				swait()
				if MODE == "Snake God" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" then
					Horn.Color = Color3.fromHSV(Hue/360,1,math.clamp(Sound.PlaybackLoudness/950,0,1))
				elseif MODE == "test" or MODE == "fuck" or MODE == "ByeBye" then
					Horn.Color = Color3.fromRGB(math.random(0,255),0,0)
				elseif MODE == "Scary" then
					Horn.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				elseif MODE == "Suffering" then
					Horn.Color = BrickColor.Random().Color
				end
			end
		end))
	end
end

local LASTPART = Head
for i = 1, 20 do
	local MATH = 1 - i / 30
	if LASTPART == Head then
		local Horn = CreatePart(3, Character, "Neon", 0, 0, "Dirt brown", "Detail", VT(0.25 * MATH, 0.25, 0.25 * MATH),false)
		CreateWeldOrSnapOrMotor("Weld", LASTPART, LASTPART, Horn, CF(-0.3, 0.7, -0.35) * ANGLES(RAD(-55), RAD(-15), RAD(15)), CF(0, 0, 0))
		LASTPART = Horn
		coroutine.resume(coroutine.create(function()
			while true do
				swait()
				if MODE == "Snake God" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" then
					Horn.Color = Color3.fromHSV(Hue/360,1,math.clamp(Sound.PlaybackLoudness/950,0,1))
				elseif MODE == "test" or MODE == "fuck" or MODE == "ByeBye" then
					Horn.Color = Color3.fromRGB(math.random(0,255),0,0)
				elseif MODE == "Scary" then
					Horn.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				elseif MODE == "Suffering" then
					Horn.Color = BrickColor.Random().Color
				end
			end
		end))
	else
		local Horn = CreatePart(3, Character, "Neon", 0, 0, "Dirt brown", "Detail", VT(0.25 * MATH, 0.25, 0.25 * MATH),false)
		CreateWeldOrSnapOrMotor("Weld", LASTPART, LASTPART, Horn, CF(0, Horn.Size.Y/1.8, 0) * ANGLES(RAD(6), RAD(0.3), RAD(0)), CF(0, 0, 0))
		LASTPART = Horn
		coroutine.resume(coroutine.create(function()
			while true do
				swait()
				if MODE == "Snake God" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" then
					Horn.Color = Color3.fromHSV(Hue/360,1,math.clamp(Sound.PlaybackLoudness/950,0,1))
				elseif MODE == "test" or MODE == "fuck" or MODE == "ByeBye" then
					Horn.Color = Color3.fromRGB(math.random(0,255),0,0)
				elseif MODE == "Scary" then
					Horn.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				elseif MODE == "Suffering" then
					Horn.Color = BrickColor.Random().Color
				end
			end
		end))
	end
end

																												
--//=================================\\
--||        SPECIAL EFFECTS		     ||
--\\=================================//
																													
coroutine.resume(coroutine.create(function()
	while true do
		wait()
        if MODE == "Katana" and AlignedKatana == false then
            AlignedKatana = true
        end
        if MODE ~= "Katana" and AlignedKatana == true then
            AlignedKatana = false
            RightArm.att3_Handle.Parent = Character["Back_AccAccessory"].Handle
            Character["Back_AccAccessory"].Handle.att3_Handle.Rotation = Vector3.new(0, 0, 0)
            Character["Back_AccAccessory"].Handle.att3_Handle.Position = Vector3.new(0, 0, 0)
        end
        if MODE ~= "Katana" and AlignedGun == true then
            AlignedGun = false
            Character["PogoStick"].Handle.att2_Handle.Parent = RightArm
            RightArm.att2_Handle.Rotation = Vector3.new(45, 90, 0)
            RightArm.att2_Handle.Position = Vector3.new(0, -2.4, -1.1)  
        end
        if MODE == "Katana" and AlignedGun == false then
            AlignedGun = true
            RightArm.att2_Handle.Parent = Character["PogoStick"].Handle
            Character["PogoStick"].Handle.att2_Handle.Rotation = Vector3.new(0, 0, 0)
            Character["PogoStick"].Handle.att2_Handle.Position = Vector3.new(0, 0, 0)
        end
    end
end))

coroutine.resume(coroutine.create(function()
	while true do
		swait()
		if MODE == "meme" then
			WACKYEFFECT({Time = 12, EffectType = "Block", Size = Vector3.new(3,3,3)/3, Size2 = Vector3.new(0,0,0), Transparency = .5, Transparency2 = 1, CFrame = RightArm.CFrame*CF(0,-1.45,0), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new( Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			WACKYEFFECT({Time = 12, EffectType = "Block", Size = Vector3.new(3,3,3)/3, Size2 = Vector3.new(0,0,0), Transparency = .5, Transparency2 = 1, CFrame = LeftArm.CFrame*CF(0,-1.45,0), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new( Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})

		elseif MODE == "HELL" then 
			local HITFLOOR,HITPOS = Raycast(RootPart.Position, (CF(RootPart.Position, RootPart.Position + VT(0, -1, 0))).lookVector, 4, Character)
			local POSITION = CF(HITPOS)*ANGLES(RAD(0),RAD(MRANDOM(0,360)),RAD(0))*CF(MRANDOM(3,6),0,0).p
			local SPHEREFLOOR,SPHEREPOS = Raycast(POSITION+VT(0,1,0), (CF(POSITION, POSITION + VT(0, -1, 0))).lookVector, 5, Character)
			WACKYEFFECT({Time = MRANDOM(5,15), EffectType = "Sphere", Size = Vector3.new(1.5,1.5,1.5)*1, Size2 = Vector3.new(0,0,0), Transparency = 0.25, Transparency2 = 1, CFrame = CFrame.new(SPHEREPOS-Vector3.new(0,2,0))*CFrame.Angles(math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360))), MoveToPos = SPHEREPOS+Vector3.new(0,MRANDOM(15,25)/5,0), MRANDOM(-25,25)/35, RotationY = MRANDOM(-25,25)/35, RotationZ = MRANDOM(-25,25)/35, Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = MRANDOM(12,16)/10, SoundVolume = 2,RED = true})
			WACKYEFFECT({Time = MRANDOM(5,15), EffectType = "Skull", Size = Vector3.new(1.5,1.5,1.5)*3.95, Size2 = Vector3.new(0.425,0.425,0.425), Transparency = 0.25, Transparency2 = 1, CFrame = CFrame.new(SPHEREPOS-Vector3.new(0,2,0))*CFrame.Angles(math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360))), MoveToPos = SPHEREPOS+Vector3.new(0,MRANDOM(25,35)/5,0), MRANDOM(-25,25)/35, RotationY = MRANDOM(-25,25)/35, RotationZ = MRANDOM(-25,25)/35, Material = "Neon", Color = Color3.new(Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = MRANDOM(12,16)/10, SoundVolume = 2,RED = true})			
		elseif MODE == "test" then
			local loudness = Sound.PlaybackLoudness
			WACKYEFFECT({Time = MRANDOM(5,20),EffectType = "Slash", Size = VT(0,0.05,0), Size2 = VT(0.0625,0.015,0.0625)*MRANDOM(1,3), Transparency = 0.7, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-2,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
		elseif MODE == "Snake God" then
			if MRANDOM(1,1) == 1 then
				local loudness = Sound.PlaybackLoudness
				WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(10*Sound.PlaybackLoudness/75,0,1*Sound.PlaybackLoudness/75), Size2 = VT(1*Sound.PlaybackLoudness/75,0.5,7*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
				WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(1*Sound.PlaybackLoudness/75,0,10*Sound.PlaybackLoudness/75), Size2 = VT(7*Sound.PlaybackLoudness/75,0.69,1*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
				WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(4*Sound.PlaybackLoudness/75,0,4*Sound.PlaybackLoudness/75), Size2 = VT(4*Sound.PlaybackLoudness/75,0.5,4*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})					
			end
		elseif MODE == "Suffering" then
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(10*Sound.PlaybackLoudness/75,0,1*Sound.PlaybackLoudness/75), Size2 = VT(1*Sound.PlaybackLoudness/75,0.5,7*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(1*Sound.PlaybackLoudness/75,0,10*Sound.PlaybackLoudness/75), Size2 = VT(7*Sound.PlaybackLoudness/75,0.69,1*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(4*Sound.PlaybackLoudness/75,0,4*Sound.PlaybackLoudness/75), Size2 = VT(4*Sound.PlaybackLoudness/75,0.5,4*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = BrickColor.Random().Color, SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
		elseif MODE == "Katana" then
			local HITFLOOR,HITPOS = Raycast(RootPart.Position, (CF(RootPart.Position, RootPart.Position + VT(0, -1, 0))).lookVector, 4, Character)
			local loudness = Sound.PlaybackLoudness
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(10*Sound.PlaybackLoudness/75,0,1*Sound.PlaybackLoudness/75), Size2 = VT(1*Sound.PlaybackLoudness/75,0.5,7*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(1*Sound.PlaybackLoudness/75,0,10*Sound.PlaybackLoudness/75), Size2 = VT(7*Sound.PlaybackLoudness/75,0.69,1*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = 12.5, EffectType = "Sphere", Size = VT(4*Sound.PlaybackLoudness/75,0,4*Sound.PlaybackLoudness/75), Size2 = VT(4*Sound.PlaybackLoudness/75,0.5,4*Sound.PlaybackLoudness/75), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CFrame.new(0,-3,0)*CFrame.Angles(RAD(0),RAD(Sound.PlaybackLoudness/666),RAD(0)), RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = MRANDOM(5,15),EffectType = "Slash", Size = VT(0,0.05,0), Size2 = VT(0.0625,0.015,0.0625)*MRANDOM(1,4), Transparency = 0.5, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-2,0)*CFrame.Angles(math.rad(math.random(-5,5)),math.rad(math.random(-360,360)),math.rad(math.random(-5,5))), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})		
			WACKYEFFECT({Time = 30, EffectType = "Sphere", Size = VT(0.5,0,0.5), Size2 = VT(0.2,25,0.2), Transparency = 0.3, Transparency2 = 1, CFrame = CF(HITPOS)*ANGLES(RAD(0),RAD(MRANDOM(0,360)),RAD(0))*CF(0,0,MRANDOM(3,15)) * ANGLES(RAD(MRANDOM(-15,15)), RAD(0), RAD(MRANDOM(-15,15))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-1,1)*5, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), UseBoomerangMath = true, SizeBoomerang = 50, SoundID = nil, SoundPitch = nil, SoundVolume = nil})	
		elseif MODE == "ByeBye" then
			WACKYEFFECT({Time = 12, EffectType = "Block", Size = Vector3.new(3,3,3)/3, Size2 = Vector3.new(0,0,0), Transparency = .5, Transparency2 = 1, CFrame = RightArm.CFrame*CF(0,-1.45,0), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.new( Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0, Sound.PlaybackLoudness/500,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			if MRANDOM(1,1) == 1 then
				local loudness = Sound.PlaybackLoudness
				WACKYEFFECT({Time = 2.5, EffectType = "Sphere", Size = VT(7+Sound.PlaybackLoudness/25,0.55,7+Sound.PlaybackLoudness/25), Size2 = VT(7+Sound.PlaybackLoudness/25,0.55,7+Sound.PlaybackLoudness/25), Transparency = 0, Transparency2 = 1, CFrame = RootPart.CFrame*CF(0,-3,0), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0+178*loudness/100,0,0), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			end
		elseif MODE == "Scary" then
			local HITFLOOR,HITPOS = Raycast(RootPart.Position, (CF(RootPart.Position, RootPart.Position + VT(0, -1, 0))).lookVector, 4, Character)
			local POSITION = CF(HITPOS)*ANGLES(RAD(0),RAD(MRANDOM(0,360)),RAD(0))*CF(MRANDOM(3,6),0,0).p
			local SPHEREFLOOR,SPHEREPOS = Raycast(POSITION+VT(0,1,0), (CF(POSITION, POSITION + VT(0, -1, 0))).lookVector, 5, Character)
			local loudness = Sound.PlaybackLoudness
			ShakeCam(0.1,loudness / 8)
			WACKYEFFECT({Time = 30, EffectType = "Sphere", Size = VT(0.5,0,0.5), Size2 = VT(0.2,25,0.2), Transparency = 0.3, Transparency2 = 1, CFrame = CF(HITPOS)*ANGLES(RAD(0),RAD(MRANDOM(0,360)),RAD(0))*CF(0,0,MRANDOM(3,15)) * ANGLES(RAD(MRANDOM(-15,15)), RAD(0), RAD(MRANDOM(-15,15))), MoveToPos = nil, RotationX = 0, RotationY = MRANDOM(-1,1)*5, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100), UseBoomerangMath = true, SizeBoomerang = 50, SoundID = nil, SoundPitch = nil, SoundVolume = nil})	
			WACKYEFFECT({Time = MRANDOM(10,30)*2, EffectType = "Sphere", Size = Vector3.new(1.5,1.5,1.5)*1, Size2 = Vector3.new(0,0,0), Transparency = 0, Transparency2 = 1, CFrame = CFrame.new(SPHEREPOS-Vector3.new(0,2,0))*CFrame.Angles(math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360))), MoveToPos = SPHEREPOS+Vector3.new(0,MRANDOM(15,25)/5,0), MRANDOM(-25,25)/35, RotationY = MRANDOM(-25,25)/35, RotationZ = MRANDOM(-25,25)/35, Material = "Neon", Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100), SoundID = nil, SoundPitch = MRANDOM(12,16)/10, SoundVolume = 2,RED = true})
			WACKYEFFECT({Time = 12, EffectType = "Block", Size = Vector3.new(3,3,3)/3, Size2 = Vector3.new(0,0,0), Transparency = .5, Transparency2 = 1, CFrame = RightArm.CFrame*CF(0,-1.45,0), MoveToPos = nil, RotationX = 0, RotationY = 0, RotationZ = 0, Material = "Neon", Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100), SoundID = nil, SoundPitch = nil, SoundVolume = nil})
			WACKYEFFECT({Time = MRANDOM(5,15), EffectType = "Skull", Size = Vector3.new(1.5,1.5,1.5)*3.95, Size2 = Vector3.new(0.425,0.425,0.425), Transparency = 0.25, Transparency2 = 1, CFrame = CFrame.new(SPHEREPOS-Vector3.new(0,2,0))*CFrame.Angles(math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360)),math.rad(MRANDOM(0,360))), MoveToPos = SPHEREPOS+Vector3.new(0,MRANDOM(25,35)/5,0), MRANDOM(-25,25)/35, RotationY = MRANDOM(-25,25)/35, RotationZ = MRANDOM(-25,25)/35, Material = "Neon", Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100), SoundID = nil, SoundPitch = MRANDOM(12,16)/10, SoundVolume = 2,RED = true})			
		end
	end
end))

--SIN = math.sin
--RAD = math.rad
--ANGLES = CFrame.Angles
--COS = math.cos
--CF = CFrame.new
--C3 = Color3.new
--VT = Vector3.new

--//=================================\\
--||      WRAP UP THE SCRIPT
--\\=================================//

local ActualVelocity = Vector3.new()

local antivoid = Instance.new("Part")
antivoid.Size = Vector3.new(400,10,400)
antivoid.Anchored = true
antivoid.Transparency = 1
antivoid.Parent = workspace
coroutine.resume(coroutine.create(function()
	while true do
		swait()
		if not alreadyfixing then
			antivoid.Position = Vector3.new(RootPart.Position.X,workspace.FallenPartsDestroyHeight+5,RootPart.Position.Z)
		end
	end
end))
while true do
	swait()
	while true do
		swait()
		if not alreadyfixing then
			for i,v in pairs(Character:GetChildren()) do
				if v:IsA("BasePart") and v.Anchored == false and v.Position.Y < (workspace.FallenPartsDestroyHeight + 50) then
					local flot = Instance.new("BodyPosition")
					local spen = Instance.new("BodyGyro")
					local hu = math.huge
					flot.MaxForce = Vector3.new(hu,hu,hu)
					spen.MaxTorque = Vector3.new(hu,hu,hu)
					local spown = nil
					for o,b in pairs(workspace:GetDescendants()) do
						if not b:IsDescendantOf(Character) and b:IsA("SpawnLocation") then
							spown = b
						end
					end
					if spown then
						RootPart.CFrame = CFrame.new(spown.Position.X,spown.Position.Y+(spown.Size.Y/2)+3,spown.Position.Z)
					else
						local base = workspace:FindFirstChild("Base")
						if not base then
							base = workspace:FindFirstChild("Baseplate")
						end
						if base then
							RootPart.CFrame = CFrame.new(math.clamp(RootPart.Position.X,-base.Size.X/2,base.Size.X/2),base.Position.Y+(base.Size.Y/2)+3,math.clamp(RootPart.Position.Z,-base.Size.X/2,base.Size.X/2))
						else
							RootPart.CFrame = CFrame.new(math.clamp(RootPart.Position.X,-100,100),20,math.clamp(RootPart.Position.Z,-100,100))
						end
					end
					flot.Position = RootPart.Position
					flot.Parent = RootPart
					spen.CFrame = RootPart.CFrame
					spen.Parent = RootPart
					coroutine.resume(coroutine.create(function()
						game:GetService("Debris"):AddItem(flot,1)
						game:GetService("Debris"):AddItem(spen,1)
					end))
				end
			end
			Torsovelocity = (ActualVelocity * Vector3.new(1,0,1)).magnitude
			if lplr.Name == USERNAME then
				Torsovelocity = (RootPart.Velocity * Vector3.new(1,0,1)).magnitude
			end 
			local WALKSPEEDVALUE = 6 / (Humanoid.WalkSpeed / 16)
			sine = sine + change
			local hit,pos = rayCast(RootPart.Position,(CFrame.new(RootPart.Position,RootPart.Position - Vector3.new(0,1,0))).lookVector,4,Character)
			--//=================================\\
			--||           ANIMATIONS 
			--\\=================================//
			
			
			--okay so go down to walk anim and fix that before anything else, if you have time to work on more tonight then please do nightmare first. then after that if you still want to continue then you may do whatever is labled. everything else that is not labled just leave alone.
			Player_Size = 1
			 if Anim == "Walk" and Torsovelocity > 1 then
					RootJoint.C1 = Clerp(RootJoint.C1,rc0 * CFrame.new(0,0,0.1 + 0.05 * math.cos(sine / 6)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),2 / 3)
					Neck.C1 = Clerp(Neck.C1,CFrame.new(0,-0.5,0) * CFrame.Angles(math.rad(-90),math.rad(0),math.rad(180)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0) - Head.RotVelocity.Y / 30),0.2 / 3)
					RightHip.C1 = Clerp(RightHip.C1,CFrame.new(0.5,.95-.2*math.sin(sine/12),-.15*math.sin(sine/12)) * CFrame.Angles(math.rad(-5),math.rad(90),math.rad(0)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(-10+35 * math.cos(sine / 12))),0.6 / 3)
					LeftHip.C1 = Clerp(LeftHip.C1,CFrame.new(-0.5,.95+.2*math.sin(sine/12),.15*math.sin(sine/12)) * CFrame.Angles(math.rad(-5),math.rad(-90),math.rad(0)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(10+35 * math.cos(sine / 12))),0.6 / 3)
			 elseif (Anim ~= "Walk") or (Torsovelocity < 1) then
					RootJoint.C1 = Clerp(RootJoint.C1,rc0 * CFrame.new() * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.2 / 3)
					Neck.C1 = Clerp(Neck.C1,CFrame.new(0,-0.5,0) * CFrame.Angles(math.rad(-90),math.rad(0),math.rad(180)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.2 / 3)
					RightHip.C1 = Clerp(RightHip.C1,CFrame.new(0.5,1,0) * CFrame.Angles(math.rad(0),math.rad(90),math.rad(0)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.7 / 3)
					LeftHip.C1 = Clerp(LeftHip.C1,CFrame.new(-0.5,1,0) * CFrame.Angles(math.rad(0),math.rad(-90),math.rad(0)) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.7 / 3)
				end
			 	if RootPart.Velocity.y > 1 and hit == nil then 
					Anim = "Jump"
					if ATTACK == false then
						RootJoint.C0 = Clerp(RootJoint.C0,rc0 * CFrame.new(0,0,0 ) * CFrame.Angles(math.rad(-5),math.rad(0),math.rad(0)),1 / 3)
						Neck.C0 = Clerp(Neck.C0,nc0 * CFrame.new(0,0 ,0 + ((1) - 1)) * CFrame.Angles(math.rad(-25),math.rad(0),math.rad(10)),1 / 3)
						RightShoulder.C0 = Clerp(RightShoulder.C0,CFrame.new(1.5,0.5,0) * CFrame.Angles(math.rad(-50),math.rad(0),math.rad(0 + 10 * math.cos(sine / 12))) * rscp,1 / 3)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0,CFrame.new(-1.5,0.5,0) * CFrame.Angles(math.rad(50),math.rad(0),math.rad(-25 - 10 * math.cos(sine / 12))) * lscp,1 / 3)
						RightHip.C0 = Clerp(RightHip.C0,CFrame.new(1,-0.4,-0.6) * CFrame.Angles(math.rad(1),math.rad(90),math.rad(0)) * CFrame.Angles(math.rad(-1 * math.sin(sine / 6)),math.rad(0),math.rad(0)),1 / 3)
						LeftHip.C0 = Clerp(LeftHip.C0,CFrame.new(-1,-1,0) * CFrame.Angles(math.rad(0),math.rad(-85),math.rad(0)) * CFrame.Angles(math.rad(-1 * math.sin(sine / 6)),math.rad(0),math.rad(0)),1 / 3)
					end
				elseif RootPart.Velocity.y < -1 and hit == nil then 
					Anim = "Fall"
					if ATTACK == false then
					RootJoint.C0 = Clerp(RootJoint.C0, ROOTC0 * CF(0, 0, 0) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.2 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(-20), RAD(0), RAD(0)), 0.2 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(45), RAD(0), RAD(25))* RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(-40), RAD(0), RAD(-20)) * LEFTSHOULDERC0, 0.2 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, -0.3) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-5), RAD(0), RAD(-20)), 0.2 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1, -0.3) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-5), RAD(0), RAD(20)), 0.2 / Animation_Speed)
					end
				elseif Torsovelocity < 1 and hit ~= nil then
					Anim = "Idle"
				if ATTACK == false and MODE == "Snake God" then
					if VALUE1 == false and math.random(1,55) == 1 then
						coroutine.resume(coroutine.create(function()
							VALUE1 = true
							wait(2)
							CreateSound(749189256,RootPart,2,math.random(5, 15) / 10,false)
							for i=1,25 do
								swait()
								FT.Parent = Torso
								FRA.Parent = RightArm
								FLA.Parent = LeftArm
								FRL.Parent = RightLeg
								FLL.Parent = LeftLeg
								for _,v in next, Character:GetDescendants() do
									if(v:IsA'DataModelMesh')then
										v.Offset = Vector3.new(math.random(-50,50)/100,math.random(-50,50)/100,math.random(-50,50)/100)
									end
								end		
							end
							VALUE1 = false
							FT.Parent = nil
							FRA.Parent = nil
							FLA.Parent = nil
							FRL.Parent = nil
							FLL.Parent = nil
							for _,v in next, Character:GetDescendants() do
								if(v:IsA'DataModelMesh')then
									v.Offset = VT(0,0,0)
								end
							end	
						end))
					end
					DOUBLED = false
					READYTODOUBLE = false
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0+.15*SIN(sine/32)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(40), RAD(-10), RAD(0)), 0.15 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(10+5*SIN(sine/24))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-10-5*SIN(sine/24))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1-.15*SIN(sine/32), 0) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8+2.5*SIN(sine/32)), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1-.15*SIN(sine/32), 0) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8+2.5*SIN(sine/32)), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					snap = math.random(1,72)
					if snap == 1 then	
						CreateSound(363808674,Head,3,1.3,false)
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-100000-Sound.PlaybackLoudness/7,100000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-99999-Sound.PlaybackLoudness/7,99999+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-200-Sound.PlaybackLoudness/7,48375935+Sound.PlaybackLoudness/7))), 1 / Animation_Speed) 
					end
				end
				if MODE == "test" and ATTACK == false then 
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0,0,3 - .5 * math.sin(sine/50)) * CFrame.Angles(math.rad(20),math.rad(0),math.rad(0)),0.7/3)
					Neck.C0 = Clerp(Neck.C0,NECKC0 * CFrame.new(0,0,0) * CFrame.Angles(math.rad(20),math.rad(10*math.cos(sine/100)),math.rad(0)),1)
					if math.random(1,60) == 1 then
						Neck.C0 = Clerp(Neck.C0,NECKC0 * CFrame.new(0,0,0) * CFrame.Angles(math.rad(20+math.random(-20,20)),math.rad((10*math.cos(sine/100))+math.random(-20,20)),math.rad(math.random(-20,20))),1)
					end
					RightShoulder.C0 = Clerp(RightShoulder.C0,CFrame.new(1.5,0.5,0) * CFrame.Angles(math.rad(-41.6-4*math.sin(sine/50)),math.rad(0),math.rad(0)) * RIGHTSHOULDERC0,0.7/3)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0,CFrame.new(-1.5,0.5,0) * CFrame.Angles(math.rad(20),math.rad(0),math.rad(-10-10*math.sin(sine/50))) * LEFTSHOULDERC0,0.7/3)
					RightHip.C0 = Clerp(RightHip.C0,CFrame.new(1,-1,-0.01) * CFrame.Angles(math.rad(10),math.rad(80),math.rad(10+10*math.sin(sine/50))),1/3)
					LeftHip.C0 = Clerp(LeftHip.C0,CFrame.new(-1,-1,-0.01) * CFrame.Angles(math.rad(20),math.rad(-80),math.rad(-10-10*math.sin(sine/50))),1/3)
				end
				if MODE == "Suffering" and ATTACK == false then 
					if VALUE1 == false and math.random(1,55) == 1 then
						coroutine.resume(coroutine.create(function()
							VALUE1 = true
							wait(2)
							CreateSound(333430981,RootPart,2,math.random(5, 15) / 10,false)
							for i=1,25 do
								swait()
								FT.Parent = Torso
								FRA.Parent = RightArm
								FLA.Parent = LeftArm
								FRL.Parent = RightLeg
								FLL.Parent = LeftLeg
								for _,v in next, Character:GetDescendants() do
									if(v:IsA'DataModelMesh')then
										v.Offset = VT(math.random(-50,50)/100,math.random(-50,50)/100,math.random(-50,50)/100)
									end
								end		
							end
							VALUE1 = false
							FT.Parent = nil
							FRA.Parent = nil
							FLA.Parent = nil
							FRL.Parent = nil
							FLL.Parent = nil
							for _,v in next, Character:GetDescendants() do
								if(v:IsA'DataModelMesh')then
									v.Offset = VT(0,0,0)
								end
							end	
						end))
					end
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end
					if math.random(1,8) == 1 then
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-87498,12093847)), RAD(MRANDOM(-123456,3746525)), RAD(MRANDOM(-2134567876,98764356))), 0.15 / Animation_Speed)
					end
					if(math.random(1,4)==1)then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					end	
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end
					local bouncyboi = Sound.PlaybackLoudness / 1200
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, -0.1, -0.1 + 0.05 * COS(SINE / 12) + bouncyboi) * ANGLES(RAD(15), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.025 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(0 - 7.5 * SIN(SINE / 12)), RAD(12 + 7.5 * SIN(SINE / 12))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-0.7, 0.5 + Sound.PlaybackLoudness / 1200, -0.3) * ANGLES(RAD(-200), RAD(0), RAD(30)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12) - bouncyboi, -0.01) * ANGLES(RAD(20), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12) - bouncyboi, -0.01) * ANGLES(RAD(5), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(25 + MRANDOM(-5,5) - 4 * COS(SINE / 12)), RAD(MRANDOM(-5,5)), RAD(15)), 1 / Animation_Speed)--]
					snap = math.random(1,72)
					if snap == 1 then
						CreateSound(363808674,Head,3,1.3,false)
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-100000-Sound.PlaybackLoudness/7,100000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-99999-Sound.PlaybackLoudness/7,99999+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-200-Sound.PlaybackLoudness/7,48375935+Sound.PlaybackLoudness/7))), 1 / Animation_Speed) 
					end 
					if MRANDOM(1,20+Sound.PlaybackLoudness/7) == 1 then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-90-Sound.PlaybackLoudness/7,90+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-30-Sound.PlaybackLoudness/7,30+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-50-Sound.PlaybackLoudness/7,50+Sound.PlaybackLoudness/7)))* RIGHTSHOULDERC0, 1 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-10000-Sound.PlaybackLoudness/7,10000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-900-Sound.PlaybackLoudness/7,900+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-20-Sound.PlaybackLoudness/7,20+Sound.PlaybackLoudness/7)))* LEFTSHOULDERC0, 1 / Animation_Speed)
					end		   
					if MRANDOM(1, 10) == 1 then
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(0 + MRANDOM(-25,25) - 4 * COS(SINE / 12)), RAD(MRANDOM(-25,25)), RAD(0)), 1.5 / Animation_Speed)
					end
				end
				if MODE == "fuck" and ATTACK == false then 
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(35), RAD(0), RAD(0)), 0.25 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.25) - 1)) * ANGLES(RAD(35), RAD(0), RAD(0)), 1 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.3, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(200)) * RIGHTSHOULDERC0, 1 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.3, 0.5, 0) * ANGLES(RAD(0), RAD(0), RAD(-200)) * LEFTSHOULDERC0, 1 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -0.5 - 0.05 * COS(SINE / 12), -0.5) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -0.8 - 0.05 * COS(SINE / 12), -0.01) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
				end
				if MODE == "Scary" and ATTACK == false then
					if(math.random(1,4)==1)then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					end	
					if math.random(1,25) == 1 then
						Neck.C0 = Clerp(Neck.C0,NECKC0*CF(0,0,0+((1)-1))*ANGLES(math.rad(math.random(-10000,10000)),math.rad(math.random(-10000,10000)),math.rad(math.random(-10000,10000))),1.5/Animation_Speed)
					end	
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 0 + 0.1 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(0+MRANDOM(-5,5)), RAD(0+MRANDOM(-5,5)), RAD(0+MRANDOM(-5,5))), 0.35 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(MRANDOM(-25,25)), RAD(12)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(20), RAD(-20)) * LEFTSHOULDERC0, 0.5 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1 - 0.05 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(80), RAD(0)) * ANGLES(RAD(-3), RAD(0), RAD(0)), 1 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.05 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(-80), RAD(0)) * ANGLES(RAD(-3), RAD(0), RAD(0)), 1 / Animation_Speed)
					if MRANDOM(1,20+Sound.PlaybackLoudness/7) == 1 then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-90-Sound.PlaybackLoudness/7,90+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-30-Sound.PlaybackLoudness/7,30+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-50-Sound.PlaybackLoudness/7,50+Sound.PlaybackLoudness/7)))* RIGHTSHOULDERC0, 1 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-10000-Sound.PlaybackLoudness/7,10000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-900-Sound.PlaybackLoudness/7,900+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-20-Sound.PlaybackLoudness/7,20+Sound.PlaybackLoudness/7)))* LEFTSHOULDERC0, 1 / Animation_Speed)
					end
					if(math.random(1,2)==1)then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					end	
				end
				if MODE == "Katana" and ATTACK == false then
					if VALUE1 == false and math.random(1,55) == 1 then
						coroutine.resume(coroutine.create(function()
							VALUE1 = true
							wait(2)
							CreateSound(333430981,RootPart,2,math.random(5, 15) / 10,false)
							for i=1,25 do
								swait()
								FT.Parent = Torso
								FRA.Parent = RightArm
								FLA.Parent = LeftArm
								FRL.Parent = RightLeg
								FLL.Parent = LeftLeg
								for _,v in next, Character:GetDescendants() do
									if(v:IsA'DataModelMesh')then
										v.Offset = VT(math.random(-50,50)/100,math.random(-50,50)/100,math.random(-50,50)/100)
									end
								end		
							end
							VALUE1 = false
							FT.Parent = nil
							FRA.Parent = nil
							FLA.Parent = nil
							FRL.Parent = nil
							FLL.Parent = nil
							for _,v in next, Character:GetDescendants() do
								if(v:IsA'DataModelMesh')then
									v.Offset = VT(0,0,0)
								end
							end	
						end))
					end
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end
					if math.random(1,8) == 1 then
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-87498,12093847)), RAD(MRANDOM(-123456,3746525)), RAD(MRANDOM(-2134567876,98764356))), 0.15 / Animation_Speed)
					end		
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 2 + 1 * COS(SINE / 18)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(15 - 2.5 * SIN(SINE / 12)), RAD(MRANDOM(-25,25)), RAD(0)), 0.15 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(0), RAD(MRANDOM(-25,25)), RAD(12)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(0), RAD(MRANDOM(-25,25)), RAD(-12)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1, 0) * ANGLES(RAD(-17 + 9.4 * COS(sine / 26)), RAD(80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -.5, -0.5) * ANGLES(RAD(-22 + 10.8 * COS(sine / 32)), RAD(-80), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
					snap = math.random(1,72)
					if snap == 1 then
						CreateSound(363808674,Head,3,1.3,false)
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-100000-Sound.PlaybackLoudness/7,100000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-99999-Sound.PlaybackLoudness/7,99999+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-200-Sound.PlaybackLoudness/7,48375935+Sound.PlaybackLoudness/7))), 1 / Animation_Speed) 
					end
					if MRANDOM(1,20+Sound.PlaybackLoudness/7) == 1 then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-90-Sound.PlaybackLoudness/7,90+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-30-Sound.PlaybackLoudness/7,30+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-50-Sound.PlaybackLoudness/7,50+Sound.PlaybackLoudness/7)))* RIGHTSHOULDERC0, 1 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-10000-Sound.PlaybackLoudness/7,10000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-900-Sound.PlaybackLoudness/7,900+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-20-Sound.PlaybackLoudness/7,20+Sound.PlaybackLoudness/7)))* LEFTSHOULDERC0, 1 / Animation_Speed)
					end
				end
				if MODE == "HELL" and ATTACK == false then
					if VALUE1 == false and math.random(1,55) == 1 then
						coroutine.resume(coroutine.create(function()
							VALUE1 = true
							wait(2)
							CreateSound(333430981,RootPart,2,math.random(5, 15) / 10,false)
							for i=1,25 do
								swait()
								FT.Parent = Torso
								FRA.Parent = RightArm
								FLA.Parent = LeftArm
								FRL.Parent = RightLeg
								FLL.Parent = LeftLeg
								for _,v in next, Character:GetDescendants() do
									if(v:IsA'DataModelMesh')then
										v.Offset = VT(math.random(-50,50)/100,math.random(-50,50)/100,math.random(-50,50)/100)
									end
								end		
							end
							VALUE1 = false
							FT.Parent = nil
							FRA.Parent = nil
							FLA.Parent = nil
							FRL.Parent = nil
							FLL.Parent = nil
							for _,v in next, Character:GetDescendants() do
								if(v:IsA'DataModelMesh')then
									v.Offset = VT(0,0,0)
								end
							end	
						end))
					end
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end
					if math.random(1,8) == 1 then
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(-87498,12093847)), RAD(MRANDOM(-123456,3746525)), RAD(MRANDOM(-2134567876,98764356))), 0.15 / Animation_Speed)
					end
					if(math.random(1,4)==1)then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5, 0) * ANGLES(RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999)), RAD(MRANDOM(-99999999,99999999))) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					end		
					if MRANDOM(1,10) == 1 then
						Neck.C0=Clerp(Torso.Neck.C0,NECKC0*angles(RAD(23 + MRANDOM(-5,5)),RAD(MRANDOM(-5,5)),RAD(22 + MRANDOM(-5,5))),1)
					end	
					bouncyboi = Sound.PlaybackLoudness / 1200
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0.1, 1 + 0.5 * COS(SINE / 18)) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0 , 0 + ((1) - 1)) * ANGLES(RAD(20), RAD(0), RAD(0)), 0.2 / Animation_Speed)	
					RightShoulder.C0 = Clerp(RightShoulder.C0,CF(1.5,0.5+.1*COS(SINE/36),-.3)*ANGLES(RAD(44.1),RAD(0),RAD(-25))*RIGHTSHOULDERC0,1/Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.25, 0.5, 0.5) * ANGLES(RAD(-45), RAD(0), RAD(45)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(0.5, -0.9 - 0.1 * COS(SINE / 1), -0.6) * ANGLES(RAD(0), RAD(-10), RAD(0)) * ANGLES(RAD(75), RAD(0), RAD(5)), 0.1 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-0.5, 0.1 - 0.1 * COS(SINE / 1), -0.6) * ANGLES(RAD(0), RAD(-10), RAD(0)) * ANGLES(RAD(25), RAD(0), RAD(-10)), 0.1 / Animation_Speed)
					if MRANDOM(1,20+Sound.PlaybackLoudness/7) == 1 then
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-90-Sound.PlaybackLoudness/7,90+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-30-Sound.PlaybackLoudness/7,30+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-50-Sound.PlaybackLoudness/7,50+Sound.PlaybackLoudness/7)))* RIGHTSHOULDERC0, 1 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.05 * SIN(SINE / 12), 0) * ANGLES(RAD(MRANDOM(-10000-Sound.PlaybackLoudness/7,10000+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-900-Sound.PlaybackLoudness/7,900+Sound.PlaybackLoudness/7)), RAD(MRANDOM(-20-Sound.PlaybackLoudness/7,20+Sound.PlaybackLoudness/7)))* LEFTSHOULDERC0, 1 / Animation_Speed)
					end
				end
				if MODE == "meme" and ATTACK == false then -- try to fix this but if not, It's no big deal examples are in the vid
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 , 0 , 00 + 0.2 * COS(SINE / 12)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0) * ANGLES(RAD(30), RAD(0), RAD(0 + 25 * COS(SINE / 20))), 0.15 / Animation_Speed)
					RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5+ 0.35 * SIN(SINE / 12), 0) * ANGLES(RAD(180), RAD(-15), RAD(0))* RIGHTSHOULDERC0, 0.15 / Animation_Speed)
					LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5, 0.5 + 0.35 * SIN(SINE / 12), 0) * ANGLES(RAD(0), RAD(0), RAD(-10 + 15 * COS(SINE / 12))) * ANGLES(RAD(0), RAD(15), RAD(0)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
					RightHip.C0 = Clerp(RightHip.C0, CF(1, -1- 0.2 * COS(SINE / 12), 0) * ANGLES(RAD(0), RAD(75), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1- 0.2 * COS(SINE / 12) , 0) * ANGLES(RAD(0), RAD(-75), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)	
				end
				if MODE == "ByeBye" and ATTACK == false then --this is one of my favorite forms.
					RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0*SIZE, 0*SIZE, 0*SIZE) * ANGLES(RAD(0), RAD(0), RAD(0)), 1 / Animation_Speed)
			        Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0*SIZE, 0*SIZE, 0*SIZE + ((1*SIZE) - 1)) * ANGLES(RAD(20 + MRANDOM(-24,24)), RAD(0 + MRANDOM(-24,24)), RAD(0 + MRANDOM(-24,24))), 1 / Animation_Speed)
			        RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5*SIZE, 0.5*SIZE, 0*SIZE) * ANGLES(RAD(180 + MRANDOM(-24,24)), RAD(0 + MRANDOM(-24,24)), RAD(-25 + MRANDOM(-24,24))) * RIGHTSHOULDERC0, 1 / Animation_Speed)
			        LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.5*SIZE, 0.5*SIZE, 0*SIZE) * ANGLES(RAD(180 + MRANDOM(-24,24)), RAD(0 + MRANDOM(-24,24)), RAD(25 + MRANDOM(-24,24))) * LEFTSHOULDERC0, 1 / Animation_Speed)
			        RightHip.C0 = Clerp(RightHip.C0, CF(1*SIZE, -1*SIZE, -0.01*SIZE) * ANGLES(RAD(0), RAD(85 + MRANDOM(-24,24)), RAD(0)) * ANGLES(RAD(-3), RAD(0), RAD(0)), 1 / Animation_Speed)
			        LeftHip.C0 = Clerp(LeftHip.C0, CF(-1*SIZE, -1*SIZE, -0.01*SIZE) * ANGLES(RAD(0), RAD(-85 + MRANDOM(-24,24)), RAD(0)) * ANGLES(RAD(-3), RAD(0), RAD(0)), 1 / Animation_Speed)
				end
			elseif Torsovelocity > 5 and hit ~= nil then
					Anim = "Walk"
				if ATTACK == false then
					if MODE == "Snake God" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" or MODE == "Scary" or MODE == "Suffering" then --fix the arm on this
						RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, -0.1) * ANGLES(RAD(5), RAD(0), RAD(0)), 0.15 / Animation_Speed)
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(MRANDOM(1, 2) - 2.5 * SIN(SINE / 12)), RAD(MRANDOM(1, 2)), RAD(MRANDOM(1, 2))), 1 / Animation_Speed)
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.5, 0.5, 0) * ANGLES(RAD(35 * COS(SINE / WALKSPEEDVALUE)), RAD(0), RAD(5)) * RIGHTSHOULDERC0, 0.35 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CFrame.new(-1.5, 0.5, 0 - 0.2 * math.cos(sine / 12)) * CFrame.Angles(math.rad(20 + 45 * math.cos(sine / 12)), math.rad(0 - 10 * math.cos(sine / 12)), math.rad(0 + 2.5 * math.cos(sine / 12))) * lscp, 1 / 3)
						RightHip.C0 = Clerp(RightHip.C0, CF(1 , -1 - 0.15 * COS(SINE / WALKSPEEDVALUE*2), -0.2+ 0.2 * COS(SINE / WALKSPEEDVALUE)) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(-15)), 2 / Animation_Speed)
						LeftHip.C0 = Clerp(LeftHip.C0, CF(-1, -1 - 0.15 * COS(SINE / WALKSPEEDVALUE*2), -0.2+ -0.2 * COS(SINE / WALKSPEEDVALUE)) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(15)), 2 / Animation_Speed)
					elseif MODE == "test" and ATTACK == false then 
						RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CFrame.new(0,0,3 - .5 * math.sin(sine/50)) * CFrame.Angles(math.rad(20),math.rad(0),math.rad(0)),0.7/3)
						Neck.C0 = Clerp(Neck.C0,NECKC0 * CFrame.new(0,0,0) * CFrame.Angles(math.rad(0),math.rad(0),math.rad(0)),0.7/3)
						RightShoulder.C0 = Clerp(RightShoulder.C0,CFrame.new(1.5,0.5,0) * CFrame.Angles(math.rad(-41.6-4*math.sin(sine/50)),math.rad(0),math.rad(0)) * RIGHTSHOULDERC0,0.7/3)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0,CFrame.new(-1.5,0.5,0) * CFrame.Angles(math.rad(20),math.rad(0),math.rad(-10-10*math.sin(sine/50))) * LEFTSHOULDERC0,0.7/3)
						RightHip.C0 = Clerp(RightHip.C0,CFrame.new(1,-1,-0.01) * CFrame.Angles(math.rad(-20),math.rad(80),math.rad(10+10*math.sin(sine/50))),1/3)
						LeftHip.C0 = Clerp(LeftHip.C0,CFrame.new(-1,-1,-0.01) * CFrame.Angles(math.rad(-10),math.rad(-80),math.rad(-10-10*math.sin(sine/50))),1/3)
					elseif MODE == "ByeBye" and ATTACK == false then 
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1) - 1)) * ANGLES(RAD(15 - 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)), 3 / Animation_Speed)
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(1.1, 0.35, 0.4) * ANGLES(RAD(135), RAD(0), RAD(3)) * ANGLES(RAD(0 - 1.5 * COS(SINE / 15) + 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)) * RIGHTSHOULDERC0, 0.15 / Animation_Speed)
						RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0 - 0.05 * COS(SINE / 15) + 0.05 * SIN(SINE / 15), 0, 0 + 0.05 * COS(SINE / 20)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.8 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1.4, 0.35, 0.4) * ANGLES(RAD(15), RAD(0), RAD(12)) * ANGLES(RAD(0 - 1.5 * COS(SINE / 15) + 2.5 * SIN(SINE / 12)), RAD(0), RAD(0)) * LEFTSHOULDERC0, 0.15 / Animation_Speed)
						RightHip.C0 = Clerp(RightHip.C0, CF(1 - 0.05 * COS(SINE / 15) + 0.05 * SIN(SINE / 15), -1 - 0.05 * COS(SINE / 20), -0.01) * ANGLES(RAD(0), RAD(83), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.8 / Animation_Speed)
						LeftHip.C0 = Clerp(LeftHip.C0, CF(-1 - 0.05 * COS(SINE / 15) + 0.05 * SIN(SINE / 15), -1 - 0.05 * COS(SINE / 20), -0.01) * ANGLES(RAD(0), RAD(-83), RAD(0)) * ANGLES(RAD(0), RAD(0), RAD(0)), 0.8 / Animation_Speed)	
					elseif MODE == "fuck" and ATTACK == false then
						RootJoint.C0 = Clerp(RootJoint.C0,ROOTC0 * CF(0, 0, 1 + 0.5 * COS(SINE / 12)) * ANGLES(RAD(-25 - 3 * SIN(SINE / 12)), RAD(0), RAD(-25)), 0.15 / Animation_Speed)
						Neck.C0 = Clerp(Neck.C0, NECKC0 * CF(0, 0, 0 + ((1.1*SIZE) - 1)) * ANGLES(RAD(23 - 3 * SIN(SINE / 12)), RAD(0), RAD(30)), 1 / Animation_Speed)
						RightShoulder.C0 = Clerp(RightShoulder.C0, CF(0.75*SIZE, 0.5*SIZE, -1*SIZE) * ANGLES(RAD(70), RAD(0), RAD(-70)) * ANGLES(RAD(20), RAD(25), RAD(-15)) * RIGHTSHOULDERC0, 0.4 / Animation_Speed)
						LeftShoulder.C0 = Clerp(LeftShoulder.C0, CF(-1*SIZE, 0.2*SIZE, -0.5*SIZE) * ANGLES(RAD(25), RAD(0), RAD(85)) * LEFTSHOULDERC0, 0.4 / Animation_Speed)
						RightHip.C0 = Clerp(RightHip.C0, CF(1*SIZE, -0.5*SIZE - 0.05*SIZE * COS(SINE / 12), -0.5*SIZE) * ANGLES(RAD(0), RAD(90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
						LeftHip.C0 = Clerp(LeftHip.C0, CF(-1*SIZE, -0.8*SIZE - 0.05*SIZE * COS(SINE / 12), -0.01*SIZE) * ANGLES(RAD(0), RAD(-90), RAD(0)) * ANGLES(RAD(-8), RAD(0), RAD(0)), 0.15 / Animation_Speed)
					end
				end
			end 
			if MODE == "test" or MODE == "Snake God" or MODE == "fuck" or MODE == "HELL" or MODE == "meme" or MODE == "Katana" or MODE == "ByeBye" then
				RightArm.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
				LeftArm.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
				Torso.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
				Head.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
				LeftLeg.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
				RightLeg.Color = Color3.new(Sound.PlaybackLoudness/500,0,0)
			end
			if MODE == "Scary" then
				RightArm.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				LeftArm.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				Head.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				Torso.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				LeftLeg.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
				RightLeg.Color = Color3.fromRGB(0,0,0+178*Sound.PlaybackLoudness/100)
			end
			if MODE == "Suffering" then
				RightArm.Color = BrickColor.Random().Color
				LeftArm.Color = BrickColor.Random().Color
				Head.Color = BrickColor.Random().Color
				Torso.Color = BrickColor.Random().Color
				LeftLeg.Color = BrickColor.Random().Color
				RightLeg.Color = BrickColor.Random().Color
			end
		end
	end
end