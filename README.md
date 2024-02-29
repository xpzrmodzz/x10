--create by FRITE--
while true do wait()
local args = {
    [1] = {
        ["multiply"] = 10,
        ["action"] = "hit",
        ["enemyHum"] = workspace.dummies.TrainingDummy10.Humanoid
    }
}

game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args))
end
