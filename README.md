# DragRace
This is Edgar Mao’s project of simulating a quarter mile drag race with self-designed cars based on a preset parameter, and eventually producing the time it take for the descend car to finish the race.

Parameters:
#Engine##########

	LS3 (Corvette)
		Id=LS3
		Dyno
			BestFitCubic (rpm,hp)
				[(1750,100), (3100,200), (4300,300), (6000,390), (6500,370)]
			Weight
				195kg

	Hemi Apache (Challenger)
		Id=HA
		Dyno
			BestFitCubic (rpm,hp)
				[(1000,200), (2000,350), (4000,350), (4400,400), (4950,450), (5350,500), (6250,530), (7100,500)]
			Weight
				318 kg

	5.OL GT (Mustang)
		Id=GT
		Dyno
			BestFitCubic (rpm,hp)
				[(1000,50), (2000,100), (3200,200), (4200,300), (5100,350), (6500,395)]
		Weight
			201 kg

#Transmission########

	Borg-Warnder T56
		GearRatios=(1:2.97, 2:1.94, 3:1.35, 4:1.00, 5:0.84, 6:0.62, -1:3.38)

#Differential########

	Differential Ratio
		3.83:1

#Spoiler#############

	Coefficient of Lift
		Wind Tunnel
			BestFitCubic (degrees,C1)
				[(0,0), (5,-0.4), (10,-0.8), (13,-1.0), (15,-0.9), (20,-0.85)]

	Coefficient of Drag
		Wind Tunnel
			BestFitCubic (degrees,Cd)
				[(5,0.035), (10,0.07), (15,0.16), (17,0.23), (20,0.33)]

#Specifications#######
	1. The front tire cannot leave the ground.
	2. The car in the simulation will be driven perfectly with no tire slipping.
	3. Your tire and wheel size must be commerically avaliable.
	4. Wheelbases are from 3.0m-4.0m
	5. Car lengths are from 4.5m-5.5m
	6. Distance from bumper to axle maybe 0.5m-1.5m
	7. The engine may be 0.5m-2.0m from the front bumper or 0.5m-2.0m from the rear bumper.
	8. The engine position is measured from the front of the car.
	9. You must choose one of the given engines.
	10. The horse power will be determined by a cubic fit to the given data.
	11. The angle of attack for the spoiler may take values 0-25 degrees.
	12. You may only change the variable parameters.
	13. The spoiler must be at the end of the car 1m above the axel.
	14. The height of the center of mass if the car body will be at the same as the engine and 0.2cm above the axels.
