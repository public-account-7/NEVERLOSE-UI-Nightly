# NEVERLOSE UI
## Nightly
### Example Code
```lua
local NEVERLOSE = loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/NEVERLOSE-UI-Nightly/main/source.lua"))()

local function start()
	local Window = NEVERLOSE:AddWindow('NEVERLOSE','CSGO')

	Window:AddTabLabel('Example')

	local TabExample = Window:AddTab("Example Tab","earth") -- [ads,list,folder,earth,locked,home,mouse,user]
	local Tab = Window:AddTab("Tab","ads") 

	local section = TabExample:AddSection('Section',"right")

	section:AddLabel('Read Me!')


	section:AddButton('Create Section',function()
		local as
		as = TabExample:AddSection('Ticket',"left")
		as:AddLabel('Text Here')
		as:AddButton('</> Delete',function()
			as:Hide()
		end)
	end)

	Tab:AddSection('Test','left'):AddToggle("Auto Farm",false,function(val)
		
	end)

	section:AddToggle('Toggle',false,function() 

	end)

	section:AddToggle('Toggle',false,function() 

	end)

	section:AddToggle('Toggle',false,function() 

	end)

	section:AddKeybind('Keybind',Enum.KeyCode.F,function()

	end)

	section:AddSlider('Follow Speed',0,10,4,function()

	end)

	section:AddDropdown('Dropdown',{1,2,3},3,function()

	end)
end

local KeySystem = NEVERLOSE:KeySystem('Key System','https://httpbin.org/get',function()
	return true
end)

KeySystem:Callback(start)
```
