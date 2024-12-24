if game.PlaceId == 2753915549 then
   World1 = true
elseif game.PlaceId == 4442272183 then
   World2 = true
elseif game.PlaceId == 7449423635 then
   World3 = true
end

function CheckLevel2()
    local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
    if Old_World then
        if game.Players.LocalPlayer.Data.Level.Value == 1 or game.Players.LocalPlayer.Data.Level.Value <= 9 or SelectMonster == "" then -- Bandit
            Ms = "Bandit"
            NameQuest = "BanditQuest1"
            QuestLv = 1
            NameMon = "Bandit"
            CFrameQ = CFrame.new(1059.37195, 15.4495068, 1550.4231, 0.939700544, -0, -0.341998369, 0, 1, -0, 0.341998369, 0, 0.939700544)
            CFrameMon = CFrame.new(1353.44885, 3.40935516, 1376.92029, 0.776053488, -6.97791975e-08, 0.630666852, 6.99138596e-08, 1, 2.4612488e-08, -0.630666852, 2.49917598e-08, 0.776053488)
            Next_Level_X = 10
        elseif game.Players.LocalPlayer.Data.Level.Value == 10 or game.Players.LocalPlayer.Data.Level.Value <= 100 then
            Ms = "Shanda"
            NameQuest = "SkyExp1Quest"
            QuestLv = 2
            NameMon = "Shanda"
            CFrameQ = CFrame.new(-7859.09814, 5544.19043, -381.476196)
            CFrameMon = CFrame.new(-7904.57373, 5584.37646, -459.62973)

            Next_Level_X = 75
        elseif game.Players.LocalPlayer.Data.Level.Value >= 60 and game.Players.LocalPlayer.Data.Level.Value <= 75-1 or SelectMonster == "Desert Bandit" then
            Ms = "Desert Bandit"
            NameQuest = "DesertQuest"
            QuestLv = 1
            NameMon = "Desert Bandit"
            CFrameQ = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
            CFrameMon = CFrame.new(932.788818, 6.8503746, 4488.24609, -0.998625934, 3.08948351e-08, 0.0524050146, 2.79967303e-08, 1, -5.60361286e-08, -0.0524050146, -5.44919629e-08, -0.998625934)
        elseif game.Players.LocalPlayer.Data.Level.Value >= 75 and game.Players.LocalPlayer.Data.Level.Value <= 90-1 or SelectMonster == "Desert Officer" then
            Ms = "Desert Officer"
            NameQuest = "DesertQuest"
            QuestLv = 2
            NameMon = "Desert Officer"
            CFrameQ = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
            CFrameMon = CFrame.new(1617.07886, 1.5542295, 4295.54932, -0.997540116, -2.26287735e-08, -0.070099175, -1.69377223e-08, 1, -8.17798806e-08, 0.070099175, -8.03913949e-08, -0.997540116)
            
            SelectMonster = "Desert Bandit"
            Next_Level_X = 90
        elseif game.Players.LocalPlayer.Data.Level.Value >= 90 and game.Players.LocalPlayer.Data.Level.Value <= 100-1 or SelectMonster == "Snow Bandit" then -- Snow Bandits
            Ms = "Snow Bandit"
            NameQuest = "SnowQuest"
            QuestLv = 1
            NameMon = "Snow Bandit"
            CFrameQ = CFrame.new(1389.74451, 86.6520844, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
            CFrameMon = CFrame.new(1412.92346, 55.3503647, -1260.62036, -0.246266365, -0.0169920288, -0.969053388, 0.000432241941, 0.999844253, -0.0176417865, 0.969202161, -0.00476344163, -0.246220857)
            
            if SelectMonster == "Snow Bandit" then
            else
                Next_Level_X = 100
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 110 then
                SelectBoss_P = "Yeti" 
            end
            
        elseif game.Players.LocalPlayer.Data.Level.Value == 100 or game.Players.LocalPlayer.Data.Level.Value <= 119 or SelectMonster == "Snowman" then -- Snowman
            Next_Level_X = 120
            Ms = "Snowman"
            NameQuest = "SnowQuest"
            QuestLv = 2
            NameMon = "Snowman"
            CFrameQ = CFrame.new(1389.74451, 86.6520844, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
            CFrameMon = CFrame.new(1376.86401, 97.2779999, -1396.93115, -0.986755967, 7.71178321e-08, -0.162211925, 7.71531674e-08, 1, 6.08143536e-09, 0.162211925, -6.51427134e-09, -0.986755967)
            
            
            if game.Players.LocalPlayer.Data.Level.Value >= 110 then
                SelectBoss_P = "Yeti" 
            end
            SelectMonster = "Snow Bandit"
        elseif game.Players.LocalPlayer.Data.Level.Value == 120 or game.Players.LocalPlayer.Data.Level.Value <= 174 or SelectMonster == "Chief Petty Officer" then -- Chief Petty Officer
            Ms = "Chief Petty Officer"
            NameQuest = "MarineQuest2"
            QuestLv = 1
            NameMon = "Chief Petty Officer"
            CFrameQ = CFrame.new(-5039.58643, 27.3500385, 4324.68018, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            CFrameMon = CFrame.new(-4882.8623, 22.6520386, 4255.53516, 0.273695946, -5.40380647e-08, -0.96181643, 4.37720793e-08, 1, -4.37274998e-08, 0.96181643, -3.01326679e-08, 0.273695946)
            
            
            if game.Players.LocalPlayer.Data.Level.Value >= 130 then
                SelectBoss_P = "Vice Admiral"
            end
            if SelectMonster == "Chief Petty Officer" then
            else
                Next_Level_X = 175
            end
        elseif SelectMonster == "Sky Bandit" then -- Sky Bandit
            Ms = "Sky Bandit"
            NameQuest = "SkyQuest"
            QuestLv = 1
            NameMon = "Sky Bandit"
            CFrameQ = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            CFrameMon = CFrame.new(-4959.51367, 365.39267, -2974.56812, 0.964867651, 7.74418396e-08, 0.262737453, -6.95931988e-08, 1, -3.91783708e-08, -0.262737453, 1.95171506e-08, 0.964867651)
            
            
        elseif game.Players.LocalPlayer.Data.Level.Value == 175 or game.Players.LocalPlayer.Data.Level.Value <= 190-1 or SelectMonster == "Dark Master" then -- Dark Master
            
            Ms = "Dark Master"
            NameQuest = "SkyQuest"
            QuestLv = 2
            NameMon = "Dark Master"
            CFrameQ = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            CFrameMon = CFrame.new(-5079.98096, 376.477356, -2194.17139, 0.465965867, -3.69776352e-08, 0.884802461, 3.40249851e-09, 1, 4.00000886e-08, -0.884802461, -1.56281423e-08, 0.465965867)
            
            SelectMonster = "Sky Bandit"
            if SelectMonster == "Dark Master" then
            else
                Next_Level_X = 190
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 190 or game.Players.LocalPlayer.Data.Level.Value <= 209 or SelectMonster == "Prisoner" then
            
            Ms = "Prisoner"
            QuestLv = 1
            NameQuest = "PrisonerQuest"
            NameMon = "Prisoner"
            CFrameQ = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
            CFrameMon = CFrame.new(5433.39307, 88.678093, 514.986877, 0.879988372, 0, -0.474995494, 0, 1, 0, 0.474995494, 0, 0.879988372)
            if game.Players.LocalPlayer.Data.Level.Value >= 220 then
                SelectBoss_P = "Warden" 
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 232 then
                SelectBoss_P = "Chief Warden"
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 242 then
                SelectBoss_P = "Thunder God"
            end
            if SelectMonster == "Prisoner" then
            else
                Next_Level_X = 210
            end
            Bypass_TP_Dis = true
        elseif game.Players.LocalPlayer.Data.Level.Value == 210 or game.Players.LocalPlayer.Data.Level.Value <= 249 or SelectMonster == "Dangerous Prisoner" then
            if game.Players.LocalPlayer.Data.Level.Value >= 220 then
                SelectBoss_P = "Warden" 
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 232 then
                SelectBoss_P = "Chief Warden"
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 242 then
                SelectBoss_P = "Thunder God"
            end
            Ms = "Dangerous Prisoner"
            QuestLv = 2
            NameQuest = "PrisonerQuest"
            NameMon = "Dangerous Prisoner"
            CFrameQ = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
            CFrameMon = CFrame.new(5433.39307, 88.678093, 514.986877, 0.879988372, 0, -0.474995494, 0, 1, 0, 0.474995494, 0, 0.879988372)
            SelectMonster = "Prisoner"
            Next_Level_X = 250
            Bypass_TP_Dis = true
        elseif game.Players.LocalPlayer.Data.Level.Value == 250 or game.Players.LocalPlayer.Data.Level.Value <= 274 or SelectMonster == "Toga Warrior" then -- Toga Warrior
            
            Ms = "Toga Warrior"
            NameQuest = "ColosseumQuest"
            QuestLv = 1
            NameMon = "Toga Warrior"
            CFrameQ = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
            CFrameMon = CFrame.new(-1779.97583, 44.6077499, -2736.35474, 0.984437346, 4.10396339e-08, 0.175734788, -3.62286876e-08, 1, -3.05844168e-08, -0.175734788, 2.3741821e-08, 0.984437346)
            
            if SelectMonster == "Toga Warrior" then
            else
                Next_Level_X = 275
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 275 or game.Players.LocalPlayer.Data.Level.Value <= 299 or SelectMonster == "Gladiator" then -- Gladiato
            
            Ms = "Gladiator"
            NameQuest = "ColosseumQuest"
            QuestLv = 2
            NameMon = "Gladiator"
            CFrameQ = CFrame.new(-1576.11743, 7.38933945, -2983.30762, 0.576966345, 1.22114863e-09, 0.816767931, -3.58496594e-10, 1, -1.24185606e-09, -0.816767931, 4.2370063e-10, 0.576966345)
            CFrameMon = CFrame.new(-1274.75903, 58.1895943, -3188.16309, 0.464524001, 6.21005611e-08, 0.885560572, -4.80449414e-09, 1, -6.76054768e-08, -0.885560572, 2.71497012e-08, 0.464524001)
            
            SelectMonster = "Toga Warrior"
            Next_Level_X = 300
        elseif game.Players.LocalPlayer.Data.Level.Value == 300 or game.Players.LocalPlayer.Data.Level.Value <= 324 or SelectMonster == "Military Soldier" then -- Military Soldier
            if game.Players.LocalPlayer.Data.Level.Value >= 350 then
                SelectBoss_P = "Magma Admiral"
            end
            Ms = "Military Soldier"
            NameQuest = "MagmaQuest"
            QuestLv = 1
            NameMon = "Military Soldier"
            CFrameQ = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
            CFrameMon = CFrame.new(-5363.01123, 41.5056877, 8548.47266, -0.578253984, -3.29503091e-10, 0.815856814, 9.11209668e-08, 1, 6.498761e-08, -0.815856814, 1.11920997e-07, -0.578253984)
            
            if SelectMonster == "Military Soldier" then
            else
                Next_Level_X = 325
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 325 or game.Players.LocalPlayer.Data.Level.Value <= 374 or SelectMonster == "Military Spy" then -- Military Spy
            if game.Players.LocalPlayer.Data.Level.Value >= 350 then
                SelectBoss_P = "Magma Admiral"
            end
            Ms = "Military Spy"
            NameQuest = "MagmaQuest"
            QuestLv = 2
            NameMon = "Military Spy"
            CFrameQ = CFrame.new(-5316.55859, 12.2370615, 8517.2998, 0.588437557, -1.37880001e-08, -0.808542669, -2.10116209e-08, 1, -3.23446478e-08, 0.808542669, 3.60215964e-08, 0.588437557)
            CFrameMon = CFrame.new(-5787.99023, 120.864456, 8762.25293, -0.188358366, -1.84706277e-08, 0.982100308, -1.23782129e-07, 1, -4.93306951e-09, -0.982100308, -1.22495649e-07, -0.188358366)
            
            
            SelectMonster = "Military Soldier"
            Next_Level_X = 375
        elseif game.Players.LocalPlayer.Data.Level.Value == 375 or game.Players.LocalPlayer.Data.Level.Value <= 399 or SelectMonster == "Fishman Warrior" then -- Fishman Warrior
            if game.Players.LocalPlayer.Data.Level.Value >= 425 then
                SelectBoss_P = "Fishman Lord"
            end
            Ms = "Fishman Warrior"
            NameQuest = "FishmanQuest"
            QuestLv = 1
            NameMon = "Fishman Warrior"
            CFrameQ = CFrame.new(61122.5625, 18.4716396, 1568.16504)
            CFrameMon = CFrame.new(60946.6094, 48.6735229, 1525.91687, -0.0817126185, 8.90751153e-08, 0.996655822, 2.00889794e-08, 1, -8.77269599e-08, -0.996655822, 1.28533992e-08, -0.0817126185)
            if SelectMonster == "Fishman Warrior" then
            else
                Next_Level_X = 400
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 400 or game.Players.LocalPlayer.Data.Level.Value <= 449 or SelectMonster == "Fishman Commando" then -- Fishman Commando
            if game.Players.LocalPlayer.Data.Level.Value >= 425 then
                SelectBoss_P = "Fishman Lord"
            end
            Ms = "Fishman Commando"
            NameQuest = "FishmanQuest"
            QuestLv = 2
            NameMon = "Fishman Commando"
            CFrameQ = CFrame.new(61122.5625, 18.4716396, 1568.16504)
            CFrameMon = CFrame.new(61902.7383, 18.4828358, 1478.33936, -0.803795099, 0, -0.594906271, 0, 1, 0, 0.594906271, 0, -0.803795099)
            if SelectMonster == "Fishman Commando" then
            else
                Next_Level_X = 450
            end
            SelectMonster = "Fishman Warrior"
        elseif game.Players.LocalPlayer.Data.Level.Value == 450 or game.Players.LocalPlayer.Data.Level.Value <= 474 or SelectMonster == "God's Guard" then 
            Ms = "God's Guard"
            NameQuest = "SkyExp1Quest"
            QuestLv = 1
            NameMon = "God's Guards"
            CFrameQ = CFrame.new(-4721.71436, 845.277161, -1954.20105)
            CFrameMon = CFrame.new(-4716.95703, 853.089722, -1933.925427)
            if SelectMonster == "God's Guard" then
            else
                Next_Level_X = 475
            end
            SelectMonster = "Fishman Commando"
        elseif game.Players.LocalPlayer.Data.Level.Value == 475 or game.Players.LocalPlayer.Data.Level.Value <= 524 or SelectMonster == "Shanda" then
            Ms = "Shanda"
            NameQuest = "SkyExp1Quest"
            QuestLv = 2
            NameMon = "Shandas"
            CFrameQ = CFrame.new(-7859.09814, 5544.19043, -381.476196)
            CFrameMon = CFrame.new(-7904.57373, 5584.37646, -459.62973)
            if game.Players.LocalPlayer.Data.Level.Value >= 500 then
                SelectBoss_P = "Wysper"
            end
            if SelectMonster == "Shanda" then
            else
                Next_Level_X = 525
            end
            SelectMonster = "God's Guard"
        elseif game.Players.LocalPlayer.Data.Level.Value == 525 or game.Players.LocalPlayer.Data.Level.Value <= 549 or SelectMonster == "Royal Squad" then -- Royal Squad
            
            Ms = "Royal Squad"
            NameQuest = "SkyExp2Quest"
            QuestLv = 1
            NameMon = "Royal Squad"
            CFrameQ = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            CFrameMon = CFrame.new(-7555.04199, 5606.90479, -1303.24744, -0.896107852, -9.6057462e-10, -0.443836004, -4.24974544e-09, 1, 6.41599973e-09, 0.443836004, 7.63560326e-09, -0.896107852)
            
            
            if SelectMonster == "Royal Squad" then
            else
                Next_Level_X = 550
            end
            SelectMonster = "Shanda"
        elseif game.Players.LocalPlayer.Data.Level.Value == 550 or game.Players.LocalPlayer.Data.Level.Value <= 624 or SelectMonster == "Royal Soldier" then -- Royal Soldier
            if game.Players.LocalPlayer.Data.Level.Value >= 575 then
                SelectBoss_P = "Thunder God"
            end
            Ms = "Royal Soldier"
            NameQuest = "SkyExp2Quest"
            QuestLv = 2
            NameMon = "Royal Soldier"
            CFrameQ = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            CFrameMon = CFrame.new(-7837.31152, 5649.65186, -1791.08582, -0.716008604, 0.0104285581, -0.698013008, 5.02521061e-06, 0.99988848, 0.0149335321, 0.69809103, 0.0106890313, -0.715928733)
            
            
            if SelectMonster == "Royal Soldier" then
            else
                Next_Level_X = 625
            end
            SelectMonster = "Royal Squad"
            
        elseif game.Players.LocalPlayer.Data.Level.Value == 625 or game.Players.LocalPlayer.Data.Level.Value <= 649 or SelectMonster == "Galley Pirate" then -- Galley Pirate
            
            Ms = "Galley Pirate"
            NameQuest = "FountainQuest"
            QuestLv = 1
            NameMon = "Galley Pirate"
            CFrameQ = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
            CFrameMon = CFrame.new(5569.80518, 38.5269432, 3849.01196, 0.896460414, 3.98027495e-08, 0.443124533, -1.34262139e-08, 1, -6.26611296e-08, -0.443124533, 5.02237434e-08, 0.896460414)
            
            if SelectMonster == "Galley Pirate" then
            else
                Next_Level_X = 650
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 650 or SelectMonster == "Galley Captain" then -- Galley Captain
            if game.Players.LocalPlayer.Data.Level.Value >= 675 then
                SelectBoss_P = "Cyborg"
            end
            Ms = "Galley Captain"
            NameQuest = "FountainQuest"
            QuestLv = 2
            NameMon = "Galley Captain"
            CFrameQ = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
            CFrameMon = CFrame.new(5782.90186, 94.5326462, 4716.78174, 0.361808896, -1.24757526e-06, -0.932252586, 2.16989656e-06, 1, -4.96097414e-07, 0.932252586, -1.84339774e-06, 0.361808896)
            
            
            
            SelectMonster = "Galley Pirate"
            Next_Level_X = 9999
        end
    end
    if New_World then
        if game.Players.LocalPlayer.Data.Level.Value == 700 or game.Players.LocalPlayer.Data.Level.Value <= 724 or SelectMonster == "Raider" then -- Raider
            Ms = "Raider" 
            NameQuest = "Area1Quest"
            QuestLv = 1
            NameMon = "Raider"
            CFrameQ = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
            CFrameMon = CFrame.new(-737.026123, 10.1748352, 2392.57959, 0.272128761, 0, -0.962260842, -0, 1, -0, 0.962260842, 0, 0.272128761)
            
            if SelectMonster == "Raider" then
            else
                Next_Level_X = 725
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 725 or game.Players.LocalPlayer.Data.Level.Value <= 774 or SelectMonster == "Mercenary" then -- Mercenary
            if game.Players.LocalPlayer.Data.Level.Value >= 750 then
                SelectBoss_P = "Diamond"
            end
            Ms = "Mercenary"
            NameQuest = "Area1Quest"
            QuestLv = 2
            NameMon = "Mercenary"
            CFrameQ = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
            CFrameMon = CFrame.new(-1022.21271, 72.9855194, 1891.39148, -0.990782857, 0, -0.135460541, 0, 1, 0, 0.135460541, 0, -0.990782857)
            
            if SelectMonster == "Mercenary" then
            else
                Next_Level_X = 775
            end
            SelectMonster = "Raider"
        elseif game.Players.LocalPlayer.Data.Level.Value == 775 or game.Players.LocalPlayer.Data.Level.Value <= 799 or SelectMonster == "Swan Pirate" then -- Swan Pirate
            Ms = "Swan Pirate"
            NameQuest = "Area2Quest"
            QuestLv = 1
            NameMon = "Swan Pirate"
            CFrameQ = CFrame.new(638.43811, 71.769989, 918.282898, 0.139203906, 0, 0.99026376, 0, 1, 0, -0.99026376, 0, 0.139203906)
            CFrameMon = CFrame.new(976.467651, 111.174057, 1229.1084, 0.00852567982, -4.73897828e-08, -0.999963999, 1.12251888e-08, 1, -4.7295778e-08, 0.999963999, -1.08215579e-08, 0.00852567982)
            
            if SelectMonster == "Swan Pirate" then
            else
                Next_Level_X = 800
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 800 or game.Players.LocalPlayer.Data.Level.Value <= 874 or SelectMonster == "Factory Staff" then -- Factory Staff
            Ms = "Factory Staff"
            NameQuest = "Area2Quest"
            QuestLv = 2
            NameMon = "Factory Staff"
            CFrameQ = CFrame.new(638.43811, 71.769989, 918.282898, 0.139203906, 0, 0.99026376, 0, 1, 0, -0.99026376, 0, 0.139203906)
            CFrameMon = CFrame.new(336.74585, 73.1620483, -224.129272, 0.993632793, 3.40154607e-08, 0.112668738, -3.87658332e-08, 1, 3.99718729e-08, -0.112668738, -4.40850592e-08, 0.993632793)
            
            if SelectMonster == "Factory Staff" then
            else
                Next_Level_X = 875
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 850 then
                SelectBoss_P = "Jeremy"
            end
            SelectMonster = "Swan Pirate"
        elseif game.Players.LocalPlayer.Data.Level.Value == 875 or game.Players.LocalPlayer.Data.Level.Value <= 899 or SelectMonster == "Marine Lieutenant" then -- Marine Lieutenant
            Ms = "Marine Lieutenant"
            NameQuest = "MarineQuest3"
            QuestLv = 1
            NameMon = "Marine Lieutenant"
            CFrameQ = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            CFrameMon = CFrame.new(-2842.69922, 72.9919434, -2901.90479, -0.762281299, 0, -0.64724648, 0, 1.00000012, 0, 0.64724648, 0, -0.762281299)
            
            if SelectMonster == "Marine Lieutenant" then
            else
                Next_Level_X = 900
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 900 or game.Players.LocalPlayer.Data.Level.Value <= 949 or SelectMonster == "Marine Captain" then -- Marine Captain
            Ms = "Marine Captain"
            NameQuest = "MarineQuest3"
            QuestLv = 2
            NameMon = "Marine Captain"
            CFrameQ = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            CFrameMon = CFrame.new(-1814.70313, 72.9919434, -3208.86621, -0.900422215, 7.93464423e-08, -0.435017526, 3.68856199e-08, 1, 1.06050372e-07, 0.435017526, 7.94441988e-08, -0.900422215)
            if game.Players.LocalPlayer.Data.Level.Value >= 925 then
                SelectBoss_P = "Fajita"
            end
            if SelectMonster == "Marine Captain" then
            else
                Next_Level_X = 950
            end
            SelectMonster = "Marine Lieutenant"
        elseif game.Players.LocalPlayer.Data.Level.Value == 950 or game.Players.LocalPlayer.Data.Level.Value <= 974 or SelectMonster == "Zombie" then -- Zombie
            Ms = "Zombie"
            NameQuest = "ZombieQuest"
            QuestLv = 1
            NameMon = "Zombie"
            CFrameQ = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
            CFrameMon = CFrame.new(-5649.23438, 126.0578, -737.773743, 0.355238914, -8.10359282e-08, 0.934775114, 1.65461245e-08, 1, 8.04023372e-08, -0.934775114, -1.3095117e-08, 0.355238914)
            
            if SelectMonster == "Zombie" then
            else
                Next_Level_X = 975
            end
            Bypass_TP_Dis = true
        elseif game.Players.LocalPlayer.Data.Level.Value == 975 or game.Players.LocalPlayer.Data.Level.Value <= 999 or SelectMonster == "Vampire" then -- Vampire
            Ms = "Vampire"
            NameQuest = "ZombieQuest"
            QuestLv = 2
            NameMon = "Vampire"
            CFrameQ = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
            CFrameMon = CFrame.new(-6030.32031, 0.4377408, -1313.5564, -0.856965423, 3.9138893e-08, -0.515373945, -1.12178942e-08, 1, 9.45958547e-08, 0.515373945, 8.68467822e-08, -0.856965423)
            
            if SelectMonster == "Vampire" then
            else
                Next_Level_X = 1000
            end
            Bypass_TP_Dis = true
            SelectMonster = "Zombie"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1000 or game.Players.LocalPlayer.Data.Level.Value <= 1049 or SelectMonster == "Snow Trooper" then -- Snow Trooper **
            Ms = "Snow Trooper"
            NameQuest = "SnowMountainQuest"
            QuestLv = 1
            NameMon = "Snow Trooper"
            CFrameQ = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
            CFrameMon = CFrame.new(621.003418, 391.361053, -5335.43604, 0.481644779, 0, 0.876366913, 0, 1, 0, -0.876366913, 0, 0.481644779)
            
            if SelectMonster == "Snow Trooper" then
            else
                Next_Level_X = 1050
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 1050 or game.Players.LocalPlayer.Data.Level.Value <= 1099 or SelectMonster == "Winter Warrior" then -- Winter Warrior
            Ms = "Winter Warrior"
            NameQuest = "SnowMountainQuest"
            QuestLv = 2
            NameMon = "Winter Warrior"
            CFrameQ = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
            CFrameMon = CFrame.new(1295.62683, 429.447784, -5087.04492, -0.698032081, -8.28980049e-08, -0.71606636, -1.98835952e-08, 1, -9.63858184e-08, 0.71606636, -5.30424877e-08, -0.698032081)
            
            if SelectMonster == "Winter Warrior" then
            else
                Next_Level_X = 1100
            end
            SelectMonster = "Snow Trooper"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1100 or game.Players.LocalPlayer.Data.Level.Value <= 1124 or SelectMonster == "Lab Subordinate" then -- Lab Subordinate
            Ms = "Lab Subordinate"
            NameQuest = "IceSideQuest"
            QuestLv = 1
            NameMon = "Lab Subordinate"
            CFrameQ = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
            CFrameMon = CFrame.new(-5769.2041, 37.9288292, -4468.38721, -0.569419742, -2.49055017e-08, 0.822046936, -6.96206541e-08, 1, -1.79282633e-08, -0.822046936, -6.74401548e-08, -0.569419742)
            
            if SelectMonster == "Lab Subordinate" then
            else
                Next_Level_X = 1125
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 1125 or game.Players.LocalPlayer.Data.Level.Value <= 1174 or SelectMonster == "Horned Warrior" then -- Horned Warrior
            if game.Players.LocalPlayer.Data.Level.Value >= 1150 then
                SelectBoss_P = "Smoke Admiral"
            end
            Ms = "Horned Warrior"
            NameQuest = "IceSideQuest"
            QuestLv = 2
            NameMon = "Horned Warrior"
            CFrameQ = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
            CFrameMon = CFrame.new(-6401.27979, 15.9775667, -5948.24316, 0.388303697, 0, -0.921531856, 0, 1, 0, 0.921531856, 0, 0.388303697)
            
            if SelectMonster == "Horned Warrior" then
            else
                Next_Level_X = 1175
            end

            SelectMonster = "Lab Subordinate"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1175 or game.Players.LocalPlayer.Data.Level.Value <= 1199 or SelectMonster == "Magma Ninja" then -- Magma Ninja
            Ms = "Magma Ninja"
            NameQuest = "FireSideQuest"
            QuestLv = 1
            NameMon = "Magma Ninja"
            CFrameQ = CFrame.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            CFrameMon = CFrame.new(-5466.06445, 57.6952019, -5837.42822, -0.988835871, 0, -0.149006829, 0, 1, 0, 0.149006829, 0, -0.988835871)
            
            if SelectMonster == "Magma Ninja" then
            else
                Next_Level_X = 1200
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 1200 or game.Players.LocalPlayer.Data.Level.Value <= 1249 or SelectMonster == "Lava Pirate" then 
            Ms = "Lava Pirate"
            NameQuest = "FireSideQuest"
            QuestLv = 2
            NameMon = "Lava Pirate"
            CFrameQ = CFrame.new(-5431.09473, 15.9868021, -5296.53223, 0.831796765, 1.15322464e-07, -0.555080295, -1.10814341e-07, 1, 4.17010995e-08, 0.555080295, 2.68240168e-08, 0.831796765)
            CFrameMon = CFrame.new(-5169.71729, 34.1234779, -4669.73633, -0.196780294, 0, 0.98044765, 0, 1.00000012, -0, -0.98044765, 0, -0.196780294)
            
            if SelectMonster == "Lava Pirate" then
            else
                Next_Level_X = 1250
            end
            SelectMonster = "Magma Ninja"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1250 or game.Players.LocalPlayer.Data.Level.Value <= 1274 or SelectMonster == "Ship Deckhand" then 
            Ms = "Ship Deckhand"
            NameQuest = "ShipQuest1"
            QuestLv = 1
            NameMon = "Ship Deckhand"
            CFrameQ = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
            CFrameMon = CFrame.new(1163.80872, 138.288452, 33058.4258, -0.998580813, 5.49076979e-08, -0.0532564968, 5.57436763e-08, 1, -1.42118655e-08, 0.0532564968, -1.71604082e-08, -0.998580813)
            if SelectMonster == "Ship Deckhand" then
            else
                Next_Level_X = 1275
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 1275 or game.Players.LocalPlayer.Data.Level.Value <= 1299 or SelectMonster == "Ship Engineer" then 
            Ms = "Ship Engineer"
            NameQuest = "ShipQuest1"
            QuestLv = 2
            NameMon = "Ship Engineer"
            CFrameQ = CFrame.new(1037.80127, 125.092171, 32911.6016, -0.244533166, -0, -0.969640911, -0, 1.00000012, -0, 0.96964103, 0, -0.244533136)
            CFrameMon = CFrame.new(921.30249023438, 125.400390625, 32937.34375)
            if SelectMonster == "Ship Engineer" then
            else
                Next_Level_X = 1300
            end
            SelectMonster = "Ship Deckhand"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1300 or game.Players.LocalPlayer.Data.Level.Value <= 1324 or SelectMonster == "Ship Steward" then 
            Ms = "Ship Steward"
            NameQuest = "ShipQuest2"
            QuestLv = 1
            NameMon = "Ship Steward"
            CFrameQ = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
            CFrameMon = CFrame.new(917.96057128906, 136.89932250977, 33343.4140625)
            if SelectMonster == "Ship Steward" then
            else
                Next_Level_X = 1325
            end
            SelectMonster = "Ship Deckhand"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1325 or game.Players.LocalPlayer.Data.Level.Value <= 1349 or SelectMonster == "Ship Officer" then 
            Ms = "Ship Officer"
            NameQuest = "ShipQuest2"
            QuestLv = 2
            NameMon = "Ship Officer"
            CFrameQ = CFrame.new(968.80957, 125.092171, 33244.125, -0.869560242, 1.51905191e-08, -0.493826836, 1.44108379e-08, 1, 5.38534195e-09, 0.493826836, -2.43357912e-09, -0.869560242)
            CFrameMon = CFrame.new(944.44964599609, 181.40081787109, 33278.9453125)
            if SelectMonster == "Ship Officer" then
            else
                Next_Level_X = 1350
            end
            SelectMonster = "Ship Steward"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1350 or game.Players.LocalPlayer.Data.Level.Value <= 1374 or SelectMonster == "Arctic Warrior" then 
            Ms = "Arctic Warrior"
            NameQuest = "FrostQuest"
            QuestLv = 1
            NameMon = "Arctic Warrior"
            CFrameQ = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
            CFrameMon = CFrame.new(5878.23486, 81.3886948, -6136.35596, -0.451037169, 2.3908234e-07, 0.892505825, -1.08168464e-07, 1, -3.22542007e-07, -0.892505825, -2.4201924e-07, -0.451037169)
            
            if SelectMonster == "Arctic Warrior" then
            else
                Next_Level_X = 1375
            end
        elseif game.Players.LocalPlayer.Data.Level.Value == 1375 or game.Players.LocalPlayer.Data.Level.Value <= 1424 or SelectMonster == "Snow Lurker" then -- Snow Lurker
            if game.Players.LocalPlayer.Data.Level.Value >= 1400 then
                SelectBoss_P = "Awakened Ice Admiral"
            end
            Ms = "Snow Lurker"
            NameQuest = "FrostQuest"
            QuestLv = 2
            NameMon = "Snow Lurker"
            CFrameQ = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
            CFrameMon = CFrame.new(5513.36865, 60.546711, -6809.94971, -0.958693981, -1.65617333e-08, 0.284439981, -4.07668654e-09, 1, 4.44854642e-08, -0.284439981, 4.14883701e-08, -0.958693981)
            
            if SelectMonster == "Snow Lurker" then
            else
                Next_Level_X = 1450
            end
        
            SelectMonster = "Arctic Warrior"
        elseif game.Players.LocalPlayer.Data.Level.Value == 1425 or game.Players.LocalPlayer.Data.Level.Value <= 1449 or SelectMonster == "Sea Soldier" then -- Sea Soldier
            Ms = "Sea Soldier"
            NameQuest = "ForgottenQuest"
            QuestLv = 1
            NameMon = "Sea Soldier"
            CFrameQ = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
            CFrameMon = CFrame.new(-3115.78223, 63.8785706, -9808.38574, -0.913427353, 3.11199457e-08, 0.407000452, 7.79564235e-09, 1, -5.89660658e-08, -0.407000452, -5.06883708e-08, -0.913427353)
            
            if SelectMonster == "Sea Soldier" then
            else
                Next_Level_X = 1450
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1450 or SelectMonster == "Water Fighter" then -- Water Fighter
            if game.Players.LocalPlayer.Data.Level.Value >= 1475 then
                SelectBoss_P = "Tide Keeper"
            end
            Ms = "Water Fighter"
            NameQuest = "ForgottenQuest"
            QuestLv = 2
            NameMon = "Water Fighter"
            CFrameQ = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
            CFrameMon = CFrame.new(-3212.99683, 263.809296, -10551.8799, 0.742111444, -5.59139615e-08, -0.670276582, 1.69155214e-08, 1, -6.46908234e-08, 0.670276582, 3.66697037e-08, 0.742111444)
            
            if SelectMonster == "Water Fighter" then
            else
                Next_Level_X = 9999
            end
            SelectMonster = "Sea Soldier"
        end
    end
    if Three_World then
        if game.Players.LocalPlayer.Data.Level.Value >= 1500 and game.Players.LocalPlayer.Data.Level.Value <= 1524 or SelectMonster == "Pirate Millionaire" then -- Pirate Millionaire
            Ms = "Pirate Millionaire"
            NameQuest = "PiratePortQuest"
            QuestLv = 1
            NameMon = "Pirate Millionaire"
            CFrameQ = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
            
            if SelectMonster == "Pirate Millionaire" then
            else
                Next_Level_X = 1525
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1525 and game.Players.LocalPlayer.Data.Level.Value <= 1574 or SelectMonster == "Pistol Billionaire" then -- Pistol Billionaire
            if game.Players.LocalPlayer.Data.Level.Value >= 1550 then
                SelectBoss_P = "Stone"
            end
            Ms = "Pistol Billionaire"
            NameQuest = "PiratePortQuest"
            QuestLv = 2
            NameMon = "Pistol Billionaire"
            CFrameQ = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            CFrameMon = CFrame.new(81.164993286133, 43.755737304688, 5724.7021484375)
            
            if SelectMonster == "Pistol Billionaire" then
            else
                Next_Level_X = 1575 
            end
            
            SelectMonster = "Pirate Millionaire"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1575 and game.Players.LocalPlayer.Data.Level.Value <= 1599 or SelectMonster == "Dragon Crew Warrior" then -- Dragon Crew Warrior
            Ms = "Dragon Crew Warrior"
            NameQuest = "AmazonQuest"
            QuestLv = 1
            NameMon = "Dragon Crew Warrior"
            CFrameQ = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
            CFrameMon = CFrame.new(6241.9951171875, 51.522083282471, -1243.9771728516)
            
            if SelectMonster == "Dragon Crew Warrior" then
            else
                Next_Level_X = 1600
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1600 and game.Players.LocalPlayer.Data.Level.Value <= 1624 or SelectMonster == "Dragon Crew Archer" then -- Dragon Crew Archer
            Ms = "Dragon Crew Archer"
            NameQuest = "AmazonQuest"
            QuestLv = 2
            NameMon = "Dragon Crew Archer"
            CFrameQ = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
            CFrameMon = CFrame.new(6488.9155273438, 383.38375854492, -110.66246032715)
            
            if SelectMonster == "Dragon Crew Archer" then
            else
                Next_Level_X = 1625
            end
            SelectMonster = "Dragon Crew Warrior"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1625 and game.Players.LocalPlayer.Data.Level.Value <= 1649 or SelectMonster == "Female Islander" then 
            Ms = "Female Islander"
            NameQuest = "AmazonQuest2"
            QuestLv = 1
            NameMon = "Female Islander"
            CFrameQ = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(4770.4990234375, 758.95520019531, 1069.8680419922)
            
            if SelectMonster == "Female Islander" then
            else
                Next_Level_X = 1650
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1650 and game.Players.LocalPlayer.Data.Level.Value <= 1699 or SelectMonster == "Giant Islander" then -- Giant Islander
            Ms = "Giant Islander"
            NameQuest = "AmazonQuest2"
            QuestLv = 2
            NameMon = "Giant Islander"
            CFrameQ = CFrame.new(5448.86133, 601.516174, 751.130676, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            CFrameMon = CFrame.new(4530.3540039063, 656.75695800781, -131.60952758789)
            if game.Players.LocalPlayer.Data.Level.Value >= 1675 then
                SelectBoss_P = "Island Empress"
            end
            if SelectMonster == "Giant Islander" then
            else
                Next_Level_X = 1700
            end
        
            SelectMonster = "Female Islander"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1700 and game.Players.LocalPlayer.Data.Level.Value <= 1774 or SelectMonster == "Marine Commodore" then -- Marine Commodore
            Ms = "Marine Commodore"
            NameQuest = "MarineTreeIsland"
            QuestLv = 1
            NameMon = "Marine Commodore"
            CFrameQ = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
            CFrameMon = CFrame.new(2490.0844726563, 190.4232635498, -7160.0502929688)
            if game.Players.LocalPlayer.Data.Level.Value >= 1750 then
                SelectBoss_P = "Kilo Admiral"
            end
            if SelectMonster == "Marine Commodore" then
            else
                Next_Level_X = 1775
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1775 and game.Players.LocalPlayer.Data.Level.Value <= 1799 or SelectMonster == "Fishman Raider" then -- Fishman Raider
            Ms = "Fishman Raider"
            NameQuest = "DeepForestIsland3"
            QuestLv = 1
            NameMon = "Fishman Raider"
            CFrameQ = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            CFrameMon = CFrame.new(-10322.400390625, 390.94473266602, -8580.0908203125)
            
            if SelectMonster == "Fishman Raider" then
            else
                Next_Level_X = 1800
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1800 and game.Players.LocalPlayer.Data.Level.Value <= 1824 or SelectMonster == "Fishman Captain" then -- Fishman Captain
            Ms = "Fishman Captain"
            NameQuest = "DeepForestIsland3"
            QuestLv = 2
            NameMon = "Fishman Captain"
            CFrameQ = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            CFrameMon = CFrame.new(-11194.541992188, 442.02795410156, -8608.806640625)
            
            if SelectMonster == "Fishman Captain" then
            else
                Next_Level_X = 1825
            end
            SelectMonster = "Fishman Raider"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1825 and game.Players.LocalPlayer.Data.Level.Value <= 1849 or SelectMonster == "Forest Pirate" then -- Forest Pirate
            Ms = "Forest Pirate"
            NameQuest = "DeepForestIsland"
            QuestLv = 1
            NameMon = "Forest Pirate"
            CFrameQ = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
            CFrameMon = CFrame.new(-13225.809570313, 428.19387817383, -7753.1245117188)
            
            if SelectMonster == "Forest Pirate" then
            else
                Next_Level_X = 1850
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1850 and game.Players.LocalPlayer.Data.Level.Value <= 1899 or SelectMonster == "Mythological Pirate" then -- Mythological Pirate
            Ms = "Mythological Pirate"
            NameQuest = "DeepForestIsland"
            QuestLv = 2
            NameMon = "Mythological Pirate"
            CFrameQ = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
            CFrameMon = CFrame.new(-13869.172851563, 564.95251464844, -7084.4135742188)
            if game.Players.LocalPlayer.Data.Level.Value >= 1875 then
                SelectBoss_P = "Captain Elephant" 
            end
            if SelectMonster == "Mythological Pirate" then
            else
                Next_Level_X = 1900
            end
        
            SelectMonster = "Forest Pirate"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1900 and game.Players.LocalPlayer.Data.Level.Value <= 1924 or SelectMonster == "Jungle Pirate" then -- Jungle Pirate
            Ms = "Jungle Pirate"
            NameQuest = "DeepForestIsland2"
            QuestLv = 1
            NameMon = "Jungle Pirate"
            CFrameQ = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            CFrameMon = CFrame.new(-11982.221679688, 376.32522583008, -10451.415039063)
            
            if SelectMonster == "Jungle Pirate" then
            else
                Next_Level_X = 1925
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1925 and game.Players.LocalPlayer.Data.Level.Value <= 1974 or SelectMonster == "Musketeer Pirate" then -- Musketeer Pirate
            Ms = "Musketeer Pirate"
            NameQuest = "DeepForestIsland2"
            QuestLv = 2
            NameMon = "Musketeer Pirate"
            CFrameQ = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            CFrameMon = CFrame.new(-13282.3046875, 496.23684692383, -9565.150390625)
            
            if SelectMonster == "Musketeer Pirate" then
            else
                Next_Level_X = 1975
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 1950 then
                SelectBoss_P = "Beautiful Pirate"
            end
            SelectMonster = "Jungle Pirate"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 1975 and game.Players.LocalPlayer.Data.Level.Value <= 1999 or SelectMonster == "Reborn Skeleton" then
            Ms = "Reborn Skeleton"
            NameQuest = "HauntedQuest1"
            QuestLv = 1
            NameMon = "Reborn Skeleton"
            CFrameQ = CFrame.new(-9480.8271484375, 142.13066101074, 5566.0712890625)
            CFrameMon = CFrame.new(-8817.880859375, 191.16761779785, 6298.6557617188)
            
            if SelectMonster == "Reborn Skeleton" then
            elseif not LevelMax then
                Next_Level_X = 2000
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2000 and game.Players.LocalPlayer.Data.Level.Value <= 2024 or SelectMonster == "Living Zombie" then
            Ms = "Living Zombie"
            NameQuest = "HauntedQuest1"
            QuestLv = 2
            NameMon = "Living Zombie"
            CFrameQ = CFrame.new(-9480.8271484375, 142.13066101074, 5566.0712890625)
            CFrameMon = CFrame.new(-10125.234375, 183.94705200195, 6242.013671875)
            
            if SelectMonster == "Living Zombie" then
            elseif not LevelMax then
                Next_Level_X = 2025
            end
            SelectMonster = "Reborn Skeleton"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2025 and game.Players.LocalPlayer.Data.Level.Value <= 2049  or  SelectMonster == "Demonic Soul" then
            Ms = "Demonic Soul"
            NameQuest = "HauntedQuest2"
            QuestLv = 1
            NameMon = "Demonic"
            CFrameQ = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
            CFrameMon = CFrame.new(-9712.03125, 204.69589233398, 6193.322265625)
            
            if SelectMonster == "Demonic Soul" then
            else
                Next_Level_X = 2050
            end
            SelectMonster = "Living Zombie"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2050 and game.Players.LocalPlayer.Data.Level.Value <= 2074 or SelectMonster == "Posessed Mummy" then
            Ms = "Posessed Mummy"
            NameQuest = "HauntedQuest2"
            QuestLv = 2
            NameMon = "Posessed Mummy"
            CFrameQ = CFrame.new(-9516.9931640625, 178.00651550293, 6078.4653320313)
            CFrameMon = CFrame.new(-9545.7763671875, 69.619895935059, 6339.5615234375)    
            
            if SelectMonster == "Posessed Mummy" then
            else
                Next_Level_X = 2075
            end
            SelectMonster = "Demonic Soul"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2075 and game.Players.LocalPlayer.Data.Level.Value <= 2099 or SelectMonster == "Peanut Scout" then
            Ms = "Peanut Scout"
            NameQuest = "NutsIslandQuest"
            QuestLv = 1
            NameMon = "Peanut Scout"
            CFrameQ = CFrame.new(-2104.17163, 38.1299706, -10194.418, 0.758814394, -1.38604395e-09, 0.651306927, 2.85280208e-08, 1, -3.1108879e-08, -0.651306927, 4.21863646e-08, 0.758814394)
            CFrameMon = CFrame.new(-2098.07544, 192.611862, -10248.8867, 0.983392298, -9.57031787e-08, 0.181492642, 8.7276355e-08, 1, 5.44169616e-08, -0.181492642, -3.76732068e-08, 0.983392298)
            
            if SelectMonster == "Peanut Scout" then
            else
                Next_Level_X = 2100
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2100 and game.Players.LocalPlayer.Data.Level.Value <= 2124 or SelectMonster == "Peanut President" then
            Ms = "Peanut President"
            NameQuest = "NutsIslandQuest"
            QuestLv = 2
            NameMon = "Peanut President"
            CFrameQ = CFrame.new(-2104.17163, 38.1299706, -10194.418, 0.758814394, -1.38604395e-09, 0.651306927, 2.85280208e-08, 1, -3.1108879e-08, -0.651306927, 4.21863646e-08, 0.758814394)
            CFrameMon = CFrame.new(-1876.95959, 192.610947, -10542.2939, 0.0553516336, -2.83836812e-08, 0.998466909, -6.89634405e-10, 1, 2.84654931e-08, -0.998466909, -2.26418861e-09, 0.0553516336)
            SelectMonster = "Peanut Scout"
            
            if SelectMonster == "Peanut President" then
            else
                Next_Level_X = 2125
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2125 and game.Players.LocalPlayer.Data.Level.Value <= 2149 or SelectMonster == "Ice Cream Chef" then
            Ms = "Ice Cream Chef"
            NameQuest = "IceCreamIslandQuest"
            QuestLv = 1
            NameMon = "Ice Cream Chef"
            CFrameQ = CFrame.new(-820.404358, 65.8453293, -10965.5654, 0.822534859, 5.24448502e-08, -0.568714678, -2.08336317e-08, 1, 6.20846663e-08, 0.568714678, -3.92184099e-08, 0.822534859)
            CFrameMon = CFrame.new(-821.614075, 208.39537, -10990.7617, -0.870096624, 3.18909272e-08, 0.492881238, -1.8357893e-08, 1, -9.71107568e-08, -0.492881238, -9.35439957e-08, -0.870096624)
            
            if SelectMonster == "Ice Cream Chef" then
            else
                Next_Level_X = 2150
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2150 and game.Players.LocalPlayer.Data.Level.Value <= 2199 or SelectMonster == "Ice Cream Commander" then 
            Ms = "Ice Cream Commander"
            NameQuest = "IceCreamIslandQuest"
            QuestLv = 2
            NameMon = "Ice Cream Commander"
            CFrameQ = CFrame.new(-819.376526, 67.4634171, -10967.2832)
            CFrameMon = CFrame.new(-610.11669921875, 208.26904296875, -11253.686523438)
            
            if SelectMonster == "Ice Cream Commander" then
            else
                Next_Level_X = 2200
            end
            if game.Players.LocalPlayer.Data.Level.Value >= 2175 then
                SelectBoss_P = "Cake Queen"
            end
            SelectMonster = "Ice Cream Chef"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2200 and game.Players.LocalPlayer.Data.Level.Value <= 2224 or SelectMonster == "Cookie Crafter" then 
            Ms = "Cookie Crafter"
            NameQuest = "CakeQuest1"
            QuestLv = 1
            NameMon = "Cookie Crafter"
            CFrameQ = CFrame.new(-2020.6068115234375, 37.82400894165039, -12027.80859375)
            CFrameMon = CFrame.new(-2286.684326171875, 146.5656280517578, -12226.8818359375)
            
            if SelectMonster == "Cookie Crafter" then
            elseif not LevelMax then
                Next_Level_X = 2225
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2225 and game.Players.LocalPlayer.Data.Level.Value <= 2249 or SelectMonster == "Cake Guard" then 
            Ms = "Cake Guard"
            NameQuest = "CakeQuest1"
            QuestLv = 2
            NameMon = "Cake Guard"
            CFrameQ = CFrame.new(-2020.6068115234375, 37.82400894165039, -12027.80859375)
            CFrameMon = CFrame.new(-1817.9747314453125, 209.5632781982422, -12288.9228515625)
            SelectMonster = "Cookie Crafter"
            
            if SelectMonster == "Cake Guard" then
            elseif not LevelMax then
                Next_Level_X = 2250
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2250 and game.Players.LocalPlayer.Data.Level.Value < 2300 or SelectMonster == "Baking Staff" then 
            Ms = "Baking Staff"
            NameQuest = "CakeQuest2"
            QuestLv = 1
            NameMon = "Baking Staff"
            CFrameQ = CFrame.new(-1928.31763, 37.7296638, -12840.626)
            CFrameMon = CFrame.new(-1818.347900390625, 93.41275787353516, -12887.66015625)
            
            if SelectMonster == "Baking Staff" then
            elseif not LevelMax then
                Next_Level_X = 2300
            end
            
            SelectMonster = "Cookie Crafter"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2300 and game.Players.LocalPlayer.Data.Level.Value < 2325 or SelectMonster == "Cocoa Warrior" then 
            Ms = "Cocoa Warrior"
            NameQuest = "ChocQuest1"
            QuestLv = 1
            NameMon = "Cocoa Warrior"
            CFrameQ = CFrame.new(230.19186401367188, 24.7342586517334, -12202.6572265625)
            CFrameMon = CFrame.new(24.617475509643555, 24.734342575073242, -12227.267578125)
            if SelectMonster == "Cocoa Warrior" then
            else
                Next_Level_X = 2325
            end
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2325 and game.Players.LocalPlayer.Data.Level.Value < 2350 or SelectMonster == "Chocolate Bar Battler" then 
            Ms = "Chocolate Bar Battler"
            NameQuest = "ChocQuest1"
            QuestLv = 2
            NameMon = "Chocolate Bar Battler"
            CFrameQ = CFrame.new(230.19186401367188, 24.7342586517334, -12202.6572265625)
            CFrameMon = CFrame.new(658.2230224609375, 24.7342586517334, -12541.9912109375)
            if SelectMonster == "Chocolate Bar Battler" then
            else
                Next_Level_X = 2350
            end
            SelectMonster = "Cocoa Warrior"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2350 and game.Players.LocalPlayer.Data.Level.Value < 2375 or SelectMonster == "Sweet Thief" then 
            Ms = "Sweet Thief"
            NameQuest = "ChocQuest2"
            QuestLv = 1
            NameMon = "Sweet Thief"
            CFrameQ = CFrame.new(149.1439208984375, 24.7938289642334, -12775.41015625)
            CFrameMon = CFrame.new(51.61184310913086, 24.79380989074707, -12574.873046875)
            if SelectMonster == "Sweet Thief" then
            else
                Next_Level_X = 2375
            end
            SelectMonster = "Chocolate Bar Battler"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2375 and game.Players.LocalPlayer.Data.Level.Value < 2400 or SelectMonster == "Candy Rebel" then 
            Ms = "Candy Rebel" 
            NameQuest = "ChocQuest2"
            QuestLv = 2
            NameMon = "Candy Rebel"
            CFrameQ = CFrame.new(149.1439208984375, 24.7938289642334, -12775.41015625)
            CFrameMon = CFrame.new(28.345605850219727, 24.79380226135254, -12949.5029296875)
            if SelectMonster == "Candy Rebel" then
            else
                Next_Level_X = 2400
            end
            SelectMonster = "Sweet Thief"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2400 and game.Players.LocalPlayer.Data.Level.Value < 2425 or SelectMonster == "Candy Pirate"  then
            Ms = "Candy Pirate" 
            NameQuest = "CandyQuest1"
            QuestLv = 1
            NameMon = "Candy Pirate"
            CFrameQ = CFrame.new(-1146.80810546875, 16.107254028320312, -14444.353515625)
            CFrameMon = CFrame.new(-1333.9425048828125, 16.907636642456055, -14424.8447265625)
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2425 and game.Players.LocalPlayer.Data.Level.Value < 2550 or SelectMonster == "Snow Demon" then
            Ms = "Snow Demon"
            NameQuest = "CandyQuest1"
            QuestLv = 2
            NameMon = "Snow Demon"
            CFrameQ = CFrame.new(-1146.80810546875, 16.107254028320312, -14444.353515625)
            CFrameMon = CFrame.new(-963.0213012695312, 16.1071834564209, -14289.576171875)
            if SelectMonster == "Candy Pirate" then
            else
                Next_Level_X = 2551
            end
            SelectMonster = "Candy Pirate"
        elseif game.Players.LocalPlayer.Data.Level.Value >= 2550 then
            Ms = "Baking Staff"
            NameQuest = "CakeQuest2"
            QuestLv = 1
            NameMon = "Baking Staff"
            CFrameQ = CFrame.new(-1928.31763, 37.7296638, -12840.626)
            CFrameMon = CFrame.new(-1818.347900390625, 93.41275787353516, -12887.66015625)
            
            SelectMonster = "Cookie Crafter"
            local Lp = tostring(string.match(tostring(game.ReplicatedStorage.Remotes.CommF_:InvokeServer("CakePrinceSpawner")), "%d+"))
            if Lp == 'nil' or Lp == nil then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner",true)
                Cake_Prince_S:Set(' Cake Prince : Boss Spawn')
            else
                Cake_Prince_S:Set(' Cake Prince : '..Lp)
            end
        end
    end
end
function GetSkill_C(NameW,Skill)
    for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Main.Skills:GetChildren()) do
        if v.Name == NameW then
            if v:FindFirstChild(Skill) and tostring(v[Skill].Title.TextColor) == 'Institutional white' and v[Skill].Cooldown.AbsoluteSize.X == 0 then
                return true
            end
        end
    end
    return false
end
	function GetSkill_C(NameW,Skill)
		for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Main.Skills:GetChildren()) do
			if v.Name == NameW then
				if v:FindFirstChild(Skill) and tostring(v[Skill].Title.TextColor) == 'Institutional white' and v[Skill].Cooldown.AbsoluteSize.X == 0 then
					return true
				end
			end
		end
		return false
	end
  function Hop()
    local PlaceID = game.PlaceId
    local AllIDs = {}
    local foundAnything = ""
    local actualHour = os.date("!*t").hour
    local Deleted = false
    function TPReturner()
        local Site;
        if foundAnything == "" then
            Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
        else
            Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
        end
        local ID = ""
        if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
            foundAnything = Site.nextPageCursor
        end
        local num = 0;
        for i,v in pairs(Site.data) do
            local Possible = true
            ID = tostring(v.id)
            if tonumber(v.maxPlayers) > tonumber(v.playing) then
                for _,Existing in pairs(AllIDs) do
                    if num ~= 0 then
                        if ID == tostring(Existing) then
                            Possible = false
                        end
                    else
                        if tonumber(actualHour) ~= tonumber(Existing) then
                            local delFile = pcall(function()
                                AllIDs = {}
                                table.insert(AllIDs, actualHour)
                            end)
                        end
                    end
                    num = num + 1
                end
                if Possible == true then
                    table.insert(AllIDs, ID)
                    wait()
                    pcall(function()
                        wait()
                        game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
                    end)
                    wait(1)
                end
            end
        end
    end
    function Teleport() 
        while task.wait() do
            pcall(function()
                TPReturner()
                if foundAnything ~= "" then
                    TPReturner()
                end
            end)
        end
    end
    Teleport()
end       
    function fly()
        local mouse=game:GetService("Players").LocalPlayer:GetMouse''
        localplayer=game:GetService("Players").LocalPlayer
        game:GetService("Players").LocalPlayer.Character:WaitForChild("HumanoidRootPart")
        local torso = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
        local speedSET=25
        local keys={a=false,d=false,w=false,s=false}
        local e1
        local e2
        local function start()
            local pos = Instance.new("BodyPosition",torso)
            local gyro = Instance.new("BodyGyro",torso)
            pos.Name="EPIXPOS"
            pos.maxForce = Vector3.new(math.huge, math.huge, math.huge)
            pos.position = torso.Position
            gyro.maxTorque = Vector3.new(9e9, 9e9, 9e9)
            gyro.CFrame = torso.CFrame
            repeat
                    wait()
                    localplayer.Character.Humanoid.PlatformStand=true
                    local new=gyro.CFrame - gyro.CFrame.p + pos.position
                    if not keys.w and not keys.s and not keys.a and not keys.d then
                    speed=1
                    end
                    if keys.w then
                    new = new + workspace.CurrentCamera.CoordinateFrame.lookVector * speed
                    speed=speed+speedSET
                    end
                    if keys.s then
                    new = new - workspace.CurrentCamera.CoordinateFrame.lookVector * speed
                    speed=speed+speedSET
                    end
                    if keys.d then
                    new = new * CFrame.new(speed,0,0)
                    speed=speed+speedSET
                    end
                    if keys.a then
                    new = new * CFrame.new(-speed,0,0)
                    speed=speed+speedSET
                    end
                    if speed>speedSET then
                    speed=speedSET
                    end
                    pos.position=new.p
                    if keys.w then
                    gyro.CFrame = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(-math.rad(speed*15),0,0)
                    elseif keys.s then
                    gyro.CFrame = workspace.CurrentCamera.CoordinateFrame*CFrame.Angles(math.rad(speed*15),0,0)
                    else
                    gyro.CFrame = workspace.CurrentCamera.CoordinateFrame
                    end
            until not Fly
            if gyro then 
                    gyro:Destroy() 
            end
            if pos then 
                    pos:Destroy() 
            end
            flying=false
            localplayer.Character.Humanoid.PlatformStand=false
            speed=0
        end
        e1=mouse.KeyDown:connect(function(key)
            if not torso or not torso.Parent then 
                    flying=false e1:disconnect() e2:disconnect() return 
            end
            if key=="w" then
                keys.w=true
            elseif key=="s" then
                keys.s=true
            elseif key=="a" then
                keys.a=true
            elseif key=="d" then
                keys.d=true
            end
        end)
        e2=mouse.KeyUp:connect(function(key)
            if key=="w" then
                keys.w=false
            elseif key=="s" then
                keys.s=false
            elseif key=="a" then
                keys.a=false
            elseif key=="d" then
                keys.d=false
            end
        end)
        start()
    end    
function UpdateIslandESP() 
    for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
        pcall(function()
            if IslandESP then 
                if v.Name ~= "Sea" then
                    if not v:FindFirstChild('NameEsp') then
                        local bill = Instance.new('BillboardGui',v)
                        bill.Name = 'NameEsp'
                        bill.ExtentsOffset = Vector3.new(0, 1, 0)
                        bill.Size = UDim2.new(1,200,1,30)
                        bill.Adornee = v
                        bill.AlwaysOnTop = true
                        local name = Instance.new('TextLabel',bill)
                        name.Font = "GothamBold"
                        name.FontSize = "Size14"
                        name.TextWrapped = true
                        name.Size = UDim2.new(1,0,1,0)
                        name.TextYAlignment = 'Top'
                        name.BackgroundTransparency = 1
                        name.TextStrokeTransparency = 0.5
                        name.TextColor3 = Color3.fromRGB(7, 236, 240)
                    else
                        v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                    end
                end
            else
                if v:FindFirstChild('NameEsp') then
                    v:FindFirstChild('NameEsp'):Destroy()
                end
            end
        end)
    end
end

function isnil(thing)
return (thing == nil)
end
local function round(n)
return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
for i,v in pairs(game:GetService'Players':GetChildren()) do
    pcall(function()
        if not isnil(v.Character) then
            if ESPPlayer then
                if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v.Character.Head)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v.Character.Head
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' Distance')
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    if v.Team == game.Players.LocalPlayer.Team then
                        name.TextColor3 = Color3.new(0,255,0)
                    else
                        name.TextColor3 = Color3.new(255,0,0)
                    end
                else
                    v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' Distance\nHealth : ' .. round(v.Character.Humanoid.Health*100/v.Character.Humanoid.MaxHealth) .. '%')
                end
            else
                if v.Character.Head:FindFirstChild('NameEsp'..Number) then
                    v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end
    end)
