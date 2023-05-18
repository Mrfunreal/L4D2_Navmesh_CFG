# L4D2_Navmesh_CFG
This set of CFG files will make navmesh editing in L4D2 easier.
It contains a lot of keybinds for selecting navmesh, drawing navmesh, lowering it, raising it, ect.


To use this set, you will first need to create an autoexec.cfg which will automatically load the cfg on game launch.
- For this, add **+exec !exec.cfg** to your launch options.

bind home "exec L4D2_Navmesh_CFG/!!NavPopulationEditOn"
bind pgup "exec L4D2_Navmesh_CFG/!Navmesh"
bind pgdn "exec L4D2_Navmesh_CFG/!Navmesh_undo"
