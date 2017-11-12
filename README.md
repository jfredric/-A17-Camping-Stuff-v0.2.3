# -A17-Camping-Stuff-v0.2.3
Nandonalt's Camping Stuff v0.2.3 updated to a17
Sourced from steam with the following changes:

### Installation Instructions
To install a non-workshop RimWorld mod from zip download:
1. Click on the **Clone or download** button.
2. Click **Download ZIP**
3. Open the zip file
4. Go to your RimWorld install folder (by windows default its C:\Program Files (x86)\Steam\steamapps\common\RimWorld) and open the "Mods" folder.
5. Copy the folder from the zip file to the Mods folder (DO NOT put it inside Core)
6. After that run Rimworld and "Camping Stuff" will show up in your mod list (again) with a little folder icon next to it.
7. From there it should be just like any other workshop item

To install using git:
1. Click on the **Clone or download** button.
2. Copy the url (https://github.com/Alias44/-A17-Camping-Stuff-v0.2.3.git)
3. Open your preferred console (cmd, bash, etc).
4. cd into the mods directory. Default is C:\Program Files (x86)\Steam\steamapps\common\RimWorld\Mods
5. Enter the command **git clone https://github.com/Alias44/-A17-Camping-Stuff-v0.2.3.git**

 Note: You can get future changes by using the command **get pull origin master**


### Changes
Initial changes From Nandonalt's last version
* Removed the references to Microsoft.CSharp and System.Net.Http and setting .net target to 3.5 (these may just be my visual studio adding stuff on me)
* Changed 'stringToLines' to 'StringToLines' on CompTargetable_Tent.cs lines 53 & 195
* Changed 'getPlacements' to 'GetPlacements' on CompTargetable_Tent.cs lines 191, 306, & 530 and CompPackTents.cs line 93
* Added a '-1,' to CompTargetable_Tent.cs line 446 so it reads: return GenClosest.ClosestThingReachable(pawn.Position, pawn.Map, ThingRequest.ForDef(this.parent.Stuff), PathEndMode.InteractionCell, TraverseParms.For(pawn, pawn.NormalMaxDanger(), TraverseMode.ByPawn, false), 9999f, validator, null, -1, -1, false);
* Changed 'Scribe_Values.LookValue' to 'Scribe_Values.Look' on CompPackTent.cs lines 64 & 65
* Deleted CompPackTent.cs lines 179-204
* Changed CompPackTent.cs lines 153-164 to:
  nodoor = false;
  thingList2[i].Destroy(DestroyMode.Vanish);

### Licensing
Unsure of licensing info, as Nandonalt didn't originally publish anything in that respect.