end
end
function UpdateChestChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if string.find(v.Name,"Chest") then
            if ChestESP then
                if string.find(v.Name,"Chest") then
                    if not v:FindFirstChild('NameEsp'..Number) then
                        local bill = Instance.new('BillboardGui',v)
                        bill.Name = 'NameEsp'..Number
                        bill.ExtentsOffset = Vector3.new(0, 1, 0)
                        bill.Size = UDim2.new(1,200,1,30)
                        bill.Adornee = v
                        bill.AlwaysOnTop = true
                        local name = Instance.new('TextLabel',bill)
                        name.Font = Enum.Font.GothamSemibold
                        name.FontSize = "Size14"
                        name.TextWrapped = true
                        name.Size = UDim2.new(1,0,1,0)
                        name.TextYAlignment = 'Top'
                        name.BackgroundTransparency = 1
                        name.TextStrokeTransparency = 0.5
                        if v.Name == "Chest1" then
                            name.TextColor3 = Color3.fromRGB(109, 109, 109)
                            name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                        if v.Name == "Chest2" then
                            name.TextColor3 = Color3.fromRGB(173, 158, 21)
                            name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                        if v.Name == "Chest3" then
                            name.TextColor3 = Color3.fromRGB(85, 255, 255)
                            name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                    else
                        v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                    end
                end
            else
                if v:FindFirstChild('NameEsp'..Number) then
                    v:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end
    end)
