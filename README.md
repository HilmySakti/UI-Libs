# UI LIBS 
 *A Simple UI Template Using LUA Codes To Use. Example:*
 ```
 local lib = loadstring(game:HttpGet"https://raw.githubusercontent.com/HilmySakti/UI-Libs/master/discord%20lib.txt")()

local win = lib:Window("Navy Simulator")
local serv = win:Server("Navy Simulator", "shit ass game")

local cTab = serv:Channel("Character")
local autoTab = serv:Channel("AutoFarm")

local flySpeed = 3
local flying = false
local ws = 16
local js = 50

local autofarm = false

cTab:Slider("Walkspeed", 0,150,1, function(t)
   ws = t
end)

cTab:Slider("Jump Power", 0,150,1, function(t)
   jp = t
end)

cTab:Label("FLY CONTROLS : R-Up, F-Down, WASD")

cTab:Bind("Fly", Enum.KeyCode.B, function()
   flying = not flying
   if flying then
       game.Workspace.Gravity = 0
   else
       game.Workspace.Gravity = 196.19999694824
   end
end)
```
