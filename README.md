# Simple-VGUI For GMOD
This is a simple vgui with a rainbow and slide text 

How to add a new line of text to the vgui?

local buttonSlide = HOTANIMATIONS.Menu:Add("DButton")
        buttonSlide:Dock(TOP)
        buttonSlide:SetText("")
        local speed = 3
        local rainbowColor
        buttonSlide.Paint = function(me,w,h)
            local offset = range * math.sin(CurTime() * speed)
            surface.SetDrawColor(buttonColor)
            surface.DrawRect(0,0,w,h)
            draw.SimpleText("Slie Button", "animation_24", w * .5 +offset, h * .5, color_white, TEXT_ALIGIN_CENTER, TEXT_ALIGIN_CENTER)
        end
        
just copy this and paste it then change the buttonSlide to what ever new button you want pretty easy

USE FOOKING GMOD WIKI


Made By SwayX