end
end
function UpdateDevilChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if DevilFruitESP then
            if string.find(v.Name, "Fruit") then   
                if not v.Handle:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v.Handle)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v.Handle
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(255, 255, 255)
                    name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' Distance')
                else
                    v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' Distance')
                end
            end
        else
            if v.Handle:FindFirstChild('NameEsp'..Number) then
                v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
            end
        end
    end)
end
end
function UpdateFlowerChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if v.Name == "Flower2" or v.Name == "Flower1" then
            if FlowerESP then 
                if not v:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(255, 0, 0)
                    if v.Name == "Flower1" then 
                        name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        name.TextColor3 = Color3.fromRGB(0, 0, 255)
                    end
                    if v.Name == "Flower2" then
                        name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        name.TextColor3 = Color3.fromRGB(255, 0, 0)
                    end
                else
                    v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                end
            else
                if v:FindFirstChild('NameEsp'..Number) then
                v:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end   
    end)
end
end

function UpdateIslandESP() 
    for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
        pcall(function()
            if IslandESP then 
                if v.Name ~= "Sea" then
                    if not v:FindFirstChild('NameEsp') then
                        local bill = Instance.new('BillboardGui',v)
                        bill.Name = 'NameEsp'
                        bill.ExtentsOffset = Vector3.new(0, 1, 0)
                        bill.Size = UDim2.new(1,200,1,30)
                        bill.Adornee = v
                        bill.AlwaysOnTop = true
                        local name = Instance.new('TextLabel',bill)
                        name.Font = "GothamBold"
                        name.FontSize = "Size14"
                        name.TextWrapped = true
                        name.Size = UDim2.new(1,0,1,0)
                        name.TextYAlignment = 'Top'
                        name.BackgroundTransparency = 1
                        name.TextStrokeTransparency = 0.5
                        name.TextColor3 = Color3.fromRGB(7, 236, 240)
                    else
                        v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                    end
                end
            else
                if v:FindFirstChild('NameEsp') then
                    v:FindFirstChild('NameEsp'):Destroy()
                end
            end
        end)
    end
end

function isnil(thing)
return (thing == nil)
end
local function round(n)
return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)
function UpdatePlayerChams()
for i,v in pairs(game:GetService'Players':GetChildren()) do
    pcall(function()
        if not isnil(v.Character) then
            if ESPPlayer then
                if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v.Character.Head)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v.Character.Head
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' Distance')
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    if v.Team == game.Players.LocalPlayer.Team then
                        name.TextColor3 = Color3.new(0,255,0)
                    else
                        name.TextColor3 = Color3.new(255,0,0)
                    end
                else
                    v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' Distance\nHealth : ' .. round(v.Character.Humanoid.Health*100/v.Character.Humanoid.MaxHealth) .. '%')
                end
            else
                if v.Character.Head:FindFirstChild('NameEsp'..Number) then
                    v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end
    end)
end
end
function UpdateChestChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if string.find(v.Name,"Chest") then
            if ChestESP then
                if string.find(v.Name,"Chest") then
                    if not v:FindFirstChild('NameEsp'..Number) then
                        local bill = Instance.new('BillboardGui',v)
                        bill.Name = 'NameEsp'..Number
                        bill.ExtentsOffset = Vector3.new(0, 1, 0)
                        bill.Size = UDim2.new(1,200,1,30)
                        bill.Adornee = v
                        bill.AlwaysOnTop = true
                        local name = Instance.new('TextLabel',bill)
                        name.Font = Enum.Font.GothamSemibold
                        name.FontSize = "Size14"
                        name.TextWrapped = true
                        name.Size = UDim2.new(1,0,1,0)
                        name.TextYAlignment = 'Top'
                        name.BackgroundTransparency = 1
                        name.TextStrokeTransparency = 0.5
                        if v.Name == "Chest1" then
                            name.TextColor3 = Color3.fromRGB(109, 109, 109)
                            name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                        if v.Name == "Chest2" then
                            name.TextColor3 = Color3.fromRGB(173, 158, 21)
                            name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                        if v.Name == "Chest3" then
                            name.TextColor3 = Color3.fromRGB(85, 255, 255)
                            name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        end
                    else
                        v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                    end
                end
            else
                if v:FindFirstChild('NameEsp'..Number) then
                    v:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end
    end)
end
end
function UpdateDevilChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if DevilFruitESP then
            if string.find(v.Name, "Fruit") then   
                if not v.Handle:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v.Handle)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v.Handle
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(255, 255, 255)
                    name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' Distance')
                else
                    v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' Distance')
                end
            end
        else
            if v.Handle:FindFirstChild('NameEsp'..Number) then
                v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
            end
        end
    end)
end
end
function UpdateFlowerChams() 
for i,v in pairs(game.Workspace:GetChildren()) do
    pcall(function()
        if v.Name == "Flower2" or v.Name == "Flower1" then
            if FlowerESP then 
                if not v:FindFirstChild('NameEsp'..Number) then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'..Number
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = Enum.Font.GothamSemibold
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(255, 0, 0)
                    if v.Name == "Flower1" then 
                        name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        name.TextColor3 = Color3.fromRGB(0, 0, 255)
                    end
                    if v.Name == "Flower2" then
                        name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                        name.TextColor3 = Color3.fromRGB(255, 0, 0)
                    end
                else
                    v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' Distance')
                end
            else
                if v:FindFirstChild('NameEsp'..Number) then
                v:FindFirstChild('NameEsp'..Number):Destroy()
                end
            end
        end   
    end)
end
end

function isnil(thing)
return (thing == nil)
end
local function round(n)
return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)

function UpdateIslandMirageESP() 
for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"].Locations:GetChildren()) do
    pcall(function()
        if MirageIslandESP then 
            if v.Name == "Mirage Island" then
                if not v:FindFirstChild('NameEsp') then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = "Code"
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(80, 245, 245)
                else
                    v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                end
            end
        else
            if v:FindFirstChild('NameEsp') then
                v:FindFirstChild('NameEsp'):Destroy()
            end
        end
    end)
end
end

function isnil(thing)
return (thing == nil)
end
local function round(n)
return math.floor(tonumber(n) + 0.5)
end
Number = math.random(1, 1000000)

function UpdateAfdESP() 
for i,v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
    pcall(function()
        if AfdESP then 
            if v.Name == "Advanced Fruit Dealer" then
                if not v:FindFirstChild('NameEsp') then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = "Code"
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(80, 245, 245)
                else
                    v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                end
            end
        else
            if v:FindFirstChild('NameEsp') then
                v:FindFirstChild('NameEsp'):Destroy()
            end
        end
    end)
end
end

function UpdateAuraESP() 
for i,v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
    pcall(function()
        if AuraESP then 
            if v.Name == "Master of Enhancement" then
                if not v:FindFirstChild('NameEsp') then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = "Code"
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(80, 245, 245)
                else
                    v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                end
            end
        else
            if v:FindFirstChild('NameEsp') then
                v:FindFirstChild('NameEsp'):Destroy()
            end
        end
    end)
end
end

function UpdateLSDESP() 
for i,v in pairs(game:GetService("Workspace").NPCs:GetChildren()) do
    pcall(function()
        if LADESP then 
            if v.Name == "Legendary Sword Dealer" then
                if not v:FindFirstChild('NameEsp') then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = "Code"
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(80, 245, 245)
                else
                    v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                end
            end
        else
            if v:FindFirstChild('NameEsp') then
                v:FindFirstChild('NameEsp'):Destroy()
            end
        end
    end)
end
end

function UpdateGeaESP() 
for i,v in pairs(game:GetService("Workspace").Map.MysticIsland:GetChildren()) do 
    pcall(function()
        if GearESP then 
            if v.Name == "MeshPart" then
                if not v:FindFirstChild('NameEsp') then
                    local bill = Instance.new('BillboardGui',v)
                    bill.Name = 'NameEsp'
                    bill.ExtentsOffset = Vector3.new(0, 1, 0)
                    bill.Size = UDim2.new(1,200,1,30)
                    bill.Adornee = v
                    bill.AlwaysOnTop = true
                    local name = Instance.new('TextLabel',bill)
                    name.Font = "Code"
                    name.FontSize = "Size14"
                    name.TextWrapped = true
                    name.Size = UDim2.new(1,0,1,0)
                    name.TextYAlignment = 'Top'
                    name.BackgroundTransparency = 1
                    name.TextStrokeTransparency = 0.5
                    name.TextColor3 = Color3.fromRGB(80, 245, 245)
                else
                    v['NameEsp'].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                end
            end
        else
            if v:FindFirstChild('NameEsp') then
                v:FindFirstChild('NameEsp'):Destroy()
            end
        end
    end)
end
end

function AutoHaki()
local player = game:GetService("Players").LocalPlayer
if not player.Character:FindFirstChild("HasBuso") then
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Buso")
end
end

function UnEquip_Weapon_Farm_All(Weapon)
    local character = game.Players.LocalPlayer.Character
    if character:FindFirstChild(Weapon) then
        character:FindFirstChild(Weapon).Parent = game.Players.LocalPlayer.Backpack
    end
end

function Equip_Weapon_Farm_All(ToolSe)
if not game.Players.LocalPlayer.Character:FindFirstChild(ToolSe) then
if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
Tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
game.Players.LocalPlayer.Character.Humanoid:EquipTool(Tool)
end
end
end 
    
getgenv().ToTargets = function(p)
spawn(function()
pcall(function()
if game:GetService("Players").LocalPlayer:DistanceFromCharacter(p.Position) <= 250 then 
game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = p
elseif not game.Players.LocalPlayer.Character:FindFirstChild("Root")then 
local K = Instance.new("Part",game.Players.LocalPlayer.Character)
K.Size = Vector3.new(1,0.5,1)
K.Name = "Root"
K.Anchored = true
K.Transparency = 1
K.CanCollide = false
K.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
end
local U = (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-p.Position).Magnitude
local z = game:service("TweenService")
local B = TweenInfo.new((p.Position-game.Players.LocalPlayer.Character.Root.Position).Magnitude/300,Enum.EasingStyle.Linear)
local R,t = pcall(function()
local q = z:Create(game.Players.LocalPlayer.Character.Root,B,{CFrame = p})
q:Play()
end)
if not R then 
return t
end
game.Players.LocalPlayer.Character.Root.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
if R and game.Players.LocalPlayer.Character:FindFirstChild("Root") then 
pcall(function()
if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-p.Position).Magnitude >= 20 then 
spawn(function()
pcall(function()
if (game.Players.LocalPlayer.Character.Root.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 150 then 
game.Players.LocalPlayer.Character.Root.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
else 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame=game.Players.LocalPlayer.Character.Root.CFrame
end
end)
end)
elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-p.Position).Magnitude >= 10 and(game.Players.LocalPlayer.Character.HumanoidRootPart.Position-p.Position).Magnitude < 20 then 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position-p.Position).Magnitude < 10 then 
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
end
end)
end
end)
end)
end
    
    
spawn(function()
game:GetService("RunService").Heartbeat:Connect(function()
if _G.AutoFarmFruitMastery or _G.AutoGoNextIsland or _G.AutoObservationv2 or _G.AutoElitehunter or _G.AutoEvoRaceV2 or _G.AutoNevaSoulGuitar or _G.TeleportIsland or _G.AutoGoRaid or _G.AutoOder or _G.AutoGoNextIsland or _G.AutoFarmLevel or _G.AutoSaberSword or _G.AutoFarmBone or _G.AutoFarmDought or _G.AutoKillDoughtKing or _G.AutoFarmBossHallow or _G.AutoDragonTrident or _G.AutoPoleV1 or _G.AutoSharkSword or _G.AutoWardenSword or _G.AutoRengokuSword or _G.AutoDoflamingo or _G.AutoFarmBossHallowHop or _G.AutoSecondSea or _G.AutoThirdSea or _G.AutoDarkDagger or _G.AutoMusketeerHat or _G.AutoFarmDonSwan or _G.AutoCore or _G.AutoGreybeard or _G.Auto_Wing or _G.Umm or _G.Makori_gay or _G.FactoryStaff or _G.AutoObservation or _G.ScrapMetal or _G.Leather then
if not game:GetService("Workspace"):FindFirstChild("LOL") then
local Part = Instance.new("Part")
Part.Name = "LOL"
Part.Parent = game.Workspace
Part.Anchored = true
Part.Transparency = 1
Part.Size = Vector3.new(30,-0.5,30)
elseif game:GetService("Workspace"):FindFirstChild("LOL") then
game.Workspace["LOL"].CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0, -3.6, 0)
end
else
if game:GetService("Workspace"):FindFirstChild("LOL") then
game:GetService("Workspace"):FindFirstChild("LOL"):Destroy()
end
end
end)
end)

