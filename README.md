-- Shadow Hub

local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
	vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
	wait(1)
	vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)

game.StarterGui:SetCore("SendNotification", {
	Title = "Shadow Hub luck block";
	Text = "Criado por V1nom"; -- what the text says (ofc)
	Duration = 20;
})


local ScreenGui = Instance.new("ScreenGui")
local ScriptMain = Instance.new("Frame")
local nadad = Instance.new("Frame")
local TextBox = Instance.new("TextBox")
local diamante = Instance.new("TextButton")
local rainbow = Instance.new("TextButton")
local open_box = Instance.new("TextBox")
local normal = Instance.new("TextButton")
local galx = Instance.new("TextButton")
local super = Instance.new("TextButton")
local Close = Instance.new("TextButton")
local Open = Instance.new("Frame")
local openbutton = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.CoreGui

ScriptMain.Name = "ScriptMain"
ScriptMain.Parent = ScreenGui
ScriptMain.Active = true
ScriptMain.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
ScriptMain.BorderColor3 = Color3.fromRGB(27, 42, 53)
ScriptMain.Position = UDim2.new(0.258337736, 0, 0.16215831, 0)
ScriptMain.Size = UDim2.new(0, 605, 0, 358)
ScriptMain.Visible = false

nadad.Name = "nada d+"
nadad.Parent = ScriptMain
nadad.Active = true
nadad.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
nadad.BorderColor3 = Color3.fromRGB(243, 255, 0)
nadad.Position = UDim2.new(0.218181819, 0, 0, 0)
nadad.Size = UDim2.new(0, 9, 0, 357)

TextBox.Parent = ScriptMain
TextBox.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
TextBox.Position = UDim2.new(0.261611134, 0, 0.506370008, 0)
TextBox.Size = UDim2.new(0, 200, 0, 50)
TextBox.Font = Enum.Font.SourceSans
TextBox.Text = "QUANTIA DE ITENS"
TextBox.TextColor3 = Color3.fromRGB(236, 236, 0)
TextBox.TextSize = 14.000
TextBox.TextStrokeColor3 = Color3.fromRGB(236, 236, 0)

diamante.Name = "diamante"
diamante.Parent = ScriptMain
diamante.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
diamante.Position = UDim2.new(0.808936536, 0, 0.208095357, 0)
diamante.Size = UDim2.new(0, 114, 0, 50)
diamante.Font = Enum.Font.SourceSans
diamante.Text = "Diamante luck"
diamante.TextColor3 = Color3.fromRGB(251, 255, 0)
diamante.TextScaled = true
diamante.TextSize = 14.000
diamante.TextWrapped = true
diamante.MouseButton1Click:connect(function()
	for i=8, open_box.Text do --This number means that you'll get 800 gears (you can change this)
		game.ReplicatedStorage.SpawnDiamondBlock:FireServer()
	end
end)

rainbow.Name = "rainbow"
rainbow.Parent = ScriptMain
rainbow.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
rainbow.Position = UDim2.new(0.755589843, 0, 0.0264519602, 0)
rainbow.Size = UDim2.new(0, 92, 0, 40)
rainbow.Font = Enum.Font.SourceSans
rainbow.Text = "Rainbow luck"
rainbow.TextColor3 = Color3.fromRGB(251, 255, 0)
rainbow.TextScaled = true
rainbow.TextSize = 14.000
rainbow.TextWrapped = true
rainbow.MouseButton1Click:connect(function()
	for i=1, open_box.Text do --This number means that you'll get 100 gears (you can change this)
		game.ReplicatedStorage.SpawnRainbowBlock:FireServer()
	end
end)


open_box.Name = "open_box"
open_box.Parent = ScriptMain
open_box.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
open_box.Position = UDim2.new(0.262773573, 0, 0.304762036, 0)
open_box.Size = UDim2.new(0, 194, 0, 50)
open_box.Font = Enum.Font.SourceSans
open_box.Text = "1"
open_box.TextColor3 = Color3.fromRGB(255, 238, 0)
open_box.TextSize = 14.000
open_box.TextStrokeColor3 = Color3.fromRGB(255, 238, 0)

normal.Name = "normal"
normal.Parent = ScriptMain
normal.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
normal.Position = UDim2.new(0.524112225, 0, -0.00148096681, 0)
normal.Size = UDim2.new(0, 114, 0, 50)
normal.Font = Enum.Font.SourceSans
normal.Text = "Normal luck"
normal.TextColor3 = Color3.fromRGB(251, 255, 0)
normal.TextScaled = true
normal.TextSize = 14.000
normal.TextWrapped = true
normal.MouseButton1Click:connect(function()
	for i=1, open_box.Text do --This number means that you'll get 100 gears (you can change this)
		game.ReplicatedStorage.SpawnLuckyBlock:FireServer()
	end
end)

galx.Name = "galx"
galx.Parent = ScriptMain
galx.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
galx.Position = UDim2.new(0.289710283, 0, -0.00148096681, 0)
galx.Size = UDim2.new(0, 114, 0, 50)
galx.Font = Enum.Font.SourceSans
galx.Text = "Galax luck"
galx.TextColor3 = Color3.fromRGB(251, 255, 0)
galx.TextScaled = true
galx.TextSize = 14.000
galx.TextWrapped = true
galx.MouseButton1Click:connect(function()
	for i=1, open_box.Text do --This number means that you'll get 100 gears (you can change this)
		game.ReplicatedStorage.SpawnGalaxyBlock:FireServer()
	end
end)

super.Name = "super"
super.Parent = ScriptMain
super.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
super.Position = UDim2.new(0.808936536, 0, 0.364519954, 0)
super.Size = UDim2.new(0, 114, 0, 50)
super.Font = Enum.Font.SourceSans
super.Text = "ISANO"
super.TextColor3 = Color3.fromRGB(251, 255, 0)
super.TextScaled = true
super.TextSize = 14.000
super.TextWrapped = true
super.MouseButton1Click:connect(function()
	for i=1, open_box.Text do --This number means that you'll get 100 gears (you can change this)
		game.ReplicatedStorage.SpawnSuperBlock:FireServer()
	end
end)

Close.Name = "Close"
Close.Parent = ScriptMain
Close.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
Close.Position = UDim2.new(0.952284038, 0, -0.001480937, 0)
Close.Size = UDim2.new(0, 27, 0, 37)
Close.Font = Enum.Font.SourceSans
Close.Text = "X"
Close.TextColor3 = Color3.fromRGB(251, 255, 0)
Close.TextScaled = true
Close.TextSize = 14.000
Close.TextWrapped = true
Close.MouseButton1Click:connect(function()
	ScriptMain.Visible = false
	Open.Visible = true
end)

Open.Name = "Open"
Open.Parent = ScreenGui
Open.Active = true
Open.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
Open.BorderColor3 = Color3.fromRGB(27, 42, 53)
Open.Position = UDim2.new(0, 0, 0.469938636, 0)
Open.Size = UDim2.new(0, 238, 0, 45)

openbutton.Name = "openbutton"
openbutton.Parent = Open
openbutton.BackgroundColor3 = Color3.fromRGB(27, 42, 53)
openbutton.Position = UDim2.new(-0.132718652, 0, -0.0189502537, 0)
openbutton.Size = UDim2.new(0, 269, 0, 50)
openbutton.Font = Enum.Font.SourceSans
openbutton.Text = "Open"
openbutton.TextColor3 = Color3.fromRGB(255, 226, 0)
openbutton.TextSize = 14.000
openbutton.MouseButton1Click:connect(function()
	ScriptMain.Visible = true
	Open.Visible = false
end)
