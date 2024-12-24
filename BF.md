if game.PlaceId == 2753915549 then
   World1 = true
elseif game.PlaceId == 4442272183 then
   World2 = true
elseif game.PlaceId == 7449423635 then
   World3 = true
end

function CheckLevel()
    Lv = selff.Data.Level.Value;
    if WorldCheck["First Sea"] then
        if ((Lv == 1 or Lv <= 9) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Bandit" and not Configs.Farming.Level.AutoFarm) then
            return {
                [1] = "Bandit [Lv. 5]";
                [2] = "BanditQuest1";
                [3] = 1;
                [4] = "Bandit";
                [5] = CF(1060.9383544922, 16.455066680908, 1547.7841796875);
                [6] = CF(1038.5533447266, 41.296249389648, 1576.5098876953)
            }
        elseif ((Lv == 10 or Lv <= 14) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Monkey") then
            return {
                [1] = "Monkey [Lv. 14]";
                [2] = "JungleQuest";
                [3] = 1;
                [4] = "Monkey";
                [5] = CF(-1601.6553955078, 36.85213470459, 153.38809204102);
                [6] = CF(-1448.1446533203, 50.851993560791, 63.60718536377)
            }
        elseif ((Lv == 15 or Lv <= 29) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Gorilla") then
            return {
                [1] = "Gorilla [Lv. 20]";
                [2] = "JungleQuest";
                [3] = 2;
                [4] = "Gorilla";
                [5] = CF(-1601.6553955078, 36.85213470459, 153.38809204102);
                [6] = CF(-1142.6488037109, 40.462348937988, -515.39227294922)
            }
        elseif ((Lv == 30 or Lv <= 39) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Pirate") then
            return {
                [1] = "Pirate [Lv. 35]";
                [2] = "BuggyQuest1";
                [3] = 1;
                [4] = "Pirate";
                [5] = CF(-1140.1761474609, 4.752049446106, 3827.4057617188);
                [6] = CF(-1201.0881347656, 40.628940582275, 3857.5966796875)
            }
        elseif ((Lv == 40 or Lv <= 59) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Brute") then 
            return {
                [1] = "Brute [Lv. 45]";
                [2] = "BuggyQuest1";
                [3] = 2;
                [4] = "Brute";
                [5] = CF(-1140.1761474609, 4.752049446106, 3827.4057617188);
                [6] = CF(-1387.5324707031, 24.592035293579, 4100.9575195313)
            }
        elseif ((Lv == 60 or Lv <= 74) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Desert Bandit") then 
            return {
                [1] = "Desert Bandit [Lv. 60]";
                [2] = "DesertQuest";
                [3] = 1;
                [4] = "Desert Bandit";
                [5] = CF(896.51721191406, 6.4384617805481, 4390.1494140625);
                [6] = CF(984.99896240234, 16.109552383423, 4417.91015625)
            }
        elseif ((Lv == 75 or Lv <= 89) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Desert Officer") then 
            return {
                [1] = "Desert Officer [Lv. 70]";
                [2] = "DesertQuest";
                [3] = 2;
                [4] = "Desert Officer";
                [5] = CF(896.51721191406, 6.4384617805481, 4390.1494140625);
                [6] = CF(1547.1510009766, 14.452038764954, 4381.8002929688)
            }
        elseif ((Lv == 90 or Lv <= 99) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Snow Bandit") then 
            return {
                [1] = "Snow Bandit [Lv. 90]";
                [2] = "SnowQuest";
                [3] = 1;
                [4] = "Snow Bandit";
                [5] = CF(1386.8073730469, 87.272789001465, -1298.3576660156);
                [6] = CF(1356.3028564453, 105.76865386963, -1328.2418212891)
            }
        elseif ((Lv == 100 or Lv <= 119) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Snowman") then 
            return {
                [1] = "Snowman [Lv. 100]";
                [2] = "SnowQuest";
                [3] = 2;
                [4] = "Snowman";
                [5] = CF(1386.8073730469, 87.272789001465, -1298.3576660156);
                [6] = CF(1218.7956542969, 138.01184082031, -1488.0262451172)
            }
        elseif ((Lv == 120 or Lv <= 149) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Chief Petty Officer") then 
            return {
                [1] = "Chief Petty Officer [Lv. 120]";
                [2] = "MarineQuest2";
                [3] = 1;
                [4] = "Chief Petty Officer";
                [5] = CF(-5035.49609375, 28.677835464478, 4324.1840820313);
                [6] = CF(-4931.1552734375, 65.793113708496, 4121.8393554688)
            }
        elseif ((Lv == 150 or Lv <= 174) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Sky Bandit") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(-4842.1372070313, 717.69543457031, -2623.0483398438) - selc.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance", Vec3(-4607.82275390625, 874.3905029296875, -1667.556884765625));
            end;
            return {
                [1] = "Sky Bandit [Lv. 150]";
                [2] = "SkyQuest";
                [3] = 1;
                [4] = "Sky Bandit";
                [5] = CF(-4842.1372070313, 717.69543457031, -2623.0483398438);
                [6] = CF(-4955.6411132813, 365.46365356445, -2908.1865234375)
            }         
        elseif ((Lv == 175 or Lv <= 189) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Dark Master") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(-4842.1372070313, 717.69543457031, -2623.0483398438) - selff.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance", Vec3(-4607.82275390625, 874.3905029296875, -1667.556884765625));
            end;
            return {
                [1] = "Dark Master [Lv. 175]";
                [2] = "SkyQuest";
                [3] = 2;
                [4] = "Dark Master";
                [5] = CF(-4842.1372070313, 717.69543457031, -2623.0483398438);
                [6] = CF(-5357.3515625, 449.032958984375, -2265.667236328125)
            }
        elseif ((Lv == 190 or Lv <= 209) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Prisoner") then 
            return {
                [1] = "Prisoner [Lv. 190]";
                [2] = "PrisonerQuest";
                [3] = 1;
                [4] = "Prisoner";
                [5] = CF(5308.98828125, 1.7804901599884033, 475.06048583984375);
                [6] = CF(5164.1083984375, 15.778244972229004, 489.6533508300781)
            }
        elseif ((Lv == 210 or Lv <= 249) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Dangerous Prisoner") then 
            return {
                [1] = "Dangerous Prisoner [Lv. 210]";
                [2] = "PrisonerQuest";
                [3] = 2;
                [4] = "Dangerous Prisoner";
                [5] = CF(5308.98828125, 1.7804901599884033, 475.06048583984375);
                [6] = CF(5564.0322265625, 15.759016036987305, 682.16455078125)
            }
        elseif ((Lv == 250 or Lv <= 274) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Toga Warrior") then 
            return {
                [1] = "Toga Warrior [Lv. 250]";
                [2] = "ColosseumQuest";
                [3] = 1;
                [4] = "Toga Warrior";
                [5] = CF(-1577.7890625, 7.4151420593262, -2984.4838867188);
                [6] = CF(-1872.5166015625, 49.080215454102, -2913.810546875)
            }
        elseif ((Lv == 275 or Lv <= 299) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Gladiator") then 
            return {
                [1] = "Gladiator [Lv. 275]";
                [2] = "ColosseumQuest";
                [3] = 2;
                [4] = "Gladiator";
                [5] = CF(-1577.7890625, 7.4151420593262, -2984.4838867188);
                [6] = CF(-1324.32666015625, 58.49076843261719, -3242.227294921875)
            }
        elseif ((Lv == 300 or Lv <= 329) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Military Soldier") then 
            return {
                [1] = "Military Soldier [Lv. 300]";
                [2] = "MagmaQuest";
                [3] = 1;
                [4] = "Military Soldier";
                [5] = CF(-5316.1157226563, 12.262831687927, 8517.00390625);
                [6] = CF(-5369.0004882813, 61.24352645874, 8556.4921875)
            }
        elseif ((Lv == 330 or Lv <= 374) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Military Spy") then 
            return {
                [1] = "Military Spy [Lv. 325]";
                [2] = "MagmaQuest";
                [3] = 2;
                [4] = "Military Spy";
                [5] = CF(-5316.1157226563, 12.262831687927, 8517.00390625);
                [6] = CF(-5984.0532226563, 82.14656829834, 8753.326171875)
            }
        elseif ((Lv == 375 or Lv <= 399) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Fishman Warrior") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(61122.65234375, 18.497442245483, 1569.3997802734) - selff.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance",Vec3(61163.8515625, 11.6796875, 1819.7841796875));
            end;
            return {
                [1] = "Fishman Warrior [Lv. 375]";
                [2] = "FishmanQuest";
                [3] = 1;
                [4] = "Fishman Warrior";
                [5] = CF(61122.65234375, 18.497442245483, 1569.3997802734);
                [6] = CF(60844.10546875, 98.462875366211, 1298.3985595703)
            }
        elseif ((Lv == 400 or Lv <= 449) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Fishman Commando") then 
            
            if Configs.Farming.Level.AutoFarm and (Vec3(61122.65234375, 18.497442245483, 1569.3997802734) - selff.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance",Vec3(61163.8515625, 11.6796875, 1819.7841796875));
            end;
            return {
                [1] = "Fishman Commando [Lv. 400]";
                [2] = "FishmanQuest";
                [3] = 2;
                [4] = "Fishman Commando";
                [5] = CF(61122.65234375, 18.497442245483, 1569.3997802734);
                [6] = CF(61738.3984375, 64.207321166992, 1433.8375244141)
            }
        elseif ((Lv == 450 or Lv <= 474) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "God's Guard") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(-4721.8603515625, 845.30297851563, -1953.8489990234) - selff.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance",Vec3(-4607.82275, 872.54248, -1667.55688));
            end;
            return {
                [1] = "God's Guard [Lv. 450]";
                [2] = "SkyExp1Quest";
                [3] = 1;
                [4] = "God's Guard";
                [5] = CF(-4721.8603515625, 845.30297851563, -1953.8489990234);
                [6] = CF(-4628.0498046875, 866.92877197266, -1931.2352294922)
            }
        elseif ((Lv == 475 or Lv <= 524) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Shanda") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(-7863.1596679688, 5545.5190429688, -378.42266845703) - selff.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                CommF:InvokeServer("requestEntrance", Vec3(-7894.6176757813, 5547.1416015625, -380.29119873047)); wait(3);
            end;
            return {
                [1] = "Shanda [Lv. 475]";
                [2] = "SkyExp1Quest";
                [3] = 2;
                [4] = "Shanda";
                [5] = CF(-7863.1596679688, 5545.5190429688, -378.42266845703);
                [6] = CF(-7685.1474609375, 5601.0751953125, -441.38876342773)
            }
        elseif ((Lv == 525 or Lv <= 549) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Royal Squad") then 
            return {
                [1] = "Royal Squad [Lv. 525]";
                [2] = "SkyExp2Quest";
                [3] = 1;
                [4] = "Royal Squad";
                [5] = CF(-7903.3828125, 5635.9897460938, -1410.923828125);
                [6] = CF(-7654.2514648438, 5637.1079101563, -1407.7550048828)
            }
        elseif ((Lv == 550 or Lv <= 624) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Royal Soldier") then 
            return {
                [1] = "Royal Soldier [Lv. 550]";
                [2] = "SkyExp2Quest";
                [3] = 2;
                [4] = "Royal Soldier";
                [5] = CF(-7903.3828125, 5635.9897460938, -1410.923828125);
                [6] = CF(-7760.4106445313, 5679.9077148438, -1884.8112792969)
            }
        elseif ((Lv == 625 or Lv <= 649) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Galley Pirate") then 
            return {
                [1] = "Galley Pirate [Lv. 625]";
                [2] = "FountainQuest";
                [3] = 1;
                [4] = "Galley Pirate";
                [5] = CF(5258.2788085938, 38.526931762695, 4050.044921875);
                [6] = CF(5557.1684570313, 152.32717895508, 3998.7758789063)
            }
        elseif (Lv >= 650 and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Galley Captain") then 
            return {
                [1] = "Galley Captain [Lv. 650]";
                [2] = "FountainQuest";
                [3] = 2;
                [4] = "Galley Captain";
                [5] = CF(5258.2788085938, 38.526931762695, 4050.044921875);
                [6] = CF(5677.6772460938, 92.786109924316, 4966.6323242188)
            }
        end
    elseif WorldCheck["Second Sea"] then
        if ((Lv == 700 or Lv <= 724) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Raider") then 
            return {
                [1] = "Raider [Lv. 700]";
                [2] = "Area1Quest";
                [3] = 1;
                [4] = "Raider";
                [5] = CF(-427.72567749023, 72.99634552002, 1835.9426269531);
                [6] = CF(68.874565124512, 93.635643005371, 2429.6752929688)
            }
        elseif ((Lv == 725 or Lv <= 774) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Mercenary") then 
            return {
                [1] = "Mercenary [Lv. 725]";
                [2] = "Area1Quest";
                [3] = 2;
                [4] = "Mercenary";
                [5] = CF(-427.72567749023, 72.99634552002, 1835.9426269531);
                [6] = CF(-864.85009765625, 122.47104644775, 1453.1505126953)
            }
        elseif ((Lv == 775 or Lv <= 799) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Swan Pirate") then 
            return {
                [1] = "Swan Pirate [Lv. 775]";
                [2] = "Area2Quest";
                [3] = 1;
                [4] = "Swan Pirate";
                [5] = CF(635.61151123047, 73.096351623535, 917.81298828125);
                [6] = CF(1065.3669433594, 137.64012145996, 1324.3798828125)
            }
        elseif ((Lv == 800 or Lv <= 874) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Factory Staff") then 
            return {
                [1] = "Factory Staff [Lv. 800]";
                [2] = "Area2Quest";
                [3] = 2;
                [4] = "Factory Staff";
                [5] = CF(635.61151123047, 73.096351623535, 917.81298828125);
                [6] = CF(533.22045898438, 128.46876525879, 355.62615966797)
            }
        elseif ((Lv == 875 or Lv <= 899) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Marine Lieutenant") then 
            return {
                [1] = "Marine Lieutenant [Lv. 875]";
                [2] = "MarineQuest3";
                [3] = 1;
                [4] = "Marine Lieutenant";
                [5] = CF(-2440.9934082031, 73.04190826416, -3217.7082519531);
                [6] = CF(-2489.2622070313, 84.613594055176, -3151.8830566406)
            }
        elseif ((Lv == 900 or Lv <= 949) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Marine Captain") then 
            return {
                [1] = "Marine Captain [Lv. 900]";
                [2] = "MarineQuest3";
                [3] = 2;
                [4] = "Marine Captain";
                [5] = CF(-2440.9934082031, 73.04190826416, -3217.7082519531);
                [6] = CF(-2335.2026367188, 79.786659240723, -3245.8674316406)
            }
        elseif ((Lv == 950 or Lv <= 974) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Zombie") then 
            return {
                [1] = "Zombie [Lv. 950]";
                [2] = "ZombieQuest";
                [3] = 1;
                [4] = "Zombie";
                [5] = CF(-5494.3413085938, 48.505931854248, -794.59094238281);
                [6] = CF(-5536.4970703125, 101.08577728271, -835.59075927734)
            }
        elseif ((Lv == 975 or Lv <= 999) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Vampire") then 
            return {
                [1] = "Vampire [Lv. 975]";
                [2] = "ZombieQuest";
                [3] = 2;
                [4] = "Vampire";
                [5] = CF(-5494.3413085938, 48.505931854248, -794.59094238281);
                [6] = CF(-5806.1098632813, 16.722528457642, -1164.4384765625)
            }
        elseif ((Lv == 1000 or Lv <= 1049) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Snow Trooper") then 
            return {
                [1] = "Snow Trooper [Lv. 1000]";
                [2] = "SnowMountainQuest";
                [3] = 1;
                [4] = "Snow Trooper";
                [5] = CF(607.05963134766, 401.44781494141, -5370.5546875);
                [6] = CF(535.21051025391, 432.74209594727, -5484.9165039063)
            }
        elseif ((Lv == 1050 or Lv <= 1099) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Winter Warrior") then 
            return {
                [1] = "Winter Warrior [Lv. 1050]";
                [2] = "SnowMountainQuest";
                [3] = 2;
                [4] = "Winter Warrior";
                [5] = CF(607.05963134766, 401.44781494141, -5370.5546875);
                [6] = CF(1234.4449462891, 456.95419311523, -5174.130859375)
            }
        elseif ((Lv == 1100 or Lv <= 1124) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Lab Subordinate") then 
            return {
                [1] = "Lab Subordinate [Lv. 1100]";
                [2] = "IceSideQuest";
                [3] = 1;
                [4] = "Lab Subordinate";
                [5] = CF(-6061.841796875, 15.926671981812, -4902.0385742188);
                [6] = CF(-5720.5576171875, 63.309471130371, -4784.6103515625)
            }
        elseif ((Lv == 1125 or Lv <= 1174) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Horned Warrior") then 
            return {
                [1] = "Horned Warrior [Lv. 1125]";
                [2] = "IceSideQuest";
                [3] = 2;
                [4] = "Horned Warrior";
                [5] = CF(-6061.841796875, 15.926671981812, -4902.0385742188);
                [6] = CF(-6292.751953125, 91.181983947754, -5502.6499023438)
            }
        elseif ((Lv == 1175 or Lv <= 1199) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Magma Ninja") then 
            return {
                [1] = "Magma Ninja [Lv. 1175]";
                [2] = "FireSideQuest";
                [3] = 1;
                [4] = "Magma Ninja";
                [5] = CF(-5429.0473632813, 15.977565765381, -5297.9614257813);
                [6] = CF(-5461.8388671875, 130.36347961426, -5836.4702148438)
            }
        elseif ((Lv == 1200 or Lv <= 1249) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Lava Pirate") then 
            return {
                [1] = "Lava Pirate [Lv. 1200]";
                [2] = "FireSideQuest";
                [3] = 2;
                [4] = "Lava Pirate";
                [5] = CF(-5429.0473632813, 15.977565765381, -5297.9614257813);
                [6] = CF(-5251.1889648438, 55.164535522461, -4774.4096679688)
            }
        elseif ((Lv == 1250 or Lv <= 1274) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ship Deckhand") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(1040.2927246094, 125.08293151855, 32911.0390625) - selff.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                CommF:InvokeServer("requestEntrance",Vec3(923.21252441406, 126.9760055542, 32852.83203125));
            end;
            return {
                [1] = "Ship Deckhand [Lv. 1250]";
                [2] = "ShipQuest1";
                [3] = 1;
                [4] = "Ship Deckhand";
                [5] = CF(1040.2927246094, 125.08293151855, 32911.0390625);
                [6] = CF(921.12365722656, 125.9839553833, 33088.328125)
            }
        elseif ((Lv == 1275 or Lv <= 1299) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ship Engineer") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(1040.2927246094, 125.08293151855, 32911.0390625) - selff.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                CommF:InvokeServer("requestEntrance",Vec3(923.21252441406, 126.9760055542, 32852.83203125));
            end;
            return {
                [1] = "Ship Engineer [Lv. 1275]";
                [2] = "ShipQuest1";
                [3] = 2;
                [4] = "Ship Engineer";
                [5] = CF(1040.2927246094, 125.08293151855, 32911.0390625);
                [6] = CF(886.28179931641, 40.47790145874, 32800.83203125)
            }
        elseif ((Lv == 1300 or Lv <= 1324) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ship Steward") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(1040.2927246094, 125.08293151855, 32911.0390625) - selff.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                CommF:InvokeServer("requestEntrance",Vec3(923.21252441406, 126.9760055542, 32852.83203125));
            end;
            return {
                [1] = "Ship Steward [Lv. 1300]";
                [2] = "ShipQuest2";
                [3] = 1;
                [4] = "Ship Steward";
                [5] = CF(971.42065429688, 125.08293151855, 33245.54296875);
                [6] = CF(943.85504150391, 129.58183288574, 33444.3671875)
            }
        elseif ((Lv == 1325 or Lv <= 1349) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ship Officer") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(1040.2927246094, 125.08293151855, 32911.0390625) - selff.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                CommF:InvokeServer("requestEntrance",Vec3(923.21252441406, 126.9760055542, 32852.83203125));
            end;
            return {
                [1] = "Ship Officer [Lv. 1325]";
                [2] = "ShipQuest2";
                [3] = 2;
                [4] = "Ship Officer";
                [5] = CF(971.42065429688, 125.08293151855, 33245.54296875);
                [6] = CF(955.38458251953, 181.08335876465, 33331.890625)
            }
        elseif ((Lv == 1350 or Lv <= 1374) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Arctic Warrior") then 
            if Configs.Farming.Level.AutoFarm and (Vec3(5668.1372070313, 28.202531814575, -6484.6005859375) - selff.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                CommF:InvokeServer("requestEntrance",Vec3(-6508.5581054688, 89.034996032715, -132.83953857422));
            end;
            return {
                [1] = "Arctic Warrior [Lv. 1350]";
                [2] = "FrostQuest";
                [3] = 1;
                [4] = "Arctic Warrior";
                [5] = CF(5668.1372070313, 28.202531814575, -6484.6005859375);
                [6] = CF(5935.4541015625, 77.26016998291, -6472.7568359375)
            }
        elseif ((Lv == 1375 or Lv <= 1424) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Snow Lurker") then 
            return {
                [1] = "Snow Lurker [Lv. 1375]";
                [2] = "FrostQuest";
                [3] = 2;
                [4] = "Snow Lurker";
                [5] = CF(5668.1372070313, 28.202531814575, -6484.6005859375);
                [6] = CF(5628.482421875, 57.574996948242, -6618.3481445313)
            }
        elseif ((Lv == 1425 or Lv <= 1449) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Sea Soldier") then 
            return {
                [1] = "Sea Soldier [Lv. 1425]";
                [2] = "ForgottenQuest";
                [3] = 1;
                [4] = "Sea Soldier";
                [5] = CF(-3054.5827636719, 236.87213134766, -10147.790039063);
                [6] = CF(-3185.0153808594, 58.789089202881, -9663.6064453125)
            }
        elseif (Lv >= 1450 and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Water Fighter") then 
            return {
                [1] = "Water Fighter [Lv. 1450]";
                [2] = "ForgottenQuest";
                [3] = 2;
                [4] = "Water Fighter";
                [5] = CF(-3054.5827636719, 236.87213134766, -10147.790039063);
                [6] = CF(-3262.9301757813, 298.69036865234, -10552.529296875)
            }
        end
    elseif WorldCheck["Third Sea"] then
        if ((Lv == 1500 or Lv <= 1524) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Pirate Millionaire") then 
            return {
                [1] = "Pirate Millionaire [Lv. 1500]";
                [2] = "PiratePortQuest";
                [3] = 1;
                [4] = "Pirate Millionaire";
                [5] = CF(-289.61752319336, 43.819011688232, 5580.0903320313);
                [6] = CF(-435.68109130859, 189.69866943359, 5551.0756835938)
            }
        elseif ((Lv == 1525 or Lv <= 1574) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Pistol Billionaire") then 
            return {
                [1] = "Pistol Billionaire [Lv. 1525]";
                [2] = "PiratePortQuest";
                [3] = 2;
                [4] = "Pistol Billionaire";
                [5] = CF(-289.61752319336, 43.819011688232, 5580.0903320313);
                [6] = CF(-236.53652954102, 217.46676635742, 6006.0883789063)
            }
        elseif ((Lv == 1575 or Lv <= 1599) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Dragon Crew Warrior") then 
            return {
                [1] = "Dragon Crew Warrior [Lv. 1575]";
                [2] = "AmazonQuest";
                [3] = 1;
                [4] = "Dragon Crew Warrior";
                [5] = CF(5833.1147460938, 51.60498046875, -1103.0693359375);
                [6] = CF(6301.9975585938, 104.77153015137, -1082.6075439453)
            }
        elseif ((Lv == 1600 or Lv <= 1624) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Dragon Crew Archer") then 
            return {
                [1] = "Dragon Crew Archer [Lv. 1600]";
                [2] = "AmazonQuest";
                [3] = 2;
                [4] = "Dragon Crew Archer";
                [5] = CF(5833.1147460938, 51.60498046875, -1103.0693359375);
                [6] = CF(6831.1171875, 441.76708984375, 446.58615112305)
            }
        elseif ((Lv == 1625 or Lv <= 1649) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Female Islander") then 
            return {
                [1] = "Female Islander [Lv. 1625]";
                [2] = "AmazonQuest2";
                [3] = 1;
                [4] = "Female Islander";
                [5] = CF(5446.8793945313, 601.62945556641, 749.45672607422);
                [6] = CF(5792.5166015625, 848.14392089844, 1084.1818847656)
            }
        elseif ((Lv == 1650 or Lv <= 1699) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Giant Islander") then 
            return {
                [1] = "Giant Islander [Lv. 1650]";
                [2] = "AmazonQuest2";
                [3] = 2;
                [4] = "Giant Islander";
                [5] = CF(5446.8793945313, 601.62945556641, 749.45672607422);
                [6] = CF(5009.5068359375, 664.11071777344, -40.960144042969)
            }
        elseif ((Lv == 1700 or Lv <= 1724) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Marine Commodore") then 
            return {
                [1] = "Marine Commodore [Lv. 1700]";
                [2] = "MarineTreeIsland";
                [3] = 1;
                [4] = "Marine Commodore";
                [5] = CF(2179.98828125, 28.731239318848, -6740.0551757813);
                [6] = CF(2198.0063476563, 128.71075439453, -7109.5043945313)
            }
        elseif ((Lv == 1725 or Lv <= 1774) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Marine Rear Admiral") then 
            return {
                [1] = "Marine Rear Admiral [Lv. 1725]";
                [2] = "MarineTreeIsland";
                [3] = 2;
                [4] = "Marine Rear Admiral";
                [5] = CF(2179.98828125, 28.731239318848, -6740.0551757813);
                [6] = CF(3294.3142089844, 385.41125488281, -7048.6342773438)
            }
        elseif ((Lv == 1775 or Lv <= 1799) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Fishman Raider") then 
            return {
                [1] = "Fishman Raider [Lv. 1775]";
                [2] = "DeepForestIsland3";
                [3] = 1;
                [4] = "Fishman Raider";
                [5] = CF(-10582.759765625, 331.78845214844, -8757.666015625);
                [6] = CF(-10553.268554688, 521.38439941406, -8176.9458007813)
            }
        elseif ((Lv == 1800 or Lv <= 1824) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Fishman Captain") then 
            return {
                [1] = "Fishman Captain [Lv. 1800]";
                [2] = "DeepForestIsland3";
                [3] = 2;
                [4] = "Fishman Captain";
                [5] = CF(-10583.099609375, 331.78845214844, -8759.4638671875);
                [6] = CF(-10789.401367188, 427.18637084961, -9131.4423828125)
            }
        elseif ((Lv == 1825 or Lv <= 1849) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Forest Pirate") then 
            return {
                [1] = "Forest Pirate [Lv. 1825]";
                [2] = "DeepForestIsland";
                [3] = 1;
                [4] = "Forest Pirate";
                [5] = CF(-13232.662109375, 332.40396118164, -7626.4819335938);
                [6] = CF(-13489.397460938, 400.30349731445, -7770.251953125)
            }
        elseif ((Lv == 1850 or Lv <= 1899) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Mythological Pirate") then 
            return {
                [1] = "Mythological Pirate [Lv. 1850]";
                [2] = "DeepForestIsland";
                [3] = 2;
                [4] = "Mythological Pirate";
                [5] = CF(-13232.662109375, 332.40396118164, -7626.4819335938);
                [6] = CF(-13508.616210938, 582.46228027344, -6985.3037109375)
            }
        elseif ((Lv >= 1900 and Lv <= 1924) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Jungle Pirate") then 
            return {
                [1] = "Jungle Pirate [Lv. 1900]";
                [2] = "DeepForestIsland2";
                [3] = 1;
                [4] = "Jungle Pirate";
                [5] = CF(-12682.096679688, 390.88653564453, -9902.1240234375);
                [6] = CF(-12267.103515625, 459.75262451172, -10277.200195313)
            }
        elseif ((Lv >= 1925 and Lv <= 1974) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Musketeer Pirate") then 
            return {
                [1] = "Musketeer Pirate [Lv. 1925]";
                [2] = "DeepForestIsland2";
                [3] = 2;
                [4] = "Musketeer Pirate";
                [5] = CF(-12682.096679688, 390.88653564453, -9902.1240234375);
                [6] = CF(-13291.5078125, 520.47338867188, -9904.638671875)
            }
        elseif ((Lv >= 1975 and Lv <= 1999) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Reborn Skeleton") then 
            return {
                [1] = "Reborn Skeleton [Lv. 1975]";
                [2] = "HauntedQuest1";
                [3] = 1;
                [4] = "Reborn Skeleton";
                [5] = CF(-9479.2168, 141.215088, 5566.09277);
                [6] = CF(-8763.7236328125, 165.72299194335938, 6159.86181640625)
            }
        elseif ((Lv >= 2000 and Lv <= 2024) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Living Zombie") then 
            return {
                [1] = "Living Zombie [Lv. 2000]";
                [2] = "HauntedQuest1";
                [3] = 2;
                [4] = "Living Zombie";
                [5] = CF(-9480.80762, 142.130661, 5566.37305);
                [6] = CF(-10103.7529, 238.565979, 6179.75977)
            }
        elseif ((Lv >= 2025 and Lv <= 2049) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Demonic Soul") then 
            return {
                [1] = "Demonic Soul [Lv. 2025]";
                [2] = "HauntedQuest2";
                [3] = 1;
                [4] = "Demonic Souls";
                [5] = CF(-9516.99316, 172.017181, 6078.46533);
                [6] = CF(-9709.30762, 204.695892, 6044.04688)
            }
        elseif ((Lv >= 2050 and Lv <= 2074) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Posessed Mummy") then 
            return {
                [1] = "Posessed Mummy [Lv. 2050]";
                [2] = "HauntedQuest2";
                [3] = 2;
                [4] = "Posessed Mummys";
                [5] = CF(-9515.39551, 172.266037, 6078.89746);
                [6] = CF(-9554.11035, 65.6141663, 6041.73584)
            }
        elseif ((Lv >= 2075 and Lv <= 2099) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Peanut Scout") then 
            return {
                [1] = "Peanut Scout [Lv. 2075]";
                [2] = "NutsIslandQuest";
                [3] = 1;
                [4] = "Peanut Scout";
                [5] = CF(-2104.453125, 38.129974365234, -10194.0078125);
                [6] = CF(-2068.0949707031, 76.512603759766, -10117.150390625)
            }
        elseif ((Lv >= 2100 and Lv <= 2124) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Peanut President") then 
            return {
                [1] = "Peanut President [Lv. 2100]";
                [2] = "NutsIslandQuest";
                [3] = 2;
                [4] = "Peanut President";
                [5] = CF(-2104.453125, 38.129974365234, -10194.0078125);
                [6] = CF(-2067.33203125, 90.557350158691, -10552.051757812)
            }
        elseif ((Lv >= 2125 and Lv <= 2149) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ice Cream Chef") then 
            return {
                [1] = "Ice Cream Chef [Lv. 2125]";
                [2] = "IceCreamIslandQuest";
                [3] = 1;
                [4] = "Ice Cream Chef";
                [5] = CF(-821.35913085938, 65.845329284668, -10965.2578125);
                [6] = CF(-796.37261962891, 110.95275878906, -10847.473632812)
            }
        elseif ((Lv >= 2150 and Lv <= 2200) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Ice Cream Commander") then 
            return {
                [1] = "Ice Cream Commander [Lv. 2150]";
                [2] = "IceCreamIslandQuest";
                [3] = 2;
                [4] = "Ice Cream Commander";
                [5] = CF(-821.35913085938, 65.845329284668, -10965.2578125);
                [6] = CF(-697.65338134766, 174.48368835449, -11218.38671875)
            }
        elseif ((Lv >= 2200 and Lv <= 2224) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Cookie Crafter") then 
            return {
                [1] = "Cookie Crafter [Lv. 2200]";
                [2] = "CakeQuest1";
                [3] = 1;
                [4] = "Cookie Crafter";
                [5] = CF(-2017.4874267578125, 36.85276412963867, -12027.53515625);
                [6] = CF(-2358.5791015625, 36.85615539550781, -12111.052734375)
            };
        elseif ((Lv >= 2225 and Lv <= 2249) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Cake Guard") then 
            return {
                [1] = "Cake Guard [Lv. 2225]";
                [2] = "CakeQuest1";
                [3] = 2;
                [4] = "Cake Guard";
                [5] = CF(-2021.32007, 37.7982254, -12028.7295);
                [6] = CF(-1598.3070068359375, 43.773197174072266, -12244.5810546875)
            };
        elseif ((Lv >= 2250 and Lv <= 2274) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Baking Staff") then 
            return {
                [1] = "Baking Staff [Lv. 2250]";
                [2] = "CakeQuest2";
                [3] = 1;
                [4] = "Baking Staff";
                [5] = CF(-1927.91602, 37.7981339, -12842.5391);
                [6] = CF(-1887.8099365234375, 77.6185073852539, -12998.3505859375)
            };
        elseif ((Lv >= 2275 and Lv <= 2299) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Head Baker") then 
            return {
                [1] = "Head Baker [Lv. 2275]";
                [2] = "CakeQuest2";
                [3] = 2;
                [4] = "Head Baker";
                [5] = CF(-1927.91602, 37.7981339, -12842.5391);
                [6] = CF(-2216.188232421875, 82.884521484375, -12869.2939453125)
            };
        elseif ((Lv >= 2300 and Lv <= 2324) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Cocoa Warrior") then 
            return {
                [1] = "Cocoa Warrior [Lv. 2300]";
                [2] = "ChocQuest1";
                [3] = 1;
                [4] = "Cocoa Warrior";
                [5] = CF(233.22836303710938, 29.876001358032227, -12201.2333984375);
                [6] = CF(-21.55328369140625, 80.57499694824219, -12352.3876953125)
            };
        elseif ((Lv >= 2325 and Lv <= 2349) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Chocolate Bar Battler") then 
            return {
                [1] = "Chocolate Bar Battler [Lv. 2325]";
                [2] = "ChocQuest1";
                [3] = 2;
                [4] = "Chocolate Bar Battler";
                [5] = CF(233.22836303710938, 29.876001358032227, -12201.2333984375);
                [6] = CF(582.590576171875, 77.18809509277344, -12463.162109375)
            };
        elseif ((Lv >= 2350 and Lv <= 2374) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Sweet Thief") then 
            return {
                [1] = "Sweet Thief [Lv. 2350]";
                [2] = "ChocQuest2";
                [3] = 1;
                [4] = "Sweet Thief";
                [5] = CF(150.5066375732422, 30.693693161010742, -12774.5029296875);
                [6] = CF(165.1884765625, 76.05885314941406, -12600.8369140625)
            };
        elseif ((Lv >= 2375 and Lv <= 2399) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Candy Rebel") then 
            return {
                [1] = "Candy Rebel [Lv. 2375]";
                [2] = "ChocQuest2";
                [3] = 2;
                [4] = "Candy Rebel";
                [5] = CF(150.5066375732422, 30.693693161010742, -12774.5029296875);
                [6] = CF(134.86563110351562, 77.2476806640625, -12876.5478515625)
            };
        elseif ((Lv >= 2400 and Lv <= 2424) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Candy Pirate") then 
            return {
                [1] = "Candy Pirate [Lv. 2400]";
                [2] = "CandyQuest1";
                [3] = 1;
                [4] = "Candy Pirate";
                [5] = CF(-1150.0400390625, 20.378934860229492, -14446.3349609375);
                [6] = CF(-1310.5003662109375, 26.016523361206055, -14562.404296875)
            };
        elseif ((Lv >= 2425 and Lv <= 2449) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Snow Demon") then 
            return {
                [1] = "Snow Demon [Lv. 2449]";
                [2] = "CandyQuest1";
                [3] = 2;
                [4] = "Snow Demon";
                [5] = CF(-1150.0400390625, 20.378934860229492, -14446.3349609375);
                [6] = CF(-880.2006225585938, 71.24776458740234, -14538.609375)
            };
        elseif ((Lv >= 2450 and Lv <= 2474) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Isle Outlaw") then 
            return {
                [1] = "Isle Outlaw [Lv. 2450]";
                [2] = "TikiQuest1";
                [3] = 1;
                [4] = "Isle Outlaw";
                [5] = CF(-16547.748046875, 61.13533401489258, -173.41360473632812);
                [6] = CF(-16442.814453125, 116.13899993896484, -264.4637756347656)
            };
        elseif ((Lv >= 2475 and Lv <= 2524) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Island Boy") then 
            return {
                [1] = "Island Boy [Lv. 2475]";
                [2] = "TikiQuest1";
                [3] = 2;
                [4] = "Island Boy";
                [5] = CF(-16547.748046875, 61.13533401489258, -173.41360473632812);
                [6] = CF(-16901.26171875, 84.06756591796875, -192.88906860351562)
            };
        elseif ((Lv >= 2525 and Lv <= 2550) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Isle Champion") then 
            return {
                [1] = "Isle Champion [Lv. 2525]";
                [2] = "TikiQuest2";
                [3] = 2;
                [4] = "Isle Champion";
                [5] = CF(-16539.078125, 55.68632888793945, 1051.5738525390625);
                [6] = CF(-16641.6796875, 235.7825469970703, 1031.282958984375)
            };
        elseif ((Lv >= 2550 and Lv <= 2575) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Isle Champion") then 
            return {
                [1] = "Isle Champion [Lv. 2525]";
                [2] = "TikiQuest2";
                [3] = 2;
                [4] = "Isle Champion";
                [5] = CF(-16539.078125, 55.68632888793945, 1051.5738525390625);
                [6] = CF(-16641.6796875, 235.7825469970703, 1031.282958984375)
            };
        elseif ((Lv >= 2575 and Lv <= 2600) and not Configs.System.Selected_Mob.Auto) or (Configs.System.Selected_Mob.Auto and Configs.System.Selected_Mob.Obj == "Isle Champion") then 
            return {
                [1] = "Isle Champion [Lv. 2550]";
                [2] = "TikiQuest2";
                [3] = 2;
                [4] = "Isle Champion";
                [5] = CF(-16539.078125, 55.68632888793945, 1051.5738525390625);
                [6] = CF(-16641.6796875, 235.7825469970703, 1031.282958984375)
            };
        end;
    end;
end;

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