spawn(function()
pcall(function()
while task.wait() do
local player = game.Players.LocalPlayer
if _G.AutoFarmFruitMastery or _G.AutoGoNextIsland or _G.AutoObservationv2 or _G.AutoElitehunter or _G.AutoEvoRaceV2 or _G.AutoNevaSoulGuitar or _G.TeleportIsland or _G.AutoGoRaid or _G.AutoOder or _G.AutoGoNextIsland or _G.AutoFarmLevel or _G.AutoSaberSword or _G.AutoFarmBone or _G.AutoFarmDought or _G.AutoKillDoughtKing or _G.AutoFarmBossHallow or _G.AutoDragonTrident or _G.AutoPoleV1 or _G.AutoSharkSword or _G.AutoWardenSword or _G.AutoRengokuSword or _G.AutoDoflamingo or _G.AutoFarmBossHallowHop or _G.AutoSecondSea or _G.AutoThirdSea or _G.AutoDarkDagger or _G.AutoMusketeerHat or _G.AutoFarmDonSwan or _G.AutoCore or _G.AutoGreybeard or _G.Auto_Wing or _G.Umm or _G.Makori_gay or _G.FactoryStaff or _G.AutoObservation or _G.ScrapMetal or _G.Leather == true then
if not player.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
local BodyClip = Instance.new("BodyVelocity")
BodyClip.Name = "BodyClip"
BodyClip.Parent = player.Character.HumanoidRootPart
BodyClip.MaxForce = Vector3.new(100000, 100000, 100000)
BodyClip.Velocity = Vector3.new(0, 0, 0)
end
end
end
end)
end)

spawn(function()
pcall(function()
game:GetService("RunService").Stepped:Connect(function()
if _G.AutoFarmFruitMastery or _G.AutoGoNextIsland or _G.AutoObservationv2 or _G.AutoElitehunter or _G.AutoEvoRaceV2 or _G.AutoNevaSoulGuitar or _G.TeleportIsland or _G.AutoGoRaid or _G.AutoOder or _G.AutoGoNextIsland or _G.AutoFarmLevel or _G.AutoSaberSword or _G.AutoFarmBone or _G.AutoFarmDought or _G.AutoKillDoughtKing or _G.AutoFarmBossHallow or _G.AutoDragonTrident or _G.AutoPoleV1 or _G.AutoSharkSword or _G.AutoWardenSword or _G.AutoRengokuSword or _G.AutoDoflamingo or _G.AutoFarmBossHallowHop or _G.AutoSecondSea or _G.AutoThirdSea or _G.AutoDarkDagger or _G.AutoMusketeerHat or _G.AutoFarmDonSwan or _G.AutoCore or _G.AutoGreybeard or _G.Auto_Wing or _G.Umm or _G.Makori_gay or _G.FactoryStaff or _G.AutoObservation or _G.ScrapMetal or _G.Leather == true then
local character = game:GetService("Players").LocalPlayer.Character
local descendants = character:GetDescendants()
for _, v in pairs(descendants) do
if v:IsA("BasePart") then
v.CanCollide = false    
end
end
end
end)
end)
end)

spawn(function()
while task.wait() do
if _G.AutoFarmFruitMastery or _G.AutoGoNextIsland or _G.AutoObservationv2 or _G.AutoElitehunter or _G.AutoEvoRaceV2 or _G.AutoNevaSoulGuitar or _G.TeleportIsland or _G.AutoGoRaid or _G.AutoOder or _G.AutoGoNextIsland or _G.AutoFarmLevel or _G.AutoSaberSword or _G.AutoFarmBone or _G.AutoFarmDought or _G.AutoKillDoughtKing or _G.AutoFarmBossHallow or _G.AutoDragonTrident or _G.AutoPoleV1 or _G.AutoSharkSword or _G.AutoWardenSword or _G.AutoRengokuSword or _G.AutoDoflamingo or _G.AutoFarmBossHallowHop or _G.AutoSecondSea or _G.AutoThirdSea or _G.AutoDarkDagger or _G.AutoMusketeerHat or _G.AutoFarmDonSwan or _G.AutoCore or _G.AutoGreybeard or _G.Auto_Wing or _G.Umm or _G.Makori_gay or _G.FactoryStaff or _G.AutoObservation or _G.ScrapMetal or _G.Leather == true then
pcall(function()
game:GetService("ReplicatedStorage").Remotes.CommE:FireServer("Ken",true)
end)
end    
end
end)

function BTP(p)
pcall(function()
if (p.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude >= 1500 and not Auto_Raid and game.Players.LocalPlayer.Character.Humanoid.Health > 0 then
repeat wait()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
wait(.2)
game.Players.LocalPlayer.Character.Head:Destroy()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = p
until (p.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude < 1500 and game.Players.LocalPlayer.Character.Humanoid.Health > 0
end
end)
end

function Tween(K1)
    local player = game.Players.LocalPlayer
    local char = player.Character or player.CharacterAdded:Wait()
    local humanoid = char:WaitForChild("Humanoid")    
    if humanoid.Sit then 
        humanoid.Sit = false
    end
    local root = char:WaitForChild("HumanoidRootPart")
    root.CanCollide = false
    local dist = (K1.Position - root.Position).Magnitude
    local spd = 330
    local TweenSvc = game:GetService("TweenService")
    local TweenInf = TweenInfo.new(dist / spd, Enum.EasingStyle.Linear)
    local tween = TweenSvc:Create(root, TweenInf, {CFrame = K1})
    tween:Play()
    tween.Completed:Connect(function()
        root.CanCollide = true 
    end)
    while tween.PlaybackState == Enum.PlaybackState.Playing do
        wait(0.03) 
        if _G.StopTween then
            tween:Cancel()
            root.CanCollide = true 
            break
        end
    end
end

function StopTween(target)
    if not target then
        _G.StopTween = true
        wait()
        Tween(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
        wait()
        if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
            game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip"):Destroy()
        end
        _G.StopTween = false
        _G.Clip = false
        if game.Players.LocalPlayer.Character:FindFirstChild('Highlight') then
            game.Players.LocalPlayer.Character:FindFirstChild('Highlight'):Destroy()
        end
    end
end

function TPB(CFgo)
local Tween_s = game:service"TweenService"
local info = TweenInfo.new((game:GetService("Workspace").Boats.PirateBrigade.VehicleSeat.CFrame.Position - CFgo.Position).Magnitude/450, Enum.EasingStyle.Linear)
Tween = Tween_s:Create(game:GetService("Workspace").Boats.PirateBrigade.VehicleSeat, info, {CFrame = CFgo})
Tween:Play()
local Tweenfunc = {}
function Tweenfunc:Stop()
    Tween:Cancel()
end
return Tweenfunc
end

function TPP(CFgo)
if game.Players.LocalPlayer.Character:WaitForChild("Humanoid").Health <= 0 or not game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid") then Tween:Cancel() repeat wait() until game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid") and game:GetService("Players").LocalPlayer.Character:WaitForChild("Humanoid").Health > 0 wait(7) return end
local Tween_s = game:service"TweenService"
local info = TweenInfo.new((game:GetService("Players")["LocalPlayer"].Character.HumanoidRootPart.Position - CFgo.Position).Magnitude/600, Enum.EasingStyle.Linear)
Tween = Tween_s:Create(game.Players.LocalPlayer.Character["HumanoidRootPart"], info, {CFrame = CFgo})
Tween:Play()
local Tweenfunc = {}
function Tweenfunc:Stop()
    Tween:Cancel()
end
return Tweenfunc
end

StartPos = 1
spawn(function()
while task.wait(.1) do
if StartPos == 1 then
  randomPos = CFrame.new(0,PosY,-65)
  
elseif StartPos == 2 then
  randomPos = CFrame.new(65,PosY,0)

elseif StartPos == 3 then
  randomPos = CFrame.new(0,-65,0)
  
elseif StartPos == 4 then
  randomPos = CFrame.new(0,PosY,65)	
  
elseif StartPos == 5 then
  randomPos = CFrame.new(-65,-PosY,0)
end
end
end)

spawn(function()
while task.wait(.1) do
   StartPos = 1
    wait(.2)
   StartPos = 2
    wait(.3)
   StartPos = 3
    wait(.3)
   StartPos = 4
    wait(.3)
   StartPos = 5
    wait(.3)
end
end)

local K="CurvedRing"
local I="SlashHit"
local R="SwordSlash"
local T="SlashTail"
local O="Sounds"

spawn(function()
    while task.wait() do
        for _,y in pairs(game:GetService("Workspace")["_WorldOrigin"]:GetChildren()) do
            pcall(function()
                if y.Name==K or y.Name==I or y.Name==R or y.Name==T or y.Name==O then
                    y:Destroy()
                end
            end)
        end
    end
end)

if game:GetService("ReplicatedStorage").Effect.Container:FindFirstChild("Death") then
    local Kiritos=game:GetService("ReplicatedStorage").Effect.Container.Death
    Kiritos:Destroy()
end

if game:GetService("ReplicatedStorage").Effect.Container:FindFirstChild("Respawn") then
    local Pro=game:GetService("ReplicatedStorage").Effect.Container.Respawn
    Pro:Destroy()
end

function EquipToolSword()
	pcall(function()
		for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
			if v.ToolTip == "Sword" and v:IsA('Tool') then
				local ToolHumanoid = game.Players.LocalPlayer.Backpack:FindFirstChild(v.Name) 
				game.Players.LocalPlayer.Character.Humanoid:EquipTool(ToolHumanoid) 
			end
		end
	end)
end
function EquipAllTool()
	pcall(function()
		for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
			if v:IsA('Tool') and not (v.Name == "Summon Sea Beast" or v.Name == "Water Body" or v.Name == "Awakening") then
				local ToolHumanoid = game.Players.LocalPlayer.Backpack:FindFirstChild(v.Name) 
				game.Players.LocalPlayer.Character.Humanoid:EquipTool(ToolHumanoid) 
                wait(1)
			end
		end
	end)
end

spawn(function()
	while task.wait() do 
		pcall(function()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(game.Players.LocalPlayer.Character.X.Position, game.Players.LocalPlayer.Character.HumanoidRootPart.Position) 
			if (game.Players.LocalPlayer.Character.X.Position-game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude >= 1 then
				game.Players.LocalPlayer.Character.X.CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.Position, game.Players.LocalPlayer.Character.X.Position)
			end
		end)
	end
end)
    
    spawn(function()
        pcall(function()
            while task.wait() do
                for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do  
                    if v:IsA("Tool") then
                        if v:FindFirstChild("RemoteFunctionShoot") then 
                            SelectWeaponGun = v.Name
                        end
                    end
                end
            end
        end)
    end)
    game:GetService("Players").LocalPlayer.Idled:connect(function()
        game:GetService("VirtualUser"):Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
        wait(1)
        game:GetService("VirtualUser"):Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
    end)
_G.BringMonster = true
_G.BringMode = 320
spawn(function()
    while task.wait() do       
        if _G.BringMonster then
            pcall(function()
                CheckLevel()
                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    if _G.AutoFarmLevel and BringFarmLevel and v.Name == Monster and (Mon == "Factory Staff" or Mon == "Monkey" or Mon == "Dragon Crew Warrior" or Mon == "Dragon Crew Archer") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 275 then
                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                        v.HumanoidRootPart.CFrame = PosMon
                        v.Humanoid:ChangeState(14)
                        v.HumanoidRootPart.CanCollide = false
                        v.Head.CanCollide = false
                        if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                    elseif _G.AutoFarmLevel and BringFarmLevel and v.Name == Monster and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.BringMode then
                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                        v.HumanoidRootPart.CFrame = PosMon
                        v.Humanoid:ChangeState(14)
                        v.HumanoidRootPart.CanCollide = false
                        v.Head.CanCollide = false
                        if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        pcall(function()
            if _G.BringMonster then
                CheckLevel()
                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    if _G.AutoFarmLevel and BringFarmLevel and v.Name == Monster and (Mon == "Factory Staff" or Mon == "Monkey" or Mon == "Dragon Crew Warrior" or Mon == "Dragon Crew Archer") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 275 then
                        v.HumanoidRootPart.Size = Vector3.new(150,150,150)
                        v.HumanoidRootPart.CFrame = PosMon
                        v.Humanoid:ChangeState(14)
                        v.HumanoidRootPart.CanCollide = false
                        v.Head.CanCollide = false
                        if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                    elseif _G.AutoFarmLevel and BringFarmLevel and v.Name == Monster and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.BringMode then
                        v.HumanoidRootPart.Size = Vector3.new(150,150,150)
                        v.HumanoidRootPart.CFrame = PosMon
                        v.Humanoid:ChangeState(14)
                        v.HumanoidRootPart.CanCollide = false
                        v.Head.CanCollide = false
                        if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                        end
                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                    end
                    if _G.AutoEctoplasm and StartEctoplasmMagnet then
                        if string.find(v.Name, "Ship") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - EctoplasmMon.Position).Magnitude <= _G.BringMode then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.HumanoidRootPart.CFrame = EctoplasmMon
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoRengoku and StartRengokuMagnet then
                        if (v.Name == "Snow Lurker" or v.Name == "Arctic Warrior") and (v.HumanoidRootPart.Position - RengokuMon.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(1500,1500,1500)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = RengokuMon
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoMusketeerHat and StartMagnetMusketeerhat then
                        if v.Name == "Forest Pirate" and (v.HumanoidRootPart.Position - MusketeerHatMon.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = MusketeerHatMon
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoObservationv2 and Mangnetcitzenmon then
                        if v.Name == "Forest Pirate" and (v.HumanoidRootPart.Position - MusketeerHatMon.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = PosHee
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoEvoRaceV2 and StartEvoMagnet then
                        if v.Name == "Zombie" and (v.HumanoidRootPart.Position - PosMonEvo.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = PosMonEvo
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoBartilo and AutoBartiloBring then
                        if v.Name == "Swan Pirate" and (v.HumanoidRootPart.Position - PosMonBarto.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = PosMonBarto
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoFarmFruitMastery and StartMasteryFruitMagnet then
                        if v.Name == "Monkey" then
                            if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                v.Humanoid:ChangeState(14)
                                v.HumanoidRootPart.CanCollide = false
                                v.Head.CanCollide = false
                                v.HumanoidRootPart.CFrame = PosMonMasteryFruit
                                if v.Humanoid:FindFirstChild("Animator") then
                                    v.Humanoid.Animator:Destroy()
                                end
                                sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                            end
                        elseif v.Name == "Factory Staff" then
                            if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                v.Humanoid:ChangeState(14)
                                v.HumanoidRootPart.CanCollide = false
                                v.Head.CanCollide = false
                                v.HumanoidRootPart.CFrame = PosMonMasteryFruit
                                if v.Humanoid:FindFirstChild("Animator") then
                                    v.Humanoid.Animator:Destroy()
                                end
                                sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                            end
                        elseif v.Name == Monster then
                            if (v.HumanoidRootPart.Position - PosMonMasteryFruit.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                v.Humanoid:ChangeState(14)
                                v.HumanoidRootPart.CanCollide = false
                                v.Head.CanCollide = false
                                v.HumanoidRootPart.CFrame = PosMonMasteryFruit
                                if v.Humanoid:FindFirstChild("Animator") then
                                    v.Humanoid.Animator:Destroy()
                                end
                                sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                            end
                        end
                    end
                    if _G.AutoFarmBone and BringBones then
                        if (v.Name == "Reborn Skeleton" or v.Name == "Living Zombie" or v.Name == "Demonic Soul" or v.Name == "Posessed Mummy") and (v.HumanoidRootPart.Position - PosMonBone.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = PosMonBone
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoFarmCandy and StartCandyMagnet then
                        if (v.Name == "Ice Cream Chef" or v.Name == "Ice Cream Commander") and (v.HumanoidRootPart.Position - CandyMon.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = CandyMon
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                    if _G.AutoFarmDought and BringDought then
                        if (v.Name == "Cookie Crafter" or v.Name == "Cake Guard" or v.Name == "Baking Staff" or v.Name == "Head Baker") and (v.HumanoidRootPart.Position - PosMonDoughtOpenDoor.Position).Magnitude <= _G.BringMode and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CFrame = PosMonDoughtOpenDoor
                            if v.Humanoid:FindFirstChild("Animator") then
                                v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer, "SimulationRadius", math.huge)
                        end
                    end
                end
            end
        end)
    end
end)
task.spawn(function()
	while true do wait()
		if setscriptable then
			setscriptable(game.Players.LocalPlayer, "SimulationRadius", true)
		end
		if sethiddenproperty then
			sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
		end
	end
end)
task.spawn(function()
	while task.wait() do
		pcall(function()
			if MakoriGayMag and _G.BringMonster then
				for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
					if not string.find(v.Name,"Boss") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.BringMode then
						if InMyNetWork(v.HumanoidRootPart) then
							v.HumanoidRootPart.CFrame = PosGay
							v.Humanoid.JumpPower = 0
							v.Humanoid.WalkSpeed = 0
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							v.Head.CanCollide = false
							if v.Humanoid:FindFirstChild("Animator") then
								v.Humanoid.Animator:Destroy()
							end
							v.Humanoid:ChangeState(11)
							v.Humanoid:ChangeState(14)
						end
					end
				end
			end
		end)
	end
end)
task.spawn(function()
	while task.wait() do
		pcall(function()
			if Min_XT_Is_Kak and _G.BringMonster then
				for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
					if not string.find(v.Name,"Boss") and (v.HumanoidRootPart.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.BringMode then
						if InMyNetWork(v.HumanoidRootPart) then
							v.HumanoidRootPart.CFrame = PosNarathiwat
							v.Humanoid.JumpPower = 0
							v.Humanoid.WalkSpeed = 0
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							v.Head.CanCollide = false
							if v.Humanoid:FindFirstChild("Animator") then
								v.Humanoid.Animator:Destroy()
							end
							v.Humanoid:ChangeState(11)
							v.Humanoid:ChangeState(14)
						end
					end
				end
			end
		end)
	end
end)

function InMyNetWork(object)
	if isnetworkowner then
		return isnetworkowner(object)
	else
		if (object.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= _G.BringMode then 
			return true
		end
		return false
	end
end
local function LockFPS()
  setfpscap(60) -- ล็อค 60 fps
end
LockFPS()
_G.AutoSetSpawn = true
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.AutoSetSpawn then
                if game:GetService("Players").LocalPlayer.Character.Humanoid.Health > 0 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
                end
            end
        end
    end)
end)

local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/SaveManager.lua"))()
local InterfaceManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/InterfaceManager.lua"))()

local TweenService = game:GetService("TweenService")

if game.CoreGui:FindFirstChild("ImageButton") then
    game.CoreGui:FindFirstChild("ImageButton"):Destroy()
end

local ScreenGui = Instance.new("ScreenGui")
local ImageButton = Instance.new("ImageButton")
local UICorner = Instance.new("UICorner")
local ClickSound = Instance.new("Sound")

ScreenGui.Name = "ImageButton"
ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ImageButton.Parent = ScreenGui
ImageButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ImageButton.BorderSizePixel = 0
ImageButton.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
ImageButton.Size = UDim2.new(0, 55, 0, 50)
ImageButton.Draggable = true
ImageButton.Image = "rbxassetid://82059635556284"

UICorner.Parent = ImageButton	

ClickSound.Parent = ImageButton
ClickSound.SoundId = "rbxassetid://130785805"
ClickSound.Volume = 1

local function playClickAnimation()
    local originalSize = ImageButton.Size
    local TweenSizeUp = TweenService:Create(ImageButton, TweenInfo.new(0.1), {Size = UDim2.new(0, 55, 0, 55)})
    local TweenSizeDown = TweenService:Create(ImageButton, TweenInfo.new(0.1), {Size = originalSize})

    TweenSizeUp:Play()
    TweenSizeUp.Completed:Connect(function()
        TweenSizeDown:Play()
    end)
end

ImageButton.MouseButton1Down:Connect(function()
    ClickSound:Play()    
    playClickAnimation()    
    game:GetService("VirtualInputManager"):SendKeyEvent(true, "LeftControl", false, game)
    game:GetService("VirtualInputManager"):SendKeyEvent(false, "LeftControl", false, game)
end)

local Window = Fluent:CreateWindow({
    Title = "Rocket Hub " .. Fluent.Version,
    SubTitle = "Version : Thai & England",
    TabWidth = 100,
    Size = UDim2.fromOffset(480, 380),
    Acrylic = false,
    Theme = "Light",
    MinimizeKey = Enum.KeyCode.LeftControl
})

local Tabs = {
    Main = Window:AddTab({ Title = "General", Icon = "rbxassetid://15712703260" }),
    Sg = Window:AddTab({ Title = "Settings", Icon = "settings" }),
    IQ = Window:AddTab({ Title = "Items & Quest", Icon = "swords" }),
    Stats = Window:AddTab({ Title = "Status Tab", Icon = "chevrons-up" }),
    TP = Window:AddTab({ Title = "Island", Icon = "rbxassetid://15712738876" }),
    ESP = Window:AddTab({ Title = "ESP", Icon = "eye" }),   
    Shop = Window:AddTab({ Title = "Shop", Icon = "rbxassetid://15712767144" }), 
    Misc = Window:AddTab({ Title = "Misc", Icon = "rbxassetid://15712771666" }),
}

local Options = Fluent.Options

do
end

PosY = "35"

local Main = Tabs.Main:AddSection("Credit")
Tabs.Main:AddParagraph({
        Title = "⚡ Credit you Razer Hub"
})
Tabs.Main:AddButton({
    Title = "YouTube : Razer Hub",
    Description = "ช่องยูทูป Razer Hub",
    Callback = function()
    game.StarterGui:SetCore("SendNotification", {
        Title = "คุณ : Razer Hub ✅",
        Text = "Press Follow Channel @Razer Hub",
        Duration = 6
    })
        setclipboard("https://youtube.com/@rocketscript?si=4h1ShiGwW4ECKeMr")
    end
})
Tabs.Main:AddButton({
    Title = "Discord : Razer Hub",
    Description = "ดิสคอร์ด Razer Hub",
    Callback = function()
    game.StarterGui:SetCore("SendNotification", {
        Title = "คุณ : Razer Hub✅",
        Text = "Discord : Razer Hub",
        Icon = "rbxassetid://18888999404",
        Duration = 6
    })
        setclipboard("https://discord.gg/C4K6xGtzpa")
    end
})
local Main = Tabs.Main:AddSection("เมนูหลัก")

local Toggle = Tabs.Main:AddToggle("Auto Farm Level 1-2550 Max", {
    Title = "ออโต้ฟาร์ม เลเวล", 
    Description = "Auto Farm Level 1-2550 Max",
    Default = false,
    Callback = function(Value)
        _G.AutoFarmLevel = Value
        StopTween(_G.AutoFarmLevel)
    end
})
spawn(function()
        while task.wait() do
            if _G.AutoFarmLevel then
                pcall(function()
                    local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
                    if not string.find(QuestTitle, NameMonster) then
                        BringFarmLevel = false
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                    end
                    if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                        BringFarmLevel = false
                        CheckLevel()
                        if BypassTP then
                        if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CFrameQuest.Position).Magnitude > 1500 then
						BTP(CFrameQuest)
						elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CFrameQuest.Position).Magnitude < 1500 then
						Tween(CFrameQuest)
						end
					else
						Tween(CFrameQuest)
					end
					if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CFrameQuest.Position).Magnitude <= 5 then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest, LvQuest)
                        end
                    elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                        CheckLevel()
                        if game:GetService("Workspace").Enemies:FindFirstChild(Monster) then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                                    if v.Name == Monster then
                                        if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMonster) then
                                            repeat task.wait()
                                                Equip_Weapon_Farm_All(_G.SelectWeapon)
                                                AutoHaki()                                            
                                                PosMon = v.HumanoidRootPart.CFrame
                                                Tween(v.HumanoidRootPart.CFrame * CFrame.new(0, 30, 3))
                                                v.HumanoidRootPart.CanCollide = false
                                                v.Humanoid.WalkSpeed = 0
                                                v.Head.CanCollide = false
                                                v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
                                                BringFarmLevel = true
                                            until not _G.AutoFarmLevel or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
                                        else
                                            BringFarmLevel = false
                                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                                        end
                                    end
                                end
                            end
                        else
                            Tween(CFrameMonster * randomPos)
                            UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                            BringFarmLevel = false
                            if game:GetService("ReplicatedStorage"):FindFirstChild(Monster) then
                             Tween(game:GetService("ReplicatedStorage"):FindFirstChild(Monster).HumanoidRootPart.CFrame * randomPos)
                            end
                        end
                    end
                end)
            end
        end
    end)
   

local Toggle = Tabs.Main:AddToggle("Auto Farm Level Fruit Mastery", {
    Title = "ออโต้ฟาร์ม มาสผล + ฟาร์มเวล", 
    Description = "Auto Farm Fruit Mastery + Farm Level",
    Default = false,
    Callback = function(Value)
        _G.AutoFarmFruitMastery = Value
    StopTween(_G.AutoFarmFruitMastery)
    if _G.AutoFarmFruitMastery == false then
        UseSkill = false 
    end
    end
})
spawn(function()
    while task.wait() do
        if _G.AutoFarmFruitMastery then
            pcall(function()
                local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
                if not string.find(QuestTitle, NameMonster) then
                    Magnet = false
                    UseSkill = false
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                end
                if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                    StartMasteryFruitMagnet = false
                    UseSkill = false
                    CheckLevel()
                    repeat wait()
                        Tween(CFrameQuest)
                    until (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.AutoFarmFruitMastery
                    if (CFrameQuest.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5 then
                        wait(0.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest",NameQuest,LvQuest)
                        wait(0.1)
                    end
                elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                    CheckLevel()
                    if game:GetService("Workspace").Enemies:FindFirstChild(Monster) then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                                if v.Name == Monster then
                                    if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMonster) then
                                        HealthMs = v.Humanoid.MaxHealth * _G.Kill_At/100
                                        repeat task.wait()
                                            if v.Humanoid.Health <= HealthMs then
                                                AutoHaki()
                                                Equip_Weapon_Farm_All(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value)
                                                Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
                                                v.HumanoidRootPart.CanCollide = false
                                                PosMonMasteryFruit = v.HumanoidRootPart.CFrame
                                                v.Humanoid.WalkSpeed = 0
                                                v.Head.CanCollide = false
                                                UseSkill = true
                                            else           
                                                UseSkill = false 
                                                AutoHaki()
                                                Equip_Weapon_Farm_All(_G.SelectWeapon)                                              
                                                Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,25,0))
                                                v.HumanoidRootPart.CanCollide = false
                                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                PosMonMasteryFruit = v.HumanoidRootPart.CFrame
                                                v.Humanoid.WalkSpeed = 0
                                                v.Head.CanCollide = false
                                            end
                                            StartMasteryFruitMagnet = true
                                            game:GetService'VirtualUser':CaptureController()
                                            game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
                                        until not _G.AutoFarmFruitMastery or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
                                    else
                                        UseSkill = false
                                        StartMasteryFruitMagnet = false
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                                    end
                                end
                            end
                        end
                    else
                        Tween(CFrameMonster * randomPos)
                        UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                        StartMasteryFruitMagnet = false
                        UseSkill = false
                        if game:GetService("ReplicatedStorage"):FindFirstChild(Monster) then
                            Tween(game:GetService("ReplicatedStorage"):FindFirstChild(Monster).HumanoidRootPart.CFrame * CFrame.new(2,15,4))
                        else
                            if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Y <= 1 then
                                game:GetService("Players").LocalPlayer.Character.Humanoid.Jump = true
                                task.wait()
                                game:GetService("Players").LocalPlayer.Character.Humanoid.Jump = false
                            end
                        end
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while wait() do
        if UseSkill then
            pcall(function()
                CheckLevel()
                for i, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    if v:FindFirstChild("HumanoidRootPart") then
                        local PosMonMasteryFruit = v.HumanoidRootPart
                        if game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                            MasBF = game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
                        elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                            MasBF = game:GetService("Players").LocalPlayer.Backpack[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
                        end
                        if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon-Dragon") then
                            UseSkills({"Z", "X", "C"}, PosMonMasteryFruit.Position)
                        elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom-Venom") then
                            UseSkills({"Z", "X", "C"}, PosMonMasteryFruit.Position)
                        elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha") then
                            if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Size == Vector3.new(2, 2.0199999809265, 1) then
                                UseSkills({"Z", "X", "C", "V"}, PosMonMasteryFruit.Position)
                            end
                        elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                            UseSkills({"Z", "X", "C", "V"}, PosMonMasteryFruit.Position)
                        end
                    end
                end
            end)
        end
    end
end)

function UseSkills(skills, position)
    for _, skill in ipairs(skills) do
        if _G["Skill"..skill] then
            local args = {
                [1] = position
            }
            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
            game:GetService("VirtualInputManager"):SendKeyEvent(true, skill, false, game)
            wait(2)
            game:GetService("VirtualInputManager"):SendKeyEvent(false, skill, false, game)
        end
    end
end

spawn(function()
    game:GetService("RunService").RenderStepped:Connect(function()
        pcall(function()
            if UseSkill then
                for i, v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
                    if v.Name == "NotificationTemplate" then
                        if string.find(v.Text, "Skill locked!") then
                            v:Destroy()
                        end
                    end
                end
            end
        end)
    end)
end)

spawn(function()
    pcall(function()
        game:GetService("RunService").RenderStepped:Connect(function()
            if UseSkill then
                local args = {
                    [1] = PosMonMasteryFruit.Position
                }
                game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
            end
        end)
    end)
end)
spawn(function()
    while task.wait() do
        if UseSkillKub then
            pcall(function()
                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                    if game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                        MasBF = game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
                    elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                        MasBF = game:GetService("Players").LocalPlayer.Backpack[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].Level.Value
                    end
                    if game:GetService("Players").LocalPlayer.Character:FindFirstChild("Dragon-Dragon") then                      
                        if _G.SkillZ then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                        
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
                        end
                        if _G.SkillX then          
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))               
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
                        end
                        if _G.SkillC then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                          
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
                            wait(2)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
                        end
                    elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Venom-Venom") then   
                        if _G.SkillZ then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                        
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
                        end
                        if _G.SkillX then        
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))               
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
                        end
                        if _G.SkillC then 
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                          
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
                            wait(2)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
                        end
                    elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild("Human-Human: Buddha") then
                        if _G.SkillZ and game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Size == Vector3.new(2, 2.0199999809265, 1) then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
                        end
                        if _G.SkillX then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
                        end
                        if _G.SkillC then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
                        end
                        if _G.SkillV then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"V",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"V",false,game)
                        end
                    elseif game:GetService("Players").LocalPlayer.Character:FindFirstChild(game:GetService("Players").LocalPlayer.Data.DevilFruit.Value) then
                        if _G.SkillZ then 
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                         
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"Z",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"Z",false,game)
                        end
                        if _G.SkillX then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"X",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"X",false,game)
                        end
                        if _G.SkillC then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))                           
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"C",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"C",false,game)
                        end
                        if _G.SkillV then
                            local args = {
                                [1] = PosMonMasteryFruit.Position
                            }
                            game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Tool").Name].RemoteEvent:FireServer(unpack(args))
                            game:GetService("VirtualInputManager"):SendKeyEvent(true,"V",false,game)
                            game:GetService("VirtualInputManager"):SendKeyEvent(false,"V",false,game)
                        end
                    end
                end
            end)
        end
    end
