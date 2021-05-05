This tutorials will help those beginners who wanted to start his career in image processing 


#include<iostream>
#include<vector>
#include<map>
#include<time.h>


std::vector<std::string> labels = {
	"Berkin-PowerBank10K","EchoShow","Google-NestHellow","JBL-Flip5","JBL-LinkMusic","Mophie-DualWirelessChargingPad",
	"Mophie-UVSanitizer","Mophie-WirelessCharginPad","Morphie-4in1wirelesschargingmat","Nimble-WirelessPad","Otter-Commuter",
	"Otter-Googlepixel4a","Samsung-GalaxyA51","Samsung-GalaxyNote205G","Samsung-GalaxyNote20Ultra5G","Samsung-GalaxyS20FE5G",
	"Samsung-GalaxyS20Plus5G","Samsung-GalaxyS20Ultra5G","Samsung-GalaxyTabA","Samsung-TabS75G","Verizon-10KPortablePowerPack",
	"Verizon-5PortChargingHub","Verizon-CarAdapterFastCharger","Verizon-CarChargerFastCharger","Verizon-ChargerComboUSBC",
	"Verizon-ChargingCableBlack","Verizon-ChargingCableBlue","Verizon-ChargingCableForApple","Verizon-ChargingCablePink",
	"Verizon-WallAdapter45GaNUSBCFastCharger","Verizon-WirelessChargingPadFastCharger2Pack","iPad-8thGeneration",
	"iPhone-11Green","iPhone-11ProMidnightGreen","iPhone-12MiniGreen","iPhone-12ProMaxPacificBlue","iPhone-SEWhite",
	"iPhone-XRCoral" };

std::map<std::int8_t, std::int8_t> tree_map = { { 0,-1 },{ 1,-1 },{ 2,-1 },{ 3,-1 },{ 4,-1 },{ 5,-1 },{ 6,-1 },{ 7,-1 },{ 8,-1 },{ 9,-1 },{ 10,-1 },
{ 11,-1 },{ 12,-1 },{ 13,-1 },{ 14,-1 },{ 15,-1 },{ 16,-1 },{ 17,-1 },{ 18,-1 },{ 19,-1 },{ 20,-1 },{ 21,-1 },{ 22,-1 },{ 23,3 },{ 24,3 },{ 25,4 },
{ 26,4 },{ 27,4 },{ 28,4 },{ 29,9 },{ 30,9 },{ 31,10 },{ 32,10 },{ 33,10 },{ 34,15 },{ 35,15 },{ 36,15 },{ 37,15 },{ 38,16 },{ 39,16 },{ 40,16 },{ 41,16 },
{ 42,19 },{ 43,19 },{ 44,20 },{ 45,20 }
};

std::map<std::int8_t, std::string> unit_map = {
	{ 0,"Berkin-PowerBank10K" },{ 1,"EchoShow" },{ 2,"Google-NestHellow" },{ 3,"JBL-Speakers" },{ 4,"Mophie-WirelessCharginPad" },{ 5,"Mophie-DualWirelessChargingPad" },
	{ 5,"Nimble-WirelessPad" },{ 6,"Otter-Commuter" },{ 7,"Otter-Googlepixel4a" },{ 8,"Samsung-GalaxyA51" },{ 9,"Samsung-GalaxyNote205G" },{ 10,"Samsung-GalaxyS20" },{ 11,"Samsung-GalaxyTabA" },
	{ 12,"Samsung-TabS75G" },{ 13,"Verizon-10KPortablePowerPack" },{ 14,"Verizon-5PortChargingHub" },{ 15,"Verizon-AdapterNChargers" },{ 16,"Verizon-ChargingCables" },
	{ 17,"Verizon-WirelessChargingPadFastCharger2Pack" },{ 18,"iPad-8thGeneration" },{ 19,"iPhone-11" },{ 20,"iPhone-12" },{ 21,"iPhone-SEWhite" },{ 22,"iPhone-XRCoral" },
	{ 23,"JBL-Flip5" },{ 24,"JBL-LinkMusic" },{ 25,"Morphie-DualWirelessChargingPad" },{ 26,"Mophie-UVSanitizer" },{ 27,"Mophie-WirelessChargingPad" },{ 28,"Morphie-4in1Wirelesschargingmat" },
	{ 29,"Samsung-GalaxyNote205G" },{ 30,"Samsung-GalaxyNote20Ultra5G" },{ 31,"Samsung-GalaxyS20FE5G" },{ 32,"Samsung-GalaxyS20Plus5G" },{ 33,"Samsung-GalaxyS20Ultra5G" },
	{ 34,"Verizon-CarAdapterFastCharger" },{ 35,"Verizon-CarChargerFastCharger" },{ 36,"Verizon-ChargerComboUSBC" },{ 37,"Verizon-WallAdapter45GaNUSBCFastCharger" },{ 38,"Verizon-ChargingCableBlack" },
	{ 39,"Verizon-ChargingCableBlue" },{ 40,"Verizon-ChargingCableForApple" },{ 41,"Verizon-ChargingCablePink" },{ 42,"iPhone-11Green" },{ 43,"iPhone-11ProMidnightGreen" },
	{ 44,"iPhone-12MiniGreen" },{ 45,"iPhone-12ProMaxPacificBlue" }
};
