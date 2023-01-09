local RandomTransparencyBlock = workspace.RandomMaterial
Daniel18:07
workspace.Transperent.Transparency = 0.5
Олексій Калінін18:09
local FallingBlockOrigin = workspace.FallingBlock.Position
workspace.FallingBlock.Position = FallingBlockOrigin
wait(2)

workspace.FallingBlock.Position = FallingBlockOrigin
wait(2)

workspace.FallingBlock.Position = FallingBlockOrigin
wait(2)

workspace.FallingBlock.Position = FallingBlockOrigin
wait(2)

workspace.FallingBlock.Position = FallingBlockOrigin
wait(2)



function spike(partTouching)
	if partTouching.Parent:FindFirstChild("Humanoid") then-- Ця функція вказує що при дотику персонажа до шипів він втрачає здоровя
		partTouching.Parent.Humanoid.Health = 0
	end
end

script.Parent.Touched:Connect(spike)-- тут відбувається реалізація функції
Святослав Панчишин20:06
function spike(partTouching)
	if partTouching.Parent:FindFirstChild("Humanoid") then
		partTouching.Parent.Humanoid.Health = 0
	end
end

script.Parent.Touched:Connect(spike)