end)
spawn(function()
    game:GetService("RunService").RenderStepped:Connect(function()
        pcall(function()
            if UseSkillKub then
                for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.Notifications:GetChildren()) do
                    if v.Name == "NotificationTemplate" then
                        if string.find(v.Text,"Skill locked!") then
                            v:Destroy()
                        end
                    end
                end
            end
        end)
    end)
end)
spawn(function()
    pcall(function()
        game:GetService("RunService").RenderStepped:Connect(function()
            if UseSkillKub then
                local args = {
                    [1] = PosMonMasteryFruit.Position
                }
                game:GetService("Players").LocalPlayer.Character[game:GetService("Players").LocalPlayer.Data.DevilFruit.Value].RemoteEvent:FireServer(unpack(args))
            end
        end)
    end)
end)

local Main = Tabs.Main:AddSection("ทำเควสโลก 2-3")
local Toggle = Tabs.Main:AddToggle("Auto Quest World", {
    Title = "ออโต้ทำ เควสโลก 2 [Lv. 700]", 
    Description = "Auto Second Sea",
    Default = false,
    Callback = function(Value)
        _G.AutoSecondSea = Value
    StopTween(_G.AutoSecondSea)
    end
})
spawn(function()
    while task.wait() do 
        if _G.AutoSecondSea then
            pcall(function()
                local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
                if Lv >= 700 and World1 then
                    if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                        local CFrame1 = CFrame.new(4849.29883, 5.65138149, 719.611877)
                        repeat Tween(CFrame1) wait() until (CFrame1.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                        wait(1.1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("DressrosaQuestProgress","Detective")
                        wait(0.5)
                        Equip_Weapon_Farm_All("Key")
                        repeat Tween(CFrame.new(1347.7124, 37.3751602, -1325.6488)) wait() until (Vector3.new(1347.7124, 37.3751602, -1325.6488)-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                        wait(0.5)
                    else
                        if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                            if game:GetService("Workspace").Enemies:FindFirstChild("Ice Admiral") then
                                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                    if v.Name == "Ice Admiral" then
                                        if not v.Humanoid.Health <= 0 then
                                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                                OldCFrameSecond = v.HumanoidRootPart.CFrame
                                                repeat task.wait()
                                                    AutoHaki()
                                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                                    v.HumanoidRootPart.CanCollide = false
                                                    v.Humanoid.WalkSpeed = 0
                                                    v.Head.CanCollide = false
                                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                    v.HumanoidRootPart.CFrame = OldCFrameSecond
                                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                                    sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                                until not _G.AutoSecondSea or not v.Parent or v.Humanoid.Health <= 0
                                            end
                                        else 
                                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
                                        end
                                    end
                                end
                            else
                                if game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral") then
                                    Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                end
                            end
                        end
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.Main:AddToggle("Auto Quest World", {
    Title = "ออโต้ทำ เควสโลก 3 [Lv. 1500]", 
    Description = "Auto Third Sea",
    Default = false,
    Callback = function(Value)
        _G.AutoThirdSea = Value
    StopTween(_G.AutoThirdSea)
    end
})
spawn(function()
    while task.wait() do
        if _G.AutoThirdSea then
            pcall(function()
                if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1500 and World2 then
                    _G.AutoFarmLevel = false
                    if game:GetService("ReplicatedStorage").Remotes["CommF_"]:InvokeServer("ZQuestProgress", "General") == 0 then
                        Tween(CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016))
                        if (CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
                            wait(1.5)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Begin")
                        end
                        wait(1.8)
                        if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == "rip_indra" then
                                    OldCFrameThird = v.HumanoidRootPart.CFrame
                                    repeat task.wait()
                                        AutoHaki()
                                        Equip_Weapon_Farm_All(_G.SelectWeapon)
                                        Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
                                        v.HumanoidRootPart.CFrame = OldCFrameThird
                                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                        v.HumanoidRootPart.CanCollide = false
                                        v.Humanoid.WalkSpeed = 0
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
                                        sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                    until _G.AutoThirdSea == false or v.Humanoid.Health <= 0 or not v.Parent
                                end
                            end
                        elseif not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra") and (CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
                            Tween(CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016))
                        end
                    end
                end
            end)
        end
    end
end)

local Main = Tabs.Main:AddSection("เค้ก & คาตากุริ [World 3]")
local KilledCheck = Tabs.Main:AddParagraph({
    Title = "Killed : 0 | Defeated : 0",
})

local killedCount = 0
local defeatedCount = 0

spawn(function()
    while task.wait() do
        pcall(function()
            for _, v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                if v.Name == "Cookie Crafter" or v.Name == "Cake Guard" or v.Name == "Baking Staff" or v.Name == "Head Baker" then
                    if v:FindFirstChild("Humanoid") and v.Humanoid.Health <= 0 then
                        killedCount = killedCount + 1
                        v:Destroy()
                    end
                end
            end            
            if killedCount >= 500 then
                killedCount = 0
            end
        end)
    end
end)

spawn(function()
    while task.wait() do
        pcall(function()
            local response = game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")
            local responseLength = string.len(response)
            if responseLength == 88 then
                defeatedCount = tonumber(string.sub(response, 39, 41))
            elseif responseLength == 87 then
                defeatedCount = tonumber(string.sub(response, 39, 40))
            elseif responseLength == 86 then
                defeatedCount = tonumber(string.sub(response, 39, 39))
            else
                defeatedCount = 0
            end
            KilledCheck:SetTitle("You're now Kill : " .. killedCount .. " Defeated : " .. defeatedCount)
        end)
    end
end)

local Toggle = Tabs.Main:AddToggle("Auto Farm Cake Prince", {
    Title = "ออโต้ฟาร์ม เค้ก + คาตากุริ", 
    Description = "Auto Farm Cake Prince",
    Default = false,
    Callback = function(Value)
        _G.AutoFarmDought = Value
        StopTween( _G.AutoFarmDought)
    end
})
spawn(function()
    while task.wait() do
        pcall(function()
            if string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 88 then
                KillMob = (tonumber(string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),39,41)) - 500)
            elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 87 then
                KillMob = (tonumber(string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),40,41)) - 500)
            elseif string.len(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner")) == 86 then
                KillMob = (tonumber(string.sub(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner"),41,41)) - 500)
            end
        end)
    end
end)
spawn(function()
    while task.wait() do
        if _G.AutoFarmDought then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Cake Prince" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                               repeat task.wait()
			                       Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                    sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
                                until not _G.AutoFarmDought or not v.Parent or v.Humanoid.Health <= 0
                            end
                        end
                    end
                else
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    else
                        if KillMob == 0 then
                        end                    
                        if game:GetService("Workspace").Map.CakeLoaf.BigMirror.Other.Transparency == 1 then
                            if game:GetService("Workspace").Enemies:FindFirstChild("Cookie Crafter") or game:GetService("Workspace").Enemies:FindFirstChild("Cake Guard") or game:GetService("Workspace").Enemies:FindFirstChild("Baking Staff") or game:GetService("Workspace").Enemies:FindFirstChild("Head Baker") then
                                for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                    if v.Name == "Cookie Crafter" or v.Name == "Cake Guard" or v.Name == "Baking Staff" or v.Name == "Head Baker" then
                                        if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                            repeat task.wait()
                                                AutoHaki()
                                                Equip_Weapon_Farm_All(_G.SelectWeapon)
                                                v.HumanoidRootPart.CanCollide = false
                                                v.Humanoid.WalkSpeed = 0
                                                v.Head.CanCollide = false 
                                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                BringDought = true
                                                PosMonDoughtOpenDoor = v.HumanoidRootPart.CFrame
                                                Tween(v.HumanoidRootPart.CFrame * CFrame.new(0, 35, 4))
                                            until not _G.AutoFarmDought or not v.Parent or v.Humanoid.Health <= 0 or game:GetService("Workspace").Map.CakeLoaf.BigMirror.Other.Transparency == 0 or game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince [Lv. 2300] [Raid Boss]") or KillMob == 0
                                        end
                                    end
                                end
                            else
                            if BypassTP then
                            if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CakePos.Position).Magnitude > 1500 then
                            BTP(CFrame.new(-2106.864013671875, 139.4144287109375, -12053.1982421875))
                            elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - CakePos.Position).Magnitude < 1500 then
                            Tween(CFrame.new(-2106.864013671875, 139.4144287109375, -12053.1982421875))
                            end
                        else
                            Tween(CFrame.new(-2106.864013671875, 139.4144287109375, -12053.1982421875))
                        end
                                BringDought = false
                                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                                Tween(CFrame.new(-2106.864013671875, 139.4144287109375, -12053.1982421875))
                                if game:GetService("ReplicatedStorage"):FindFirstChild("Cookie Crafter") then
                                    Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Cookie Crafter").HumanoidRootPart.CFrame * CFrame.new(2,20,2)) 
                                else
                                    if game:GetService("ReplicatedStorage"):FindFirstChild("Cake Guard") then
                                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Cake Guard").HumanoidRootPart.CFrame * CFrame.new(2,20,2)) 
                                    else
                                        if game:GetService("ReplicatedStorage"):FindFirstChild("Baking Staff") then
                                            Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Baking Staff").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                                        else
                                            if game:GetService("ReplicatedStorage"):FindFirstChild("Head Baker") then
                                                Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Head Baker").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                                            end
                                        end
                                    end
                                end                       
                            end
                        else
                            if game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince") then
                                Tween(game:GetService("Workspace").Enemies:FindFirstChild("Cake Prince").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                            else
                                if game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince") then
                                    Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Cake Prince").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                                end
                            end
                        end
                    end
                end
            end)
        end
    end
end)   
local Toggle = Tabs.Main:AddToggle("Auto Dought King", {
    Title = "ออโต้ตี คาตากุริ V2", 
    Description = "Auto Dought King",
    Default = false,
    Callback = function(Value)
        _G.AutoKillDoughtKing = Value
        StopTween( _G.AutoKillDoughtKing)
    end
})

spawn(function()
        while task.wait() do
            if  _G.AutoKillDoughtKing and World3 then
                pcall(function()
                    if game:GetService("Workspace").Enemies:FindFirstChild("Dough King") then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if v.Name == "Dough King" then
                                if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                    repeat task.wait()
                                        AutoHaki()
                                        Equip_Weapon_Farm_All(_G.SelectWeapon)
                                        v.HumanoidRootPart.CanCollide = false
                                        v.Humanoid.WalkSpeed = 0
                                        v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                        Tween(v.HumanoidRootPart.CFrame * randomPos)
                                        sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
                                    until not  _G.AutoKillDoughtKing or not v.Parent or v.Humanoid.Health <= 0
                                    _G.AutoKillDoughtKing = false
                                end
                            end
                        end
                    end
                end)
            end
        end
    end)    
local Toggle = Tabs.Main:AddToggle("Auto Cake Prince Spawner", {
    Title = "ออโต้เสก คาตากุริ", 
    Description = "Auto Cake Prince Spawner",
    Default = true,
    Callback = function(Value)
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CakePrinceSpawner",Value)
    end
})
local Main = Tabs.Main:AddSection("กระดูก & โบน [World 3]")
local BoneCheck = Tabs.Main:AddParagraph({
    Title = "You're now having 0 Bones",
    Content = "Auto Farm Bones will auto farm skeleton bones for you."
})
spawn(function()
    while task.wait() do
          pcall(function()
            BoneCheck:SetTitle("You're now having "..(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Check")).. " Bones")
        end)
    end
end)

local Toggle = Tabs.Main:AddToggle("Auto Farm Bone", {
    Title = "ออโต้ฟาร์ม กระดูก & โบน", 
    Description = "Auto Farm Bones",
    Default = false,
    Callback = function(Value)
        _G.AutoFarmBone = Value
        StopTween( _G.AutoFarmBone)
    end
})   
spawn(function()
while task.wait() do
if _G.AutoFarmBone and World3 then
pcall(function()
local enemies = game:GetService("Workspace").Enemies
if enemies:FindFirstChild("Reborn Skeleton") or enemies:FindFirstChild("Living Zombie") or enemies:FindFirstChild("Demonic Soul") or enemies:FindFirstChild("Posessed Mummy") then
for _, MobBone in pairs(enemies:GetChildren()) do
if MobBone.Name == "Reborn Skeleton" or MobBone.Name == "Living Zombie" or MobBone.Name == "Demonic Soul" or MobBone.Name == "Posessed Mummy" then
if MobBone:FindFirstChild("Humanoid") and MobBone:FindFirstChild("HumanoidRootPart") and MobBone.Humanoid.Health > 0 then
repeat 
task.wait()
AutoHaki()
Equip_Weapon_Farm_All(_G.SelectWeapon)
MobBone.HumanoidRootPart.CanCollide = false
MobBone.Humanoid.WalkSpeed = 0
MobBone.Head.CanCollide = false 
BringBones = true
PosMonBone = MobBone.HumanoidRootPart.CFrame                                  
Tween(MobBone.HumanoidRootPart.CFrame * CFrame.new(0, 35, 4))
until not _G.AutoFarmBone or not MobBone.Parent or MobBone.Humanoid.Health <= 0
end
end
end
else
if BypassTP then
local playerPos = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
local targetPos = BonePos.Position                       
if (playerPos - targetPos).Magnitude > 1500 then
BTP(CFrame.new(-9710.945, 204.795, 6041.272))
elseif (playerPos - targetPos).Magnitude < 1500 then
Tween(CFrame.new(-9710.945, 204.795, 6041.272))
end
else
Tween(CFrame.new(-9710.945, 204.795, 6041.272))
end
UnEquip_Weapon_Farm_All(_G.SelectWeapon)
BringBones = false
Tween(CFrame.new(-9710.945, 204.795, 6041.272))
for _, NemeBoneMob in pairs(game:GetService("ReplicatedStorage"):GetChildren()) do
if NemeBoneMob.Name == "Reborn Skeleton" then
Tween(NemeBoneMob.HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
elseif NemeBoneMob.Name == "Living Zombie" then
Tween(NemeBoneMob.HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
elseif NemeBoneMob.Name == "Demonic Soul" then
Tween(NemeBoneMob.HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
elseif NemeBoneMob.Name == "Posessed Mummy" then
Tween(NemeBoneMob.HumanoidRootPart.CFrame * CFrame.new(2, 20, 2))
end
end
end
end)
end
end
end)

local Toggle = Tabs.Main:AddToggle("Auto Random Bone", {
    Title = "ออโต้สุ่ม กระดูก & โบน",
    Description = "Auto Random Bones",
    Default = false,
    Callback = function(Value)
        _G.AutoRandomBone = Value
    end
})    
spawn(function()    
while task.wait(.1) do
if _G.AutoRandomBone then      
pcall(function()
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bones","Buy",1,1)
end)
end
end
end)

local Toggle = Tabs.Main:AddToggle("Auto Pray", {
    Title = "สวดมนต์",
    Description = "Auto Pray",
    Default = false,
    Callback = function(Value)
        _G.AutoPray = Value
    end
})    
spawn(function()
pcall(function()
while task.wait() do
if _G.AutoPray and World3 then    
Tween(CFrame.new(-8652.99707, 143.450119, 6170.50879, -0.983064115, -2.48005533e-10, 0.18326205, -1.78910387e-09, 1, -8.24392288e-09, -0.18326205, -8.43218029e-09, -0.983064115))
wait(.1)
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",1)
end
end
end)
end)

local Toggle = Tabs.Main:AddToggle("Auto Try Luck", {
    Title = "เสี่ยงโชค",
    Description = "Auto Try Luck",
    Default = false,
    Callback = function(Value)
        _G.TryLuck = Value
    end
})    
spawn(function()
pcall(function()
while task.wait() do
if _G.TryLuck and World3  then    
Tween(CFrame.new(-8652.99707, 143.450119, 6170.50879, -0.983064115, -2.48005533e-10, 0.18326205, -1.78910387e-09, 1, -8.24392288e-09, -0.18326205, -8.43218029e-09, -0.983064115))
wait(.1)
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2)
end
end
end)
end)

local Main = Tabs.Main:AddSection("ลงดัน & ลอร์")
_G.SelectChip = _G.SelectChip or ""

local Raidslist = {}

local RaidsModule = require(game:GetService("ReplicatedStorage").Raids)
for _, raid in pairs(RaidsModule.raids) do
    table.insert(Raidslist, raid)
end
for _, advancedRaid in pairs(RaidsModule.advancedRaids) do
    table.insert(Raidslist, advancedRaid)
end


local SelectChip = Tabs.Main:AddDropdown("Select Chip", {
    Title = "เลือกชิปลงดัน",
    Description = "Select Chip",
    Values = Raidslist,
    Multi = false,
    Default = _G.SelectChip,
})

SelectChip:OnChanged(function(Value)
    _G.SelectChip = Value 
end)
Tabs.Main:AddButton({
    Title = "ซื้อซิปที่เลือก",
    Description = "Buy Select Chip",
    Callback = function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc","Select",_G.SelectChip)
    end
})
local Toggle = Tabs.Main:AddToggle("Auto Start Raid", {
    Title = "เริ่มออโต้ลงดัน", 
    Description = "Start Raid [World2, World3]", 
    Default = false,
    Callback = function(Value)
    _G.AutoGoRaid = Value
    end
})
spawn(function()
while task.wait() do
pcall(function()
if _G.AutoGoRaid then
if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game:GetService("Players").LocalPlayer.Character:FindFirstChild("Special Microchip") then
if World2 then
fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
elseif World3 then
fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
end
end
end
end
end)
end
end)
local Toggle = Tabs.Main:AddToggle("Kill Aura", {
    Title = "มอนตายทันที", 
    Description = "Kill Aura", 
    Default = false,
    Callback = function(Value)
    _G.AutoKillAura = Value
    end
})
spawn(function()
pcall(function() 
while task.wait() do
if _G.AutoKillAura then
if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
for i,v in pairs(game:GetService("Workspace").Enemies:GetDescendants()) do
if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
pcall(function()
repeat wait()
sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
v.Humanoid.Health = 0
v.HumanoidRootPart.CanCollide = false
until not _G.AutoKillAura or not v.Parent or v.Humanoid.Health <= 0
end)
end
end
end
end
end
end)
end)

local Toggle = Tabs.Main:AddToggle("Auto Next Island", {
    Title = "ออโต้เกาะต่อไป", 
    Description = "Auto Next Island", 
    Default = false,
    Callback = function(Value)
        _G.AutoGoNextIsland = Value
            StopTween(_G.AutoGoNextIsland)
    end
})

spawn(function()
    pcall(function()
        while task.wait() do
            if _G.AutoGoNextIsland then
                if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == true then
                    if game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
                        Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0, 80, 0))
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
                       Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0, 80, 0))
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
                       Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0, 80, 0))
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
                        Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0, 80, 0))
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                        Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame*CFrame.new(0, 80, 0))
                    end
                end
            end
        end
    end)
