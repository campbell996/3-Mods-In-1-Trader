# 3-Mods-In-1.-Trader-Master
This Download Includes.    @6x6 All Terrain Vehicle > @Ivory Car Pack [Official] > @RKSL Studios-LCVP Mk5 Landing Craft 

This Installation Requires 3 Mods:
1. https://steamcommunity.com/sharedfiles/filedetails/?id=1888644057
2. https://steamcommunity.com/sharedfiles/filedetails/?id=1190934425
3. https://steamcommunity.com/sharedfiles/filedetails/?id=1752496126 
  
This File Is Better To Read In Notepad++. 

This is the Exile trader files for > @6x6AllTerrainVehicle <> @IvoryCarPack[Official] <> @RKSLStudios-LCVPMk5LandingCraft <
DOWNLOAD>>>>> https://github.com/campbell996/3-Mods-In-1-Trader-Master <<<<< DOWNLOAD
 
I Did Not create These Mods. But I Did Create These Trader Files. 

INSTALLATION 

Step 1. Using pbo manager extract your mission.pbo & enter the mission folder that is extracted.   http://www.armaholic.com/page.php?id=16369 

Step 2. Create a folder called >>>>> traders <<<<<. Continue on step 3. 

Step 3. Place the >>>>> 3IN1 <<<<< folder that comes with this download. In the traders folder from step 2. 

Step 4. Open your >>>>> config.cpp <<<<< file using notepad++. Continue on step 5. 

Step 5. Find >>>>> class CfgExileArsenal <<<<< and add this at the top >>>>> #include "traders\3IN1\ItemList3IN1.hpp" <<<<<.

Step 5 Example

This is what it is before.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
class CfgExileArsenal
{
 class Exile_Uniform_BambiOverall    { quality = 1; price = 1; sellPrice = 1; };
 ///////////////////////////////////////////////////////////////////////////////
 // Civillian Clothing
 ///////////////////////////////////////////////////////////////////////////////
 class U_C_Journalist        { quality = 1; price = 20; };
 class U_C_Poloshirt_blue       { quality = 1; price = 20; };
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

And this is what it should be after...

class CfgExileArsenal
{
 #include "traders\3IN1\ItemList3IN1.hpp"
 class Exile_Uniform_BambiOverall    { quality = 1; price = 1; sellPrice = 1; };
 ///////////////////////////////////////////////////////////////////////////////
 // Civillian Clothing
 ///////////////////////////////////////////////////////////////////////////////
 class U_C_Journalist        { quality = 1; price = 20; };
 class U_C_Poloshirt_blue       { quality = 1; price = 20; };
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
 
 
Step 6. Find >>>>> class CfgTraderCategories <<<<< and add this at the top >>>>> #include "traders\3IN1\TraderCategories3IN1.hpp" <<<<<.

Step 6 Example

This is what it is before.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
class CfgTraderCategories
{
 class Community
 {
  name = "Community Items";
  icon = "a3\ui_f\data\gui\Rsc\RscDisplayArsenal\uniform_ca.paa";
  items[] =
  {
 
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

And this is what it should be after.

class CfgTraderCategories
{
 #include "traders\3IN1\TraderCategories3IN1.hpp"
 class Community
 {
  name = "Community Items";
  icon = "a3\ui_f\data\gui\Rsc\RscDisplayArsenal\uniform_ca.paa";
  items[] =
  {
 
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 

Step 7. Find >>>>> class CfgTraders <<<<< And in that Find >>>>> class Exile_Trader_Vehicle <<<<<

and add all 6 of these >>>>> >"AllTerrainVehicles",<>"IvoryCars",<>"IvoryMarkedPoliceCars",<>"IvoryUnmarkedPoliceCars",<>"IvorySlicktopPoliceCars",<>"IvoryTaxis"< <<<<<. 

Step 7 Example

This is what it is before.

////////////////////////////////////////////////////////////////////
class Exile_Trader_Vehicle
 {
  name = "VEHICLE";
  showWeaponFilter = 0;
  categories[] =
  {
   "Cars",
   "Trucks"
  };
 };
////////////////////////////////////////////////////////////////////

And this is what it should be after...   Dont forget the last catrgory cant have a > , <   but the rest must.

class Exile_Trader_Vehicle
 {
  name = "VEHICLE";
  showWeaponFilter = 0;
  categories[] =
  {
   "Cars",
   "Trucks",
   "AllTerrainVehicles",
   "IvoryCars",
   "IvoryMarkedPoliceCars",
   "IvoryUnmarkedPoliceCars",
   "IvorySlicktopPoliceCars",
   "IvoryTaxis"
  };
 };
////////////////////////////////////////////////////////////////////// 

Step 8. Find >>>>> class CfgTraders <<<<< And in that Find >>>>> class Exile_Trader_Boat <<<<<
and add this >>>>> > "Mk5Crafts" <<<<< Same as above example. except in the >>>>> class Exile_Trader_Boat <<<<<. 

Step 9. Download All 3 Of These Mods >>>>> @6x6 All Terrain Vehicle <> @Ivory Car Pack [Official] <> @RKSL Studios-LCVP Mk5 Landing Craft <<<<< from either the A3Launcher or from the Steam Workshop.
 
Step 10. Copy All 3 Of The Mods You Just Downloaded And Add Them To Your Exile Server Root Folder. And Remove All Spacing In The Folders Names.

Step 10 Example      BEFORE: @RKSL Studios-LCVP Mk5 Landing Craft   AFTER: @RKSLStudios-LCVPMk5LandingCraft
 
Step 11. Add the Bikey's to your server keys folder. If Required.
 
Step 12. Add >>>>> @6x6AllTerrainVehicle;@IvoryCarPack[Official];@RKSLStudios-LCVPMk5LandingCraft <<<<< to your server start parameter. 

Note. All the IvoryCars may show in the trader as full black paintjobs Even the police and taxi liviries. But once you purchase/spawn them they will have there intended liveries.

Enjoy........
