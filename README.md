if game.PlaceId == 8908228901 then -- SharkBite2
local DiscordLib = loadstring(game:HttpGet("https://pastebin.com/raw/xcdmdnw0"))()
local win = DiscordLib:Window("SharkBite2")

local serv = win:Server("ByPFN", "")
local tgls = serv:Channel("AutoFarm")


-----------------------------------------------------------------------------------------
_G.weapon = true
tgls:Toggle("Auto AFK",true, function(bool)
    _G.weapon = bool
end)

spawn(function()
    while wait(1) do
      if _G.weapon then
        pcall(function() 
            


local args = {
    [1] = false
}

game:GetService("ReplicatedStorage").EventsFolder.GameLoop.ToggleSpectator:InvokeServer(unpack(args))

           
            wait(2)
        end)
      end
    end
end)

-----------------

_G.weapon = true
tgls:Toggle("เข้าเกม",true, function(bool)
    _G.weapon = bool
end)

spawn(function()
    while wait(1) do
      if _G.weapon then
        pcall(function() 
            


game:GetService("ReplicatedStorage").EventsFolder.Players.PlayerFinishedStartMenu:FireServer()

           
            wait(2)
        end)
      end
    end
end)




-----------------



_G.AFK = true
    tgls:Toggle("AFK เดิน",true, function(bool)
        _G.AKF = bool
    end)

spawn(function()
    while wait() do
        if _G.AKF then
        pcall(function() 
            local VirtualUser = game:GetService("VirtualUser")
            VirtualUser:CaptureController()
            VirtualUser:SetKeyDown("W",key)
            wait(1)
            VirtualUser:CaptureController()
            VirtualUser:SetKeyUp("W",key)
            wait(1)
        end)
    end
end
end)


-----------------

end