end)

if World2 then
local Toggle = Tabs.Main:AddToggle("Auto  Law", {
    Title = "ออโต้ตีบอส ลอร์", 
    Description = "Auto Law Boss", 
    Default = false,
    Callback = function(Value)
  _G.AutoOder = Value
    StopTween( _G.AutoOder)
    end
})
end
spawn(function()
while task.wait() do
if  _G.AutoOder then
pcall(function()
if game:GetService("Workspace").Enemies:FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
if v.Name == "Order [Lv. 1250] [Raid Boss]" then
if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
repeat task.wait()
AutoHaki()
Equip_Weapon_Farm_All(_G.SelectWeapon)
v.HumanoidRootPart.CanCollide = false
v.Humanoid.WalkSpeed = 0
v.HumanoidRootPart.Size = Vector3.new(50,45,45)
Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,25,0))
sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
until not  _G.AutoOder or not v.Parent or v.Humanoid.Health <= 0
end
end
end
else
if game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(0,25,5))
end
end
end)
end
end
end)

if World2 then
Tabs.Main:AddButton({
    Title = "ซื้อชิปลอร์",
    Description = "Buy Law Raid Chip", 
    Callback = function()
        local args = {
        [1] = "BlackbeardReward",
        [2] = "Microchip",
        [3] = "2"
     }
     game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end
})
end

local Main = Tabs.Main:AddSection("🔋กำหนดฆ่ามอนที่เลือด% & Skill🪫")
local Slider = Tabs.Main:AddSlider("Kill Monster", {
        Title = "Kill Monster At ..% Health",
        Description = "ฆ่ามอนสเตอร์ที่ ...% พลังชีวิต",
        Default = 30,
        Min = 0,
        Max = 100,
        Rounding = 0,
        Callback = function(Value)
            _G.Kill_At = Value
        end
    })
_G.Kill_At = 30
local Toggle = Tabs.Main:AddToggle("Auto Skill", {
    Title = "Skill Z", 
    Description = "สกิว Z", 
    Default = true,
    Callback = function(Value)
    _G.SkillZ = Value
    end
})
local Toggle = Tabs.Main:AddToggle("Auto Skill", {
    Title = "Skill X", 
    Description = "สกิว X", 
    Default = true,
    Callback = function(Value)
    _G.SkillX = Value
    end
})
local Toggle = Tabs.Main:AddToggle("Auto Skill", {
    Title = "Skill C", 
    Description = "สกิว C", 
    Default = true,
    Callback = function(Value)
    _G.SkillC = Value
    end
})
local Toggle = Tabs.Main:AddToggle("Auto Skill", {
    Title = "Skill V", 
    Description = "สกิว V", 
    Default = true,
    Callback = function(Value)
    _G.SkillV = Value
    end
})

local Main = Tabs.Sg:AddSection("เมนูตั้งค่าฟาร์ม")
local SelectWeapon = Tabs.Sg:AddDropdown("SelectWeapon", {
    Title = "เลือกอาวุธ",
    Description = "Select Combat/Weapon", 
    Values = {"หมัด","ดาบ","ปืน","ผลปีศาจ"},
    Multi = false,
    Default = 1,
})
SelectWeapon:OnChanged(function(Value)
    _G.SelectWeapon = Value
end)   
spawn(function()
    while task.wait() do
        pcall(function()
            local backpack = game.Players.LocalPlayer.Backpack
            local selectedWeapon = _G.SelectWeapon            
            if selectedWeapon == "หมัด" then
                for i, v in pairs(backpack:GetChildren()) do
                    if v.ToolTip == "Melee" and backpack:FindFirstChild(tostring(v.Name)) then
                        _G.SelectWeapon = v.Name
                    end
                end
            elseif selectedWeapon == "ดาบ" then
                for i, v in pairs(backpack:GetChildren()) do
                    if v.ToolTip == "Sword" and backpack:FindFirstChild(tostring(v.Name)) then
                        _G.SelectWeapon = v.Name
                    end
                end
            elseif selectedWeapon == "ปืน" then
                for i, v in pairs(backpack:GetChildren()) do
                    if v.ToolTip == "Gun" and backpack:FindFirstChild(tostring(v.Name)) then
                        _G.SelectWeapon = v.Name
                    end
                end
            elseif selectedWeapon == "ผลปีศาจ" then
                for i, v in pairs(backpack:GetChildren()) do
                    if v.ToolTip == "Blox Fruit" and backpack:FindFirstChild(tostring(v.Name)) then
                        _G.SelectWeapon = v.Name
                    end
                end
            end
        end)
    end
end)

local SelectFast = Tabs.Sg:AddDropdown("SelectWeapon", {
    Title = "เลือกความเร็ว Fast Attack",
    Description = "Select Fast Attack", 
    Values = {"Noob Fast","Normal Fast","Super Fast"},
    Multi = false,
    Default = 2,
})
SelectFast:OnChanged(function(Value)
    _G.FastAttackType = Value
end)   

local Toggle = Tabs.Sg:AddToggle("Haki", {
    Title = "ออโต้เปิดฮาคิ", 
    Description = "Auto Haki", 
    Default = true,
    Callback = function(Value)
        _G.AUTOHAKI = Value
    end
})
spawn(function()
	while task.wait() do
		if _G.AUTOHAKI then 
			if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
				local args = {
					[1] = "Buso"
				}
				game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
			end
		end
	end
end)
local Toggle = Tabs.Sg:AddToggle("Auto Hide Notification", {
    Title = "ปิดการแจ้งเตือน",
    Description = "Disable Notifications", 
    Default = true,
    Callback = function(Value)
        _G.HideNotificationExp = Value
    end
})
spawn(function()
	while task.wait() do
	   pcall(function()
		if _G.HideNotificationExp then
			game.Players.LocalPlayer.PlayerGui.Notifications.Enabled = false
		else
			game.Players.LocalPlayer.PlayerGui.Notifications.Enabled = true
			end
		end)
	end
end)
local Toggle = Tabs.Sg:AddToggle("Auto Codes", {
    Title = "สุ่มโค้ค Exp2", 
    Description = "Redeem Codes", 
    Default = true,
    Callback = function(Value)
        _G.AutoRedeemCode = Value
    end
})    
spawn(function()
	while task.wait() do
		if _G.AutoRedeemCode then
	function UseCode(Text)
				game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
			end
        UseCode("Enyo_is_Pro")
        UseCode("Magicbus")
        UseCode("JCWK")
        UseCode("Starcodeheo")
        UseCode("Bluxxy")
        UseCode("fudd10_v2")
        UseCode("3BVISITS")
        UseCode("UPD16")
        UseCode("FUDD10")
        UseCode("BIGNEWS")
        UseCode("Sub2OfficialNoobie")
        UseCode("SUB2GAMERROBOT_EXP1")
        UseCode("StrawHatMaine")
        UseCode("SUB2NOOBMASTER123")
        UseCode("Sub2Daigrock")
        UseCode("Axiore")
        UseCode("TantaiGaming")
        UseCode("STRAWHATMAINE")
        UseCode("kittgaming")
        UseCode("Magicbus")
        UseCode("JCWK")
        UseCode("Starcodeheo")
        UseCode("Bluxxy")
        UseCode("fudd10_v2")
        UseCode("Enyu_is_Pro")
        UseCode("Sub2Fer999")
        UseCode("THEGREATACE")
        UseCode("SUB2GAMERROBOT_EXP1")
        UseCode("Sub2OfficialNoobie")
        UseCode("StrawHatMaine")
        UseCode("SUB2NOOBMASTER123")
        UseCode("Sub2Daigrock")
        UseCode("Axiore")
        UseCode("TantaiGaming")
        UseCode("STRAWHATMAINE")
        UseCode("JCWK")
        UseCode("Sub2Fer999")
        UseCode("Magicbus")
        UseCode("Starcodeheo")
        UseCode("Bluxxy")
        UseCode("Sub2Fer999")
        UseCode("GAMERROBOT_YT")
            end
        end
    end)
Tabs.Sg:AddButton({
    Title = "ภาพกากสำหรับมือถือแล็ค",
    Description = "FPS Booster",
    Callback = function()
        FPSBooster()
    end
})
function FPSBooster()
        local decalsyeeted = true
        local g = game
        local w = g.Workspace
        local l = g.Lighting
        local t = w.Terrain
        sethiddenproperty(l, "Technology", 2)
        sethiddenproperty(t, "Decoration", false)
        t.WaterWaveSize = 0
        t.WaterWaveSpeed = 0
        t.WaterReflectance = 0
        t.WaterTransparency = 0
        l.GlobalShadows = false
        l.FogEnd = 9e9
        l.Brightness = 0
        settings().Rendering.QualityLevel = "Level01"
        for i, v in pairs(g:GetDescendants()) do
            if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
                v.Material = "Plastic"
                v.Reflectance = 0
            elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
                v.Transparency = 1
            elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
                v.Lifetime = NumberRange.new(0)
            elseif v:IsA("Explosion") then
                v.BlastPressure = 1
                v.BlastRadius = 1
            elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
                v.Enabled = false
            elseif v:IsA("MeshPart") then
                v.Material = "Plastic"
                v.Reflectance = 0
                v.TextureID = 10385902758728957
            end
        end
        for i, e in pairs(l:GetChildren()) do
            if
                e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or
                    e:IsA("DepthOfFieldEffect")
             then
                e.Enabled = false
            end
        end
    end
local Toggle = Tabs.Sg:AddToggle("Black Screen", {
    Title = "หน้าจอสีดำ",
    Description = "Black Screen", 
    Default = _G.BlackScreen,
    Callback = function(Value)
        _G.BlackScreen = Value
    end
})
spawn(function()
    while task.wait() do
        if _G.BlackScreen then
                game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(500, 0, 500, 500)
        else
                game:GetService("Players").LocalPlayer.PlayerGui.Main.Blackscreen.Size = UDim2.new(1, 0, 500, 500)
        end
    end
end)
local Toggle = Tabs.Sg:AddToggle("White Screen", {
    Title = "หน้าจอสีขาว",
    Description = "White Screen", 
    Default = _G.WhiteScreen,
    Callback = function(Value)
        _G.WhiteScreen = Value
    end
})
spawn(function()
   while task.wait() do
      if _G.WhiteScreen then
         pcall(function()
            game:GetService("RunService"):Set3dRenderingEnabled(false)
         end)
      else
         pcall(function()
            game:GetService("RunService"):Set3dRenderingEnabled(true)
         end)
      end
   end
end)

local Main = Tabs.IQ:AddSection("เมนูดาบต่างๆ")
local Toggle = Tabs.IQ:AddToggle("Auto Swords", {
    Title = "ออโต้ทำดาบ เวเดน", 
    Description = "Auto Warden [Sword]",
    Default = false,
    Callback = function(Value)
        _G.AutoWardenSword = Value
        StopTween( _G.AutoWardenSword)
    end
})
spawn(function()
while task.wait() do
if  _G.AutoWardenSword and World1 then
pcall(function()
if game:GetService("Workspace").Enemies:FindFirstChild("Chief Warden") then
for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
if v.Name == "Chief Warden" then
if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
repeat task.wait()
AutoHaki()
Equip_Weapon_Farm_All(_G.SelectWeapon)
v.HumanoidRootPart.CanCollide = false
v.Humanoid.WalkSpeed = 0
v.HumanoidRootPart.Size = Vector3.new(50,50,50)
Tween(v.HumanoidRootPart.CFrame * randomPos)
sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
until not  _G.AutoWardenSword or not v.Parent or v.Humanoid.Health <= 0
_G.AutoWardenSword = false
end
end
end
else
if BypassTP then
if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude > 1500 then
BTP(CFrame.new(5240.02392578125, 95.66567993164062, 743.1629028320312))
elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude < 1500 then
Tween(CFrame.new(5240.02392578125, 95.66567993164062, 743.1629028320312))
end
else
Tween(CFrame.new(5240.02392578125, 95.66567993164062, 743.1629028320312))
end
UnEquip_Weapon_Farm_All(_G.SelectWeapon)
Tween(CFrame.new(5240.02392578125, 95.66567993164062, 743.1629028320312))
if game:GetService("ReplicatedStorage"):FindFirstChild("Chief Warden") then
Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Chief Warden").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
end
end
end)
end
end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Swords", {
    Title = "ออโต้ทำดาบ ฉลาม", 
    Description = "Auto Shark [Sword]",
    Default = false,
    Callback = function(Value)
        _G.AutoSharkSword = Value
        StopTween( _G.AutoSharkSword)
    end
})
spawn(function()
    while task.wait() do
      if  _G.AutoSharkSword and World1 then
         pcall(function()
           if game:GetService("Workspace").Enemies:FindFirstChild("The Saw") then
              for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
              if v.Name == "The Saw" then
             if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                      repeat task.wait()
                      AutoHaki()
                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
               v.Humanoid.WalkSpeed = 0
                      v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                              Tween(v.HumanoidRootPart.CFrame * randomPos)
                 sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
                      until not  _G.AutoSharkSword or not v.Parent or v.Humanoid.Health <= 0
                                _G.AutoSharkSword = false
                 end
                        end
          end
                else
         if BypassTP then
              if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude > 1500 then
                BTP(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
        elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude < 1500 then
                Tween(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
        end
            else
        Tween(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
           end
     UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
           if game:GetService("ReplicatedStorage"):FindFirstChild("The Saw") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("The Saw").HumanoidRootPart.CFrame * CFrame.new(2,40,2))
                    end
                end
            end)
        end
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Swords", {
    Title = "ออโต้ทำดาบ แชงค์คูส", 
    Description = "Auto Saber [Sword]",
    Default = false,
    Callback = function(Value)
        _G.AutoSaberSword = Value
        StopTween( _G.AutoSaberSword)
    end
})
spawn(function()
    while task.wait() do
        if _G.AutoSaberSword and game.Players.LocalPlayer.Data.Level.Value >= 200 and World1 then
            pcall(function()
                if game:GetService("Workspace").Map.Jungle.Final.Part.Transparency == 0 then
                    if game:GetService("Workspace").Map.Jungle.QuestPlates.Door.Transparency == 0 then
                        if (CFrame.new(-1612.55884, 36.9774132, 148.719543, 0.37091279, 3.0717151e-09, -0.928667724, 3.97099491e-08, 1, 1.91679348e-08, 0.928667724, -4.39869794e-08, 0.37091279).Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 100 then
                            Tween(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame)
                            wait(1)
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate1.Button.CFrame
                            wait(2)
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate2.Button.CFrame
                            wait(2)
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate3.Button.CFrame
                            wait(2)
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate4.Button.CFrame
                            wait(2)
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace").Map.Jungle.QuestPlates.Plate5.Button.CFrame
                            wait(2)
                        else
                            Tween(CFrame.new(-1612.55884, 36.9774132, 148.719543, 0.37091279, 3.0717151e-09, -0.928667724, 3.97099491e-08, 1, 1.91679348e-08, 0.928667724, -4.39869794e-08, 0.37091279))
                        end
                    else
                        if game:GetService("Workspace").Map.Desert.Burn.Part.Transparency == 0 then
                            if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Torch") or game.Players.LocalPlayer.Character:FindFirstChild("Torch") then
                                Equip_Weapon_Farm_All("Torch")
                                Tween(CFrame.new(1114.61475, 5.04679728, 4350.22803, -0.648466587, -1.28799094e-09, 0.761243105, -5.70652914e-10, 1, 1.20584542e-09, -0.761243105, 3.47544882e-10, -0.648466587))
                              else
                              Tween(CFrame.new(-1610.00757, 11.5049858, 164.001587, 0.984807551, -0.167722285, -0.0449818149, 0.17364943, 0.951244235, 0.254912198, 3.42372805e-05, -0.258850515, 0.965917408))
                            end
                        else
                            if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","SickMan") ~= 0 then
                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","GetCup")
                                wait(0.5)
                                Equip_Weapon_Farm_All("Cup")
                                wait(0.5)
                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","FillCup",game:GetService("Players").LocalPlayer.Character.Cup)
                                wait(0)
                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","SickMan")
                            else
                                if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon") == nil then
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon")
                                elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon") == 0 then
                                if game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader") or game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader") then
                                    Tween(CFrame.new(-2883.5400390625, 7.562280178070068, 5441.826171875)) 
                                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                            if v.Name == "Mob Leader" then
                                               if game:GetService("Workspace").Enemies:FindFirstChild("Mob Leader") then
                                                if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                                    repeat task.wait()                                                                                                       
                                                    AutoHaki()
                                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                                    v.HumanoidRootPart.CanCollide = false
                                                    v.Humanoid.WalkSpeed = 0
                                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)                             
                                                    Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,10,0))
                                                    sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                                    until v.Humanoid.Health <= 0 or not _G.AutoSaberSword
                                                 end
                                            end
                                            if game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader") then
                                                Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Mob Leader").HumanoidRootPart.CFrame * CFrame.new(0,7,2))
                                            end
                                        end
                                    end
                                 end
                                elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon") == 1 then
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","RichSon")
                                    wait(0.5)
                                    Equip_Weapon_Farm_All("Relic")
                                    wait(0.5)
                                    Tween(CFrame.new(-1404.91504, 29.9773273, 3.80598116, 0.876514494, 5.66906877e-09, 0.481375456, 2.53851997e-08, 1, -5.79995607e-08, -0.481375456, 6.30572643e-08, 0.876514494))
                                end
                            end
                        end
                    end
                else
                    if game:GetService("Workspace").Enemies:FindFirstChild("Saber Expert") or game:GetService("ReplicatedStorage"):FindFirstChild("Saber Expert") then
                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                if v.Name == "Saber Expert" then
                                    repeat task.wait()                                                                           
                                        Equip_Weapon_Farm_All(_G.SelectWeapon)
                                        Tween(v.HumanoidRootPart.CFrame * randomPos)
                                        v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
                                        v.HumanoidRootPart.Transparency = 1
                                        v.Humanoid.JumpPower = 0
                                        v.Humanoid.WalkSpeed = 0
                                        v.HumanoidRootPart.CanCollide = false                                     
                                        FarmPos = v.HumanoidRootPart.CFrame
                                        MonFarm = v.Name
                                    until v.Humanoid.Health <= 0 or not _G.AutoSaberSword
                                    if v.Humanoid.Health <= 0 then
                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ProQuestProgress","PlaceRelic")
                                    end
                                end
                            end
                        end
                    end
                end
            end)
        end
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Swords", {
    Title = "ออโต้ทำ โพV1", 
    Description = "Auto Pole V1 [Sword]",
    Default = false,
    Callback = function(Value)
        _G.AutoPoleV1 = Value
        StopTween( _G.AutoPoleV1)
    end
})
spawn(function()
    while task.wait() do
        if  _G.AutoPoleV1 and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Thunder God") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Thunder God" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()                                
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                    sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
                                until not  _G.AutoPoleV1 or not v.Parent or v.Humanoid.Health <= 0
                                _G.AutoPoleV1 = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude > 1500 then
                BTP(CFrame.new(-7619.01220703125, 5618.587890625, -2454.539794921875))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Position).Magnitude < 1500 then
                Tween(CFrame.new(-7619.01220703125, 5618.587890625, -2454.539794921875))
                end
            else
                Tween(CFrame.new(-7619.01220703125, 5618.587890625, -2454.539794921875))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-7619.01220703125, 5618.587890625, -2454.539794921875))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Thunder God").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto  Law", {
    Title = "ออโต้ทำดาบ ลอร์", 
    Description = "Auto Law Boss", 
    Default = false,
    Callback = function(Value)
  _G.AutoOder = Value
    StopTween( _G.AutoOder)
    end
})
spawn(function()
while task.wait() do
if  _G.AutoOder then
pcall(function()
if game:GetService("Workspace").Enemies:FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
if v.Name == "Order [Lv. 1250] [Raid Boss]" then
if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
repeat task.wait()
AutoHaki()
Equip_Weapon_Farm_All(_G.SelectWeapon)
v.HumanoidRootPart.CanCollide = false
v.Humanoid.WalkSpeed = 0
v.HumanoidRootPart.Size = Vector3.new(50,45,45)
Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,25,0))
sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
until not  _G.AutoOder or not v.Parent or v.Humanoid.Health <= 0
end
end
end
else
if game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]") then
Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Order [Lv. 1250] [Raid Boss]").HumanoidRootPart.CFrame * CFrame.new(0,25,5))
end
end
end)
end
end
end)

local Main = Tabs.IQ:AddSection("เมนูทำของต่างๆ")
local Elite = Tabs.IQ:AddParagraph({
    Title = "Status : Not",
})
spawn(function()
    while task.wait() do
        pcall(function()
            if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo") or game:GetService("ReplicatedStorage"):FindFirstChild("Deandre") or game:GetService("ReplicatedStorage"):FindFirstChild("Urban") or game:GetService("Workspace").Enemies:FindFirstChild("Diablo") or game:GetService("Workspace").Enemies:FindFirstChild("Deandre") or game:GetService("Workspace").Enemies:FindFirstChild("Urban") then
                Elite:SetTitle("อีลิทฮันเตอร์ : เกิดแล้ว! ✅")	
            else
                Elite:SetTitle("อีลิทฮันเตอร์ : ยังไม่เกิด ❌")	
            end
        end)
    end
end)

