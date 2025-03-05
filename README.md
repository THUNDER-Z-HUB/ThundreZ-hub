-- สมมุติว่ามีหลายแผนที่ที่เราใช้ในเกม
local mapName = "Mega Clickers , Fisch , The $1,000,000 Glass Bridge"
local currentMap = game.Workspace:FindFirstChild("Mega Clickers") -- คุณสามารถแทนชื่อแผนที่ด้วยชื่อของโมเดลใน Workspace
if currentMap then
    mapName = currentMap.Name
end

-- ตรวจสอบว่าแผนที่ไหนกำลังใช้งานอยู่ และโหลดสคริปต์ที่ตรงกัน
if mapName == "Mega Clickers" then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/THUNDER-Z-HUB/ThundreZ-hub/refs/heads/main/ThunderZhub.lua"))()
elseif mapName == "Fisch" then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/yourusername/script_map2.lua"))()
elseif mapName == "The $1,000,000 Glass Bridge" then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/yourusername/script_map3.lua"))()
