# NEVERLOSE UI
## Nightly

![Screenshot 2023-10-05 160728](https://github.com/3345-c-a-t-s-u-s/NEVERLOSE-UI-Nightly/assets/117000269/87274dd2-d4a9-4624-9547-6e2225d253ea)

### Example Code
```lua
local NEVERLOSE = loadstring(game:HttpGet('https://raw.githubusercontent.com/3345-c-a-t-s-u-s/NEVERLOSE-UI-Nightly/main/source.lua'))()

local Window = NEVERLOSE:AddWindow('NEVERLOSE','Example')

Window:AddTabLabel('Example')

local TabExample = Window:AddTab("Example Tab","ads")
local Tab = Window:AddTab("Tab","ads")

local section = TabExample:AddSection('Section',"right")

section:AddLabel('Read Me!')


section:AddButton('Create Section',function()
	local as
	as = TabExample:AddSection('Ticket',"left")
	as:AddLabel('WHO ASKED?')
	as:AddButton('remove',function()
		as:Hide()
	end)
end)

Tab:AddSection('gayyyyyy','left')

section:AddToggle('Toggle',false,function() 
	
end)

section:AddToggle('Toggle',false,function() 

end)

section:AddToggle('Toggle',false,function() 

end)

section:AddKeybind('Keybind',Enum.KeyCode.F,function()
	
end)

section:AddSlider('Slider',0,10,4,function()

end)

section:AddDropdown('Dropdown',{1,2,3},3,function()

end)
```