local EliteProgress = Tabs.IQ:AddParagraph({
    Title = "Elite Progress : Not",
})
spawn(function()
    pcall(function()
        while wait() do
            EliteProgress:SetTitle("Elite Progress : "..game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter","Progress"))
        end
    end)
end)

local Toggle = Tabs.IQ:AddToggle("Farm", {
    Title = "ออโต้ตีบอส อีลิทฮันเตอร์", 
    Description = "Auto Elite Hunter + ย้ายเชิร์ฟหา", 
    Default = false,
    Callback = function(Value)
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
    _G.AutoElitehunter = Value
    StopTween(_G.AutoElitehunter)
    end
})
spawn(function()
    while task.wait() do
        if _G.AutoElitehunter and World3 then
            pcall(function()
                local QuestTitle = game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text
                if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                    if BypassTP then
                    if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Elite.Position).Magnitude > 1500 then
                    BTP(CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188))
                    elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - Elite.Position).Magnitude < 1500 then
                    Tween(CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188))
                    end
                else
                    Tween(CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188))
                end
                if (Vector3.new(-5418.892578125, 313.74130249023, -2826.2260742188)-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("EliteHunter")
                    end
                elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                    if string.find(QuestTitle,"Diablo") or string.find(QuestTitle,"Deandre") or string.find(QuestTitle,"Urban") then
                        if game:GetService("Workspace").Enemies:FindFirstChild("Diablo") or game:GetService("Workspace").Enemies:FindFirstChild("Deandre") or game:GetService("Workspace").Enemies:FindFirstChild("Urban") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == "Diablo" or v.Name == "Deandre" or v.Name == "Urban" then
                                    if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                        repeat task.wait()
                                            AutoHaki()
                                            Equip_Weapon_Farm_All(_G.SelectWeapon)
                                            v.HumanoidRootPart.CanCollide = false
                                            v.Humanoid.WalkSpeed = 0
                                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                            Tween(v.HumanoidRootPart.CFrame * randomPos)
                                            game:GetService("VirtualUser"):CaptureController()
                                            game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
                                            sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                        until _G.AutoElitehunter == false or v.Humanoid.Health <= 0 or not v.Parent
                                    end
                                end
                            end
                        else
                            if game:GetService("ReplicatedStorage"):FindFirstChild("Diablo") then
                                Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Diablo").HumanoidRootPart.CFrame * CFrame.new(0,20,5))
                            elseif game:GetService("ReplicatedStorage"):FindFirstChild("Deandre") then
                                Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Deandre").HumanoidRootPart.CFrame * CFrame.new(0,20,5))
                            elseif game:GetService("ReplicatedStorage"):FindFirstChild("Urban") then
                                Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Urban").HumanoidRootPart.CFrame * CFrame.new(0,20,5))
                            else
                                if _G.AutoElitehunter then
                                    Hop()
                                else
                                    Tween(CFrame.new(-5418.892578125, 313.74130249023, -2826.2260742188))
                                end
                            end
                        end                    
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Evo Race V2", {
    Title = "ออโต้อีโว เผ่าV2", 
    Description = "Auto Evo Race V2",
    Default = false,
    Callback = function(Value)
        _G.AutoEvoRaceV2 = Value
        StopTween( _G.AutoEvoRaceV2)
    end
})
spawn(function()
pcall(function()
while task.wait() do
if _G.AutoEvoRaceV2 and World2 then
if not game:GetService("Players").LocalPlayer.Data.Race:FindFirstChild("Evolved") then
if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 0 then
Tween(CFrame.new(-2779.83521, 72.9661407, -3574.02002, -0.730484903, 6.39014104e-08, -0.68292886, 3.59963224e-08, 1, 5.50667032e-08, 0.68292886, 1.56424669e-08, -0.730484903))
if (Vector3.new(-2779.83521, 72.9661407, -3574.02002) - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
wait(.1)
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","2")
end
elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 1 then
pcall(function()
if not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 1") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 1") then
Tween(game:GetService("Workspace").Flower1.CFrame)
elseif not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 2") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 2") then
Tween(game:GetService("Workspace").Flower2.CFrame)
elseif not game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 3") and not game:GetService("Players").LocalPlayer.Character:FindFirstChild("Flower 3") then
if game:GetService("Workspace").Enemies:FindFirstChild("Zombie") then
for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
if v.Name == "Zombie" then
repeat task.wait()
AutoHaki()
Equip_Weapon_Farm_All(_G.SelectWeapon)
Tween(v.HumanoidRootPart.CFrame * CFrame.new(0,25,0))
v.HumanoidRootPart.CanCollide = false
v.HumanoidRootPart.Size = Vector3.new(50,50,50)
PosMonEvo = v.HumanoidRootPart.CFrame
StartEvoMagnet = true
until game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Flower 3") or not v.Parent or v.Humanoid.Health <= 0 or _G.AutoEvoRaceV2 == false
StartEvoMagnet = false
end
end
else
StartEvoMagnet = false
Tween(CFrame.new(-5685.9233398438, 48.480125427246, -853.23724365234))
end
end
end)
elseif game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","1") == 2 then
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Alchemist","3")
end
end
end
end
end)
end)
local Toggle = Tabs.IQ:AddToggle("Auto SoulGuitar", {
    Title = "ออโต้ทำ กีต้าร์บรู๊ค", 
    Description = "Auto Soul Guitar",
    Default = false,
    Callback = function(Value)
        _G.AutoNevaSoulGuitar = Value
        StopTween( _G.AutoNevaSoulGuitar)
    end
})
spawn(function()
    while task.wait() do
        pcall(function()
            if _G.AutoNevaSoulGuitar then
                if GetWeaponInventory("Soul Guitar") == false then
                    if (CFrame.new(-9681.458984375, 6.139880657196045, 6341.3720703125).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 5000 then
                        if game:GetService("Workspace").NPCs:FindFirstChild("Skeleton Machine") then
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("soulGuitarBuy",true)
                        else
                            if game:GetService("Workspace").Map["Haunted Castle"].Candle1.Transparency == 0 then
                                if game:GetService("Workspace").Map["Haunted Castle"].Placard1.Left.Part.Transparency == 0 then
                                    Quest2 = true
                                    repeat wait() Tween(CFrame.new(-8762.69140625, 176.84783935546875, 6171.3076171875)) until (CFrame.new(-8762.69140625, 176.84783935546875, 6171.3076171875).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.AutoNevaSoulGuitar
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard7.Left.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard6.Left.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard5.Left.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard4.Right.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard3.Left.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard2.Right.ClickDetector)
                                    wait(1)
                                    fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"].Placard1.Right.ClickDetector)
                                    wait(1)
                                elseif game:GetService("Workspace").Map["Haunted Castle"].Tablet.Segment1:FindFirstChild("ClickDetector") then
                                    if game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part1:FindFirstChild("ClickDetector") then
                                        Quest4 = true
                                        repeat wait() Tween(CFrame.new(-9553.5986328125, 65.62338256835938, 6041.58837890625)) until (CFrame.new(-9553.5986328125, 65.62338256835938, 6041.58837890625).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or not _G.AutoNevaSoulGuitar
                                        wait(1)
                                        Tween(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part3.CFrame)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part3.ClickDetector)
                                        wait(1)
                                        Tween(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.CFrame)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part4.ClickDetector)
                                        wait(1)
                                        Tween(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.CFrame)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.ClickDetector)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part6.ClickDetector)
                                        wait(1)
                                        Tween(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part8.CFrame)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part8.ClickDetector)
                                        wait(1)
                                        Tween(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.CFrame)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
                                        wait(1)
                                        fireclickdetector(game:GetService("Workspace").Map["Haunted Castle"]["Lab Puzzle"].ColorFloor.Model.Part10.ClickDetector)
                                    else
                                        Quest3 = true
                                    end
                                else
                                    if game:GetService("Workspace").NPCs:FindFirstChild("Ghost") then
                                        local args = {
                                            [1] = "GuitarPuzzleProgress",
                                            [2] = "Ghost"
                                        }

                                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                                    end
                                    if game.Workspace.Enemies:FindFirstChild("Living Zombie") then
                                        for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                                            if v:FindFirstChild("HumanoidRootPart") and v:FindFirstChild("Humanoid") and v.Humanoid.Health > 0 then
                                                if v.Name == "Living Zombie" then
                                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                                    v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                                                    v.HumanoidRootPart.Transparency = 1
                                                    v.Humanoid.JumpPower = 0
                                                    v.Humanoid.WalkSpeed = 0
                                                    v.HumanoidRootPart.CanCollide = false
                                                    v.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,20,0)
                                                    Tween(CFrame.new(-10160.787109375, 138.6616973876953, 5955.03076171875))
                                                end
                                            end
                                        end
                                    else
                                        Tween(CFrame.new(-10160.787109375, 138.6616973876953, 5955.03076171875))
                                    end
                                end
                            else    
                                if string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2), "Error") then
                                    Tween(CFrame.new(-8653.2060546875, 140.98487854003906, 6160.033203125))
                                elseif string.find(game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2), "Nothing") then
                                    print("Yo Wait Next Night!")
                                else
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("gravestoneEvent",2,true)
                                end
                            end
                        end
                    else
                        Tween(CFrame.new(-9681.458984375, 6.139880657196045, 6341.3720703125))
                    end                
                end
            end
        end)
    end
end)

local Main = Tabs.IQ:AddSection("เมนูต่างๆ")
local Toggle = Tabs.IQ:AddToggle("Auto Greybeard", {
    Title = "ออโต้ตีบอส หมวดขาว", 
    Description = "Auto Greybeard [Level. 700]",
    Default = false,
    Callback = function(Value)
        _G.AutoGreybeard = Value
        StopTween( _G.AutoGreybeard)
    end
})
spawn(function()
    while task.wait() do
        if  _G.AutoGreybeard and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Greybeard") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Greybeard" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.HumanoidRootPart.CFrame * CFrame.new(0, 25, 0)
                                    sethiddenproperty(game.Players.LocalPlayer,"SimulationRadius",math.huge)
                                until not  _G.AutoGreybeard or not v.Parent or v.Humanoid.Health <= 0
                                _G.AutoGreybeard = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - GayMakPos.Position).Magnitude > 1500 then
                BTP(CFrame.new(-5023.38330078125, 28.65203285217285, 4332.3818359375))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - GayMakPos.Position).Magnitude < 1500 then
                Tween(CFrame.new(-5023.38330078125, 28.65203285217285, 4332.3818359375))
                end
            else
                Tween(CFrame.new(-5023.38330078125, 28.65203285217285, 4332.3818359375))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-5023.38330078125, 28.65203285217285, 4332.3818359375))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Greybeard") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Greybeard").HumanoidRootPart.CFrame * CFrame.new(0,25,4))                 
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Core", {
    Title = "ออโต้ตี โรงงาน", 
    Description = "Auto Core",
    Default = false,
    Callback = function(Value)
        _G.AutoCore = Value
        StopTween( _G.AutoCore)
    end
})
spawn(function()
    while task.wait() do
       pcall(function()
        if _G.AutoCore and Word2 then
           if game:GetService("Workspace").Enemies:FindFirstChild("Core") then
               for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                 if v.Name == "Core" and v.Humanoid.Health > 0 then
                    repeat task.wait()
                     AutoHaki()         
                     Equip_Weapon_Farm_All(_G.SelectWeapon)           
                     Tween(CFrame.new(448.46756, 199.356781, -441.389252))                                  
                     until v.Humanoid.Health <= 0 or _G.AutoCore == false
                     end
                    end
                else
                    Tween(CFrame.new(448.46756, 199.356781, -441.389252))
                end
            end
        end)
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Don Swan", {
    Title = "ออโต้ตี โดฟามิงโก้", 
    Description = "Auto Don Swan",
    Default = false,
    Callback = function(Value)
        _G.AutoFarmDonSwan = Value
        StopTween( _G.AutoFarmDonSwan)
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.AutoFarmDonSwan and World2 then
                if game:GetService("Workspace").Enemies:FindFirstChild("Don Swan") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Don Swan" and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
                            repeat task.wait()
                                pcall(function()                                
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                    sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                end)
                            until _G.AutoFarmDonSwan == false or v.Humanoid.Health <= 0
                            _G.AutoFarmDonSwan = false
                        end
                    end
                else 
                    repeat task.wait()
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(2284.912109375, 15.537666320801, 905.48291015625)) 
                    until (CFrame.new(2284.912109375, 15.537666320801, 905.48291015625).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 or _G.AutoFarmSwanGlasses == false
                end
            end
        end
    end)
end)

local Toggle = Tabs.IQ:AddToggle("Auto Forest Pirate & Captain Elephant", {
    Title = "ออโต้ตี โจรสลัดบุก", 
    Description = "Auto Forest Pirate & Captain Elephant",
    Default = false,
    Callback = function(Value)
        _G.AutoMusketeerHat = Value
        StopTween( _G.AutoMusketeerHat)
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.AutoMusketeerHat and World3 then
                if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress").KilledBandits == false then
                    if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Forest Pirate") and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "50") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                        if game:GetService("Workspace").Enemies:FindFirstChild("Forest Pirate") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == "Forest Pirate" then
                                    repeat task.wait()
                                        pcall(function()                                        
                                            Equip_Weapon_Farm_All(_G.SelectWeapon)
                                            AutoHaki()
                                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                            Tween(v.HumanoidRootPart.CFrame * randomPos)
                                            v.HumanoidRootPart.CanCollide = false
                                            MusketeerHatMon = v.HumanoidRootPart.CFrame
                                            StartMagnetMusketeerhat = true
                                        end)
                                    until _G.AutoMusketeerHat == false or not v.Parent or v.Humanoid.Health <= 0 or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
                                    StartMagnetMusketeerhat = false
                                    _G.AutoMusketeerHat = false
                                end
                            end
                        else
                            StartMagnetMusketeerhat = false
                            Tween(CFrame.new(-13206.452148438, 425.89199829102, -7964.5537109375))
                        end
                    else
                        Tween(CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125))
                        if (Vector3.new(-12443.8671875, 332.40396118164, -7675.4892578125) - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 30 then
                            wait(1.5)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest","CitizenQuest",1)
                        end
                    end
                elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress").KilledBoss == false then
                    if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible and string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, "Captain Elephant") and game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                        if game:GetService("Workspace").Enemies:FindFirstChild("Captain Elephant") then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == "Captain Elephant" then
                                    OldCFrameElephant = v.HumanoidRootPart.CFrame
                                    repeat task.wait()
                                        pcall(function()
                                            Equip_Weapon_Farm_All(_G.SelectWeapon)
                                            AutoHaki()
                                            v.HumanoidRootPart.CanCollide = false
                                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                            Tween(v.HumanoidRootPart.CFrame * randomPos)
                                            v.HumanoidRootPart.CanCollide = false
                                            v.HumanoidRootPart.CFrame = OldCFrameElephant
                                            sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                        end)
                                    until _G.AutoMusketeerHat == false or v.Humanoid.Health <= 0 or not v.Parent or game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false
                                end
                            end
                        else
                            Tween(CFrame.new(-13374.889648438, 421.27752685547, -8225.208984375))
                        end
                    else
                        Tween(CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125))
                        if (CFrame.new(-12443.8671875, 332.40396118164, -7675.4892578125).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
                            wait(1.5)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen")
                        end
                    end
                elseif game:GetService("Players").LocalPlayer.Data.Level.Value >= 1800 and game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 2 then
                    Tween(CFrame.new(-12512.138671875, 340.39279174805, -9872.8203125))
                end
            end
        end
    end)
end)

local Toggle = Tabs.IQ:AddToggle("Auto Rip_indra", {
    Title = "ออโต้ตี แอดมิน", 
    Description = "Auto rip_indra",
    Default = false,
    Callback = function(Value)
        _G.AutoDarkDagger = Value
        StopTween( _G.AutoDarkDagger)
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.AutoDarkDagger then
                if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra True Form") or game:GetService("Workspace").Enemies:FindFirstChild("rip_indra") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == ("rip_indra True Form" or v.Name == "rip_indra") and v.Humanoid.Health > 0 and v:IsA("Model") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") then
                            repeat task.wait()
                                pcall(function()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                end)
                            until _G.AutoDarkDagger == false or v.Humanoid.Health <= 0
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - AdminPos.Position).Magnitude > 1500 then
                BTP(CFrame.new(-5344.822265625, 423.98541259766, -2725.0930175781))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - AdminPos.Position).Magnitude < 1500 then
                Tween(CFrame.new(-5344.822265625, 423.98541259766, -2725.0930175781))
                end
            else
                Tween(CFrame.new(-5344.822265625, 423.98541259766, -2725.0930175781))
            end
                    UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                    Tween(CFrame.new(-5344.822265625, 423.98541259766, -2725.0930175781))
                end
            end
        end
    end)
end)
spawn(function()
    pcall(function()
        while task.wait() do
            if (_G.AutoDarkDagger_Hop and _G.AutoDarkDagger) and World3 and not game:GetService("ReplicatedStorage"):FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") and not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra True Form [Lv. 5000] [Raid Boss]") then
                Hop()
            end
        end
    end)
end)

local Main = Tabs.IQ:AddSection("เมนูฟาร์มต่างๆ")
local ObservationRange = Tabs.IQ:AddParagraph({
    Title = "Observation Level : Not",
})
spawn(function()
    while task.wait() do
        pcall(function()
            ObservationRange:SetTitle("Observation Level : "..math.floor(game:GetService("Players").LocalPlayer.VisionRadius.Value))
        end)
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Observation", {
    Title = "ออโต้ฟาร์ม ฮาคิสังเกต", 
    Description = "Auto Farm Observation",
    Default = false,
    Callback = function(Value)
        _G.AutoObservation = Value
        StopTween( _G.AutoObservation)
    end
})
spawn(function()
    while task.wait() do
        pcall(function()
            if _G.AutoObservation then
                local player = game:GetService("Players").LocalPlayer
                local character = player.Character or player.CharacterAdded:Wait()
                local humanoidRootPart = character:WaitForChild("HumanoidRootPart")
                
                local enemies = game:GetService("Workspace").Enemies:GetChildren()
                local target = nil
                
                for _, enemy in ipairs(enemies) do
                    if enemy:FindFirstChild("HumanoidRootPart") then
                        local distance = (humanoidRootPart.Position - enemy.HumanoidRootPart.Position).Magnitude
                        if distance <= 400 then
                            target = enemy
                            break
                        end
                    end
                end
                
                if target then
                    local targetPosition = target.HumanoidRootPart.Position
                    local flyPosition = targetPosition + Vector3.new(0, 20, 0) -- ตำแหน่งเหนือศัตรู
                    
                    Tween(CFrame.new(targetPosition))

                    repeat task.wait()
                        if not player.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
                            game:GetService('VirtualUser'):CaptureController()
                            game:GetService('VirtualUser'):SetKeyDown('0x65') -- กด E เพื่อเปิด Haki
                            wait(2)
                            game:GetService('VirtualUser'):SetKeyUp('0x65')
                        end
                    until player.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") or not _G.AutoObservation
                    
                    Tween(CFrame.new(flyPosition))
                end
            end
        end)
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Observation", {
    Title = "ออโต้ทำ ฮาคิสังเกต V2", 
    Description = "Auto Observation V2",
    Default = false,
    Callback = function(Value)
        _G.AutoObservationv2 = Value
        if not _G.AutoObservationv2 then
            StopTween(false)
        end
    end
})
spawn(function()
    while task.wait() do
        if not _G.AutoObservationv2 then return end
        pcall(function()
            if _G.AutoObservationv2 and World3 then
                if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen") == 3 then
                    _G.AutoMusketeerHat = false
                    if game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Banana") and 
                       game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Apple") and 
                       game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Pineapple") then
                        repeat 
                            Tween(CFrame.new(-12444.78515625, 332.40396118164, -7673.1806640625)) 
                            task.wait() 
                        until not _G.AutoObservationv2 or 
                              (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - 
                               Vector3.new(-12444.78515625, 332.40396118164, -7673.1806640625)).Magnitude <= 10
                        task.wait(0.5)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("CitizenQuestProgress","Citizen")
                    elseif game:GetService("Players").LocalPlayer.Backpack:FindFirstChild("Fruit Bowl") or 
                           game:GetService("Players").LocalPlayer.Character:FindFirstChild("Fruit Bowl") then
                        repeat 
                            Tween(CFrame.new(-10920.125, 624.20275878906, -10266.995117188)) 
                            task.wait() 
                        until not _G.AutoObservationv2 or 
                              (game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position - 
                               Vector3.new(-10920.125, 624.20275878906, -10266.995117188)).Magnitude <= 10
                        task.wait(0.5)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk2","Start")
                        task.wait(1)
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk2","Buy")
                    else
                        for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
                            if v.Name == "Apple" or v.Name == "Banana" or v.Name == "Pineapple" then
                                v.Handle.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,1,10)
                                task.wait()
                                firetouchinterest(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart, v.Handle, 0)    
                                task.wait()
                            end
                        end   
                    end
                else
                    _G.AutoMusketeerHat = true
                end
            end
        end)
    end
end)


local Main = Tabs.IQ:AddSection("Valuable")
local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม กัมมันตรังสี", 
    Description = "Auto Farm Radioactive",
    Default = false,
    Callback = function(Value)
        _G.FactoryStaff = Value
        StopTween( _G.FactoryStaff)
    end
})
spawn(function()
    while task.wait() do
        if _G.FactoryStaff and World2 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Factory Staff") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Factory Staff" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.FactoryStaff or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos1.Position).Magnitude > 1500 then
                BTP(CFrame.new(-507.7895202636719, 72.99479675292969, -126.45632934570312))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos1.Position).Magnitude < 1500 then
                Tween(CFrame.new(-507.7895202636719, 72.99479675292969, -126.45632934570312))
                end
            else
                Tween(CFrame.new(-507.7895202636719, 72.99479675292969, -126.45632934570312))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-507.7895202636719, 72.99479675292969, -126.45632934570312))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Factory Staff") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Factory Staff").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม มิสติก ดรอปเล็ต", 
    Description = "Auto Farm Mystic Droplet",
    Default = false,
    Callback = function(Value)
        _G.Makori_gay = Value
        StopTween( _G.Makori_gay)
    end
})
spawn(function()
    while task.wait() do
        if _G.Makori_gay and World2 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Water Fighter") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Water Fighter" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Makori_gay or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos2.Position).Magnitude > 1500 then
                BTP(CFrame.new(-3352.9013671875, 285.01556396484375, -10534.841796875))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos2.Position).Magnitude < 1500 then
                Tween(CFrame.new(-3352.9013671875, 285.01556396484375, -10534.841796875))
                end
            else
                Tween(CFrame.new(-3352.9013671875, 285.01556396484375, -10534.841796875))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-3352.9013671875, 285.01556396484375, -10534.841796875))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Water Fighter") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Water Fighter").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม แร่แม็กม่า", 
    Description = "Auto Farm Mystic Droplet",
    Default = false,
    Callback = function(Value)
        _G.Umm = Value
        StopTween( _G.Umm)
    end
})
spawn(function()
    while task.wait() do
        if _G.Umm and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Military Spy") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Military Spy" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Umm or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos3.Position).Magnitude > 1500 then
                BTP(CFrame.new(-5850.2802734375, 77.28675079345703, 8848.6748046875))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos3.Position).Magnitude < 1500 then
                Tween(CFrame.new(-5850.2802734375, 77.28675079345703, 8848.6748046875))
                end
            else
                Tween(CFrame.new(-5850.2802734375, 77.28675079345703, 8848.6748046875))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-5850.2802734375, 77.28675079345703, 8848.6748046875))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Military Spy") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Military Spy").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        if _G.Umm and World2 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Lava Pirate") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Lava Pirate" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Umm or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos4.Position).Magnitude > 1500 then
                BTP(CFrame.new(-5234.60595703125, 51.953372955322266, -4732.27880859375))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos4.Position).Magnitude < 1500 then
                Tween(CFrame.new(-5234.60595703125, 51.953372955322266, -4732.27880859375))
                end
            else
                Tween(CFrame.new(-5234.60595703125, 51.953372955322266, -4732.27880859375))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-5234.60595703125, 51.953372955322266, -4732.27880859375))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Lava Pirate") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Lava Pirate").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม ปีกนางฟ้า", 
    Description = "Auto Farm Angel Wing",
    Default = false,
    Callback = function(Value)
        _G.Auto_Wing = Value
        StopTween( _G.Auto_Wing)
    end
})
spawn(function()
    while task.wait() do
        if _G.Auto_Wing and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Royal Soldier") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Royal Soldier" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Auto_Wing or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos5.Position).Magnitude > 1500 then
                BTP(CFrame.new(-7827.15625, 5606.912109375, -1705.5833740234375))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos5.Position).Magnitude < 1500 then
                Tween(CFrame.new(-7827.15625, 5606.912109375, -1705.5833740234375))
                end
            else
                Tween(CFrame.new(-7827.15625, 5606.912109375, -1705.5833740234375))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-7827.15625, 5606.912109375, -1705.5833740234375))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Royal Soldier") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Royal Soldier").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม หนัง", 
    Description = "Auto Farm Leather",
    Default = false,
    Callback = function(Value)
        _G.Leather = Value
        StopTween( _G.Leather)
    end
})
spawn(function()
    while task.wait() do
        if _G.Leather and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Pirate") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Pirate" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Leather or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos6.Position).Magnitude > 1500 then
                BTP(CFrame.new(-1211.8792724609375, 4.787090301513672, 3916.83056640625))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos6.Position).Magnitude < 1500 then
              Tween(CFrame.new(-1211.8792724609375, 4.787090301513672, 3916.83056640625))
                end
            else
                Tween(CFrame.new(-1211.8792724609375, 4.787090301513672, 3916.83056640625))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-1211.8792724609375, 4.787090301513672, 3916.83056640625))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Pirate") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Pirate").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        if _G.Leather and World2 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Marine Captain") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Marine Captain" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Leather or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos7.Position).Magnitude > 1500 then
                BTP(CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos7.Position).Magnitude < 1500 then
                Tween(CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375))
                end
            else
                Tween(CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-2010.5059814453125, 73.00115966796875, -3326.620849609375))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Marine Captain") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Marine Captain").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        if _G.Leather and World3 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Jungle Pirate") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Jungle Pirate" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.Leather or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos8.Position).Magnitude > 1500 then
                BTP(CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos8.Position).Magnitude < 1500 then
                Tween(CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375))
                end
            else
                Tween(CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-11975.78515625, 331.7734069824219, -10620.0302734375))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Jungle Pirate") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Jungle Pirate").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)

