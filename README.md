-- create By FRITE
while true do
    wait()
    
    local args1 = {
        [1] = {
            ["multiply"] = 10,
            ["action"] = "hit",
            ["enemyHum"] = workspace.dummies.TrainingDummy10.Humanoid
        }
    }

    game:GetService("ReplicatedStorage").DamageEvent:FireServer(unpack(args1))

    local args2 = {
        [1] = {
            ["multiply"] = 10,
            ["action"] = "damage",
            ["enemyChar"] = workspace.dummies.TrainingDummy10
        }
    }

    game:GetService("ReplicatedStorage").Events.WaterbeamEvent:FireServer(unpack(args2))
end
