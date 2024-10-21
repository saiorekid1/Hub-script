-- Carregar a biblioteca Orion
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

-- Criar a janela principal
local Window = OrionLib:MakeWindow({
    Name = "Onion Library Hub",
    HidePremium = false,
    SaveConfig = true,
    ConfigFolder = "OnionLibrary"
})

-- Criar uma aba
local Tab = Window:MakeTab({
    Name = "Scripts",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
})

-- Criar uma seção
local Section = Tab:AddSection({
    Name = "Admin Scripts"
})

-- Adicionar botões e funcionalidades
Section:AddButton({
    Name = "Infinite Yield",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source"))()
    end
})

Section:AddButton({
    Name = "Dex Explorer V3",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/peyton2465/Dex/master/out.lua"))()
    end
})

Section:AddButton({
    Name = "Admin Scripts",
    Callback = function()
        loadstring(game