local Toggle = Tabs.IQ:AddToggle("Auto Farm", {
    Title = "ออโต้ฟาร์ม เศษโลหะ", 
    Description = "Auto Farm Scrap Metal",
    Default = false,
    Callback = function(Value)
        _G.ScrapMetal = Value
        StopTween( _G.ScrapMetal)
    end
})
spawn(function()
    while task.wait() do
        if _G.ScrapMetal and World1 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Brute") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Brute" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not Scrap or not _G.ScrapMetal or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos9.Position).Magnitude > 1500 then
                BTP(CFrame.new(-1132.4202880859375, 14.844913482666016, 4293.30517578125))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos9.Position).Magnitude < 1500 then
                Tween(CFrame.new(-1132.4202880859375, 14.844913482666016, 4293.30517578125))
                end
            else
               Tween(CFrame.new(-1132.4202880859375, 14.844913482666016, 4293.30517578125))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-1132.4202880859375, 14.844913482666016, 4293.30517578125))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Brute") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Brute").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        if _G.ScrapMetal and World2 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Mercenary") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Mercenary" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.ScrapMetal or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos10.Position).Magnitude > 1500 then
                BTP(CFrame.new(-972.307373046875, 73.04473876953125, 1419.2901611328125))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos10.Position).Magnitude < 1500 then
                Tween(CFrame.new(-972.307373046875, 73.04473876953125, 1419.2901611328125))
                end
            else
                Tween(CFrame.new(-972.307373046875, 73.04473876953125, 1419.2901611328125))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-972.307373046875, 73.04473876953125, 1419.2901611328125))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Mercenary") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Mercenary").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)
spawn(function()
    while task.wait() do
        if _G.ScrapMetal and World3 then
            pcall(function()
                if game:GetService("Workspace").Enemies:FindFirstChild("Pirate Millionaire") then
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if v.Name == "Pirate Millionaire" then
                            if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                repeat task.wait()
                                    AutoHaki()
                                    Equip_Weapon_Farm_All(_G.SelectWeapon)
                                    v.HumanoidRootPart.CanCollide = false
                                    v.Humanoid.WalkSpeed = 0
                                    v.Head.CanCollide = false 
                                    MakoriGayMag = true
                                    PosGay = v.HumanoidRootPart.CFrame
                                    Tween(v.HumanoidRootPart.CFrame * randomPos)
                                until not _G.ScrapMetal or not v.Parent or v.Humanoid.Health <= 0
                                MakoriGayMag = false
                            end
                        end
                    end
                else
                if BypassTP then
                if (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos11.Position).Magnitude > 1500 then
                BTP(CFrame.new(-289.6311950683594, 43.8282470703125, 5583.66357421875))
                elseif (game.Players.LocalPlayer.Character.HumanoidRootPart.Position - MaterialsPos11.Position).Magnitude < 1500 then
                Tween(CFrame.new(-289.6311950683594, 43.8282470703125, 5583.66357421875))
                end
            else
                Tween(CFrame.new(-289.6311950683594, 43.8282470703125, 5583.66357421875))
            end
                UnEquip_Weapon_Farm_All(_G.SelectWeapon)
                Tween(CFrame.new(-289.6311950683594, 43.8282470703125, 5583.66357421875))
                    if game:GetService("ReplicatedStorage"):FindFirstChild("Pirate Millionaire") then
                        Tween(game:GetService("ReplicatedStorage"):FindFirstChild("Pirate Millionaire").HumanoidRootPart.CFrame * CFrame.new(2,20,2))
                    end
                end
            end)
        end
    end
end)


local Main = Tabs.Stats:AddSection("สถานะ & สเตตัส")
local PointStatus = Tabs.Stats:AddParagraph({
    Title = "You're now having : Not Points"
})
spawn(function()
    while task.wait() do
        pcall(function()
            PointStatus:SetTitle("You're now having "..tostring(game:GetService("Players")["LocalPlayer"].Data.Points.Value).. " Points")
        end)
    end
end)
local Status = Tabs.Stats:AddParagraph({
    Title = "Status : not"
})
spawn(function()
  while task.wait() do
    pcall(function()
      Status:SetTitle("หมัด: "..game.Players.LocalPlayer.Data.Stats.Melee.Level.Value.. " เลือด: "..game.Players.LocalPlayer.Data.Stats.Defense.Level.Value.. " ดาบ: "..game.Players.LocalPlayer.Data.Stats.Sword.Level.Value.. " ปืน: "..game.Players.LocalPlayer.Data.Stats.Gun.Level.Value.. " ผลปีศาจ: "..game.Players.LocalPlayer.Data.Stats["Demon Fruit"].Level.Value)
    end)
  end
end)
local Toggle = Tabs.Stats:AddToggle("Auto Up Stats", {
    Title = "Melee",
    Default = true,
    Callback = function(Value)
        _G.Melee = Value
    end
})
local Toggle = Tabs.Stats:AddToggle("Auto Up Stats", {
    Title = "Defense",
    Default = false,
    Callback = function(Value)
        _G.Defense = Value
    end
})    
local Toggle = Tabs.Stats:AddToggle("Auto Up Stats", {
    Title = "Sword", 
    Default = false,
    Callback = function(Value)
        _G.Sword = Value
    end
})    
local Toggle = Tabs.Stats:AddToggle("Auto Up Stats", {
    Title = "Gun", 
    Default = false,
    Callback = function(Value)
        _G.Gun = Value
    end
})    
local Toggle = Tabs.Stats:AddToggle("Auto Up Stats", {
    Title = "Demon Fruit", 
    Default = false,
    Callback = function(Value)
        _G.DemonFruit = Value
    end
})    

spawn(function()
    while task.wait() do
        pcall(function()
            local a = _G.Melee
            local b = _G.Defense
            local c = _G.Sword
            local d = _G.Gun
            local e = _G.DemonFruit           
            local f = {a, b, c, d, e}
            local g = {"Melee", "Defense", "Sword", "Gun", "Demon Fruit"}            
            for h = 1, #f do
                if f[h] then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", g[h], 1)
                end
            end
        end)
    end
end)




local Main = Tabs.TP:AddSection("Join World")
Tabs.TP:AddButton({
    Title = "เทเลพอร์ตไปยัง โลก1",
    Description = "Teleport To Frist Sea",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelMain")
    end
})
Tabs.TP:AddButton({
    Title = "เทเลพอร์ตไปยัง โลก2",
    Description = "Teleport To Second Sea",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
    end
})
Tabs.TP:AddButton({
    Title = "เทเลพอร์ตไปยัง โลก3",
    Description = "Teleport To Third Sea",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
    end
})
local Main = Tabs.TP:AddSection("Teleport Island")
if World1 then
    local SelectIsland = Tabs.TP:AddDropdown("SelectIsland", {
        Title = "Select Island",
        Values = {
            "WindMill",
            "Marine",
            "Middle Town",
            "Jungle",
            "Pirate Village",
            "Desert",
            "Snow Island",
            "MarineFord",
            "Colosseum",
            "Sky Island 1",
            "Sky Island 2",
            "Sky Island 3",
            "Prison",
            "Magma Village",
            "Under Water Island",
            "Fountain City",
            "Shank Room",
            "Mob Island",
        },
        Multi = false,
        Default = _G.SelectIsland,
    })
    SelectIsland:OnChanged(function(Value)
        _G.SelectIsland = Value 
    end)
end

if World2 then
    local SelectIsland = Tabs.TP:AddDropdown("SelectIsland", {
        Title = "Select Island",
        Values = {
            "The Cafe",
            "First Spot",
            "Dark Area",
            "Flamingo Mansion",
            "Flamingo Room",
            "Green Zone",
            "Factory",
            "Colosseum",
            "Zombie Island",
            "Two Snow Mountain",
            "Punk Hazard",
            "Cursed Ship",
            "Ice Castle",
            "Forgotten Island",
            "Ussop Island",
            "Mini Sky Island"
        },
        Multi = false,
        Default = _G.SelectIsland,
    })
    SelectIsland:OnChanged(function(Value)
        _G.SelectIsland = Value 
    end)
end

if World3 then
    local SelectIsland = Tabs.TP:AddDropdown("SelectIsland", {
        Title = "Select Island",
        Values = {
            "Mansion",
            "Port Town",
            "Great Tree",
            "Castle On The Sea",
            "MiniSky", 
            "Hydra Island",
            "Floating Turtle",
            "Haunted Castle",
            "Ice Cream Island",
            "Peanut Island",
            "Cake Island",
            "Cocoa Island",
            "Candy Island New",
            "Tiki Outpost"
        },
        Multi = false,
        Default = _G.SelectIsland,
    })
    SelectIsland:OnChanged(function(Value)
        _G.SelectIsland = Value 
    end)
end
local Toggle = Tabs.TP:AddToggle("Auto Teleport To Select Island", {
    Title = "เทเลพอร์ตไปยังเกราะ [Selection]", 
    Description = "Teleport To Select Island", 
    Default = false,
    Callback = function(Value)
  _G.TeleportIsland = Value
    if _G.TeleportIsland == true then
        repeat wait()
            if _G.SelectIsland == "WindMill" then
                Tween(CFrame.new(979.79895019531, 16.516613006592, 1429.0466308594))
            elseif _G.SelectIsland == "Marine" then
                Tween(CFrame.new(-2566.4296875, 6.8556680679321, 2045.2561035156))
            elseif _G.SelectIsland == "Middle Town" then
                Tween(CFrame.new(-690.33081054688, 15.09425163269, 1582.2380371094))
            elseif _G.SelectIsland == "Jungle" then
                Tween(CFrame.new(-1612.7957763672, 36.852081298828, 149.12843322754))
            elseif _G.SelectIsland == "Pirate Village" then
                Tween(CFrame.new(-1181.3093261719, 4.7514905929565, 3803.5456542969))
            elseif _G.SelectIsland == "Desert" then
                Tween(CFrame.new(944.15789794922, 20.919729232788, 4373.3002929688))
            elseif _G.SelectIsland == "Snow Island" then
                Tween(CFrame.new(1347.8067626953, 104.66806030273, -1319.7370605469))
            elseif _G.SelectIsland == "MarineFord" then
                Tween(CFrame.new(-4914.8212890625, 50.963626861572, 4281.0278320313))
            elseif _G.SelectIsland == "Colosseum" then
                Tween( CFrame.new(-1427.6203613281, 7.2881078720093, -2792.7722167969))
            elseif _G.SelectIsland == "Sky Island 1" then
                Tween(CFrame.new(-4869.1025390625, 733.46051025391, -2667.0180664063))
            elseif _G.SelectIsland == "Sky Island 2" then  
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
            elseif _G.SelectIsland == "Sky Island 3" then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
            elseif _G.SelectIsland == "Prison" then
                Tween( CFrame.new(4875.330078125, 5.6519818305969, 734.85021972656))
            elseif _G.SelectIsland == "Magma Village" then
                Tween(CFrame.new(-5247.7163085938, 12.883934020996, 8504.96875))
            elseif _G.SelectIsland == "Under Water Island" then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
            elseif _G.SelectIsland == "Fountain City" then
                Tween(CFrame.new(5127.1284179688, 59.501365661621, 4105.4458007813))
            elseif _G.SelectIsland == "Shank Room" then
                Tween(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
            elseif _G.SelectIsland == "Mob Island" then
                Tween(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
            elseif _G.SelectIsland == "The Cafe" then
                Tween(CFrame.new(-380.47927856445, 77.220390319824, 255.82550048828))
            elseif _G.SelectIsland == "Frist Spot" then
                Tween(CFrame.new(-11.311455726624, 29.276733398438, 2771.5224609375))
            elseif _G.SelectIsland == "Dark Area" then
                Tween(CFrame.new(3780.0302734375, 22.652164459229, -3498.5859375))
            elseif _G.SelectIsland == "Flamingo Mansion" then
                Tween(CFrame.new(-483.73370361328, 332.0383605957, 595.32708740234))
            elseif _G.SelectIsland == "Flamingo Room" then
                Tween(CFrame.new(2284.4140625, 15.152037620544, 875.72534179688))
            elseif _G.SelectIsland == "Green Zone" then
                Tween( CFrame.new(-2448.5300292969, 73.016105651855, -3210.6306152344))
            elseif _G.SelectIsland == "Factory" then
                Tween(CFrame.new(424.12698364258, 211.16171264648, -427.54049682617))
            elseif _G.SelectIsland == "Colossuim" then
                Tween( CFrame.new(-1503.6224365234, 219.7956237793, 1369.3101806641))
            elseif _G.SelectIsland == "Zombie Island" then
                Tween(CFrame.new(-5622.033203125, 492.19604492188, -781.78552246094))
            elseif _G.SelectIsland == "Two Snow Mountain" then
                Tween(CFrame.new(753.14288330078, 408.23559570313, -5274.6147460938))
            elseif _G.SelectIsland == "Punk Hazard" then
                Tween(CFrame.new(-6127.654296875, 15.951762199402, -5040.2861328125))
            elseif _G.SelectIsland == "Cursed Ship" then
                Tween(CFrame.new(923.40197753906, 125.05712890625, 32885.875))
            elseif _G.SelectIsland == "Ice Castle" then
                Tween(CFrame.new(6148.4116210938, 294.38687133789, -6741.1166992188))
            elseif _G.SelectIsland == "Forgotten Island" then
                Tween(CFrame.new(-3032.7641601563, 317.89672851563, -10075.373046875))
            elseif _G.SelectIsland == "Ussop Island" then
                Tween(CFrame.new(4816.8618164063, 8.4599885940552, 2863.8195800781))
            elseif _G.SelectIsland == "Mini Sky Island" then
                Tween(CFrame.new(-288.74060058594, 49326.31640625, -35248.59375))
            elseif _G.SelectIsland == "Great Tree" then
                Tween(CFrame.new(2681.2736816406, 1682.8092041016, -7190.9853515625))
            elseif _G.SelectIsland == "Castle On The Sea" then
                Tween(CFrame.new(-5074.45556640625, 314.5155334472656, -2991.054443359375))
            elseif _G.SelectIsland == "MiniSky" then
                Tween(CFrame.new(-260.65557861328, 49325.8046875, -35253.5703125))
            elseif _G.SelectIsland == "Port Town" then
                Tween(CFrame.new(-290.7376708984375, 6.729952812194824, 5343.5537109375))
            elseif _G.SelectIsland == "Hydra Island" then
                Tween(CFrame.new(5228.8842773438, 604.23400878906, 345.0400390625))
            elseif _G.SelectIsland == "Floating Turtle" then
                Tween(CFrame.new(-13274.528320313, 531.82073974609, -7579.22265625))
            elseif _G.SelectIsland == "Mansion" then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-12471.169921875, 374.94024658203, -7551.677734375))
            elseif _G.SelectIsland == "Haunted Castle" then
                Tween(CFrame.new(-9515.3720703125, 164.00624084473, 5786.0610351562))
            elseif _G.SelectIsland == "Ice Cream Island" then
                Tween(CFrame.new(-902.56817626953, 79.93204498291, -10988.84765625))
            elseif _G.SelectIsland == "Peanut Island" then
                Tween(CFrame.new(-2062.7475585938, 50.473892211914, -10232.568359375))
            elseif _G.SelectIsland == "Cake Island" then
                Tween(CFrame.new(-1884.7747802734375, 19.327526092529297, -11666.8974609375))
            elseif _G.SelectIsland == "Cocoa Island" then
                Tween(CFrame.new(87.94276428222656, 73.55451202392578, -12319.46484375))
            elseif _G.SelectIsland == "Candy Island New⛄" then
                Tween(CFrame.new(-1014.4241943359375, 149.11068725585938, -14555.962890625))
            elseif _G.SelectIsland == "Tiki Outpost" then
                Tween(CFrame.new(-1149.328, 13.5759039, -14445.6143, -0.156446099, 0, -0.987686574, 0, 1, 0, 0.987686574, 0, -0.156446099))
            end
        until not _G.TeleportIsland
    end
    StopTween(_G.TeleportIsland)
    end
})


local Main = Tabs.ESP:AddSection("ESP ตำแหน่ง")
local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งผู้เล่น", 
    Description = "ESP Players",
    Default = false,
    Callback = function(Value)
        _G.ESPPLayers = Value
    ESPPlayer = Value
    UpdatePlayerChams()
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.ESPPLayers then
                UpdatePlayerChams()
            end
        end
    end)
end)

local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งเกราะ", 
    Description = "ESP Island",
    Default = false,
    Callback = function(Value)
        _G.ESPIsland = Value
    IslandESP = Value
    UpdateIslandESP()
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.ESPIsland then
                UpdateIslandESP()
            end
        end
    end)
end)
local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งเบรี", 
    Description = "ESP Chest",
    Default = false,
    Callback = function(Value)
        _G.ESPCHESTE = Value
    ChestESP = Value
    UpdateChestChams()
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.ESPCHESTE then
                UpdateChestChams()
            end
        end
    end)
end)
local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งผลไม้ปีศาจ", 
    Description = "ESP DevilFruit",
    Default = false,
    Callback = function(Value)
        _G.DevilFruitESP = Value
    DevilFruitESP = Value
    UpdateDevilChams()
    end
})
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.DevilFruitESP then
                UpdateDevilChams() 
            end
        end
    end)
end)
if World2 then
local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งดอกไม้", 
    Description = "ESP Flower",
    Default = false,
    Callback = function(Value)
        _G.ESPFloweers = Value
    FlowerESP = Value
    UpdateFlowerChams()
    end
})
end
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.ESPFloweers then
                UpdateFlowerChams()
            end
        end
    end)
end)
if World3 then
local Toggle = Tabs.ESP:AddToggle("ESP", {
    Title = "ตำแหน่งเกราะลับ", 
    Description = "ESP Mirage Island",
    Default = false,
    Callback = function(Value)
        _G.ESPMirageIsland = Value
    MirageIslandESP = Value
    UpdateIslandMirageESP() 
    end
})
end
spawn(function()
    pcall(function()
        while task.wait() do
            if _G.ESPMirageIsland then
                UpdateIslandMirageESP() 
            end
        end
    end)
end)

local Main = Tabs.Shop:AddSection("Auto Buyer Abilities")
Tabs.Shop:AddButton({
    Title = "Buy Geppo [$10,000 Beli]",
    Description = "ซื้อเดินชมจันทร์",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Geppo")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Buso Haki [$25,000 Beli]",
    Description = "ซื้อฮาคิเกราะ",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Buso")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Soru [$25,000 Beli]",
    Description = "ซื้อโซล",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Soru")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Observation Haki [$750,000 Beli]",
    Description = "ซื้อฮาคิสังเกตุ",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk","Buy")
    end
})
local Main = Tabs.Shop:AddSection("Auto Buyer Melee")
Tabs.Shop:AddButton({
    Title = "Buy Black Leg [$150,000 Beli]",
    Description = "ซื้อขาดำ V1",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBlackLeg")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Electro [$550,000 Beli]",
    Description = "ซื้อหมัดสายฟ้า V1",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Fishman Karate [$750,000 Beli]",
    Description = "ซื้อหมัดมนุษย์เงือก V1",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Dragon Claw [$1,500 Fragments]",
    Description = "ซื้อหมัดมังกร V1",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Superhuman [$3,000,000 Beli]",
    Description = "ซื้อหมัดชุปเปอร์ฮิวเมน V1",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Death Step [$5,000 Fragments + $5,000,000 Beli]",
    Description = "ซื้อขาดำ V2",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Sharkman Karate [$5,000 Fragments + $2,500,000 Beli]",
    Description = "ซื้อหมัดมนุษย์เงือก V2",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate",true)
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Electric Claw [$5,000 Fragments + $3,000,000 Beli]",
    Description = "ซื้อหมัดสายฟ้า V2",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Dragon Talon [$5,000 Fragments + $3,000,000 Beli]",
    Description = "ซื้อหมัดมังกร V2",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDragonTalon")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy God Human [$5,000 Fragments + $5,000,000 Beli]",
    Description = "ซื้อหมัดก็อตฮิวเมน V2",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyGodhuman")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Sanguine Art [$5,000 Fragments + $5,000,000 Beli]",
    Description = "ซื้อหมัดแวมไพร์",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySanguineArt", true)
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySanguineArt")
    end
})

local Main = Tabs.Shop:AddSection("Auto Buyer Sword")
Tabs.Shop:AddButton({
    Title = "Buy Cutlass [$1,000 Beli]",
    Description = "ซื้อมีดสั้น",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Cutlass")
    end
})
Tabs.Shop:AddButton({
    Title = "Buy Katana [$1,000 Beli]",
    Description = "ซื้อดาบคาตานะ",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Katana")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อกระบองเหล็ก",
    Description = "Buy Iron Mace [$25,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Iron Mace")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อดาบคาตานะคู่",
    Description = "Buy Dual Katana [$12,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Duel Katana")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อดาบทริปเปิลคาตานะ",
    Description = "Buy Triple Katana [$60,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Triple Katana")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อท่อ",
    Description = "Buy Pipe [$100,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Pipe")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อใบมีดสองหัว",
    Description = "Buy Dual-Headed Blade [$400,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Dual-Headed Blade")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อดาบหนวดขาว",
    Description = "Buy Bisento [$1,200,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Bisento")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อไม้เท้าวิญญาณ",
    Description = "Buy Soul Cane [$750,000 Beli]",
    Callback = function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Soul Cane")
    end
})
Tabs.Shop:AddButton({
    Title = "ซื้อโพ V2",
    Description = "Buy Pole V2 [5,000 Fragments]",
    Callback = function()
        game.ReplicatedStorage.Remotes.CommF_:InvokeServer("ThunderGodTalk")
    end
})

local Main = Tabs.Misc:AddSection("Join Server")

-- ปุ่มย้ายเชิร์ฟ
Tabs.Misc:AddButton({
    Title = "ย้ายเชิร์ฟ",
    Description = "Join Server ",
    Callback = function()
        Hop()
    end
})
-- FastAttack 
local environment, replicatedstorage, players, net, client, modulepath, characterfolder, enemyfolder do
	environment = (getgenv or getrenv or getfenv)()
	replicatedstorage = game:GetService("ReplicatedStorage")
	players = game:GetService("Players")
	client = players.LocalPlayer
	modulepath = replicatedstorage:WaitForChild("Modules")
	net = modulepath:WaitForChild("Net")
	characterfolder = workspace:WaitForChild("Characters")
	enemyfolder = workspace:WaitForChild("Enemies")
end

local Module = {}
Module.AttackCooldown = tick()
local CachedChars = {}

function Module.IsAlive(Char: Model?): boolean
	if not Char then
		return nil
	end

	if CachedChars[Char] then
		return CachedChars[Char].Health > 0
	end

	local Hum = Char:FindFirstChildOfClass("Humanoid")
	CachedChars[Char] = Hum
	return Hum and Hum.Health > 0
end

local Settings = {
	ClickDelay = 0.01,
	AutoClick = true
}

Module.FastAttack = (function()
	if environment._trash_attack then
		return environment._trash_attack
	end

	local module = {
		NextAttack = 0,
		Distance = 55,
		attackMobs = true,
		attackPlayers = true
	}

	local RegisterAttack = net:WaitForChild("RE/RegisterAttack")
	local RegisterHit = net:WaitForChild("RE/RegisterHit")

	function module:AttackEnemy(EnemyHead,Table) 
		if EnemyHead and client:DistanceFromCharacter(EnemyHead.Position) < self.Distance then
			if not self.FirstAttack then
				RegisterAttack:FireServer(Settings.ClickDelay or 0.125)
				self.FirstAttack = true
			end
			RegisterHit:FireServer(EnemyHead, (Table) and Table or {})
		end
	end

	function module:AttackNearest()
		local args = {
			[1] = nil,
			[2] = {}
		}
		for _, Enemy in enemyfolder:GetChildren() do
			if not args[1] and Enemy:FindFirstChild("HumanoidRootPart",true) and client:DistanceFromCharacter(Enemy.HumanoidRootPart.Position) < self.Distance then
				args[1] = Enemy:FindFirstChild("UpperTorso")
			else
				if Enemy:FindFirstChild("HumanoidRootPart",true) and client:DistanceFromCharacter(Enemy.HumanoidRootPart.Position) < self.Distance then
					table.insert(args[2],{
						[1] = Enemy,
						[2] = Enemy:FindFirstChild("UpperTorso")
					})
				end
			end
		end
		self:AttackEnemy(unpack(args))

		for _, Enemy in characterfolder:GetChildren() do
			if Enemy ~= client.Character then
				self:AttackEnemy(Enemy:FindFirstChild("UpperTorso"))
			end
		end

		if not self.FirstAttack then
			task.wait(0.5)
		end
	end

	function module:BladeHits()
		self:AttackNearest()
		self.FirstAttack = false
	end

	task.spawn(function()
		while task.wait(Settings.ClickDelay or 0.125) do
			if (tick() - Module.AttackCooldown) < 0.4833333194255829 then continue end
			if not Settings.AutoClick then continue end
			if not Module.IsAlive(client.Character) then continue end
			if not client.Character:FindFirstChildOfClass("Tool") then continue end

			module:BladeHits()
		end
	end)

	environment._trash_attack = module
	return module
end)()
