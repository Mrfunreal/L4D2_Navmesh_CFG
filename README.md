### L4D2 Navmesh Edit CFG set
This set of CFG files will make navmesh editing in L4D2 easier.
It contains pre-bound commands for selecting, editing, drawing lowering/raising and otherwise altering navmesh. As well as a file to toggle Population editing and assigning places easier.

Check ``!Navmesh`` and ``!NavPopulationEditToggle`` to see the accumulated commands and their assigned keybinds.<br>
Each command has an explanation on what it does. You can also change the keybinds if you want.

### Install
<details>
<summary>Click me to expand instructions</summary>

1. Download and unpack this repo into ```steamapps\common\Left 4 Dead 2\left4dead2\cfg```.
2. Create an autoexec file file called ```exec.cfg``` in ```steamapps\common\Left 4 Dead 2\left4dead2\cfg``` containing the following:<br>
```
bind home "exec L4D2_Navmesh_CFG-main/!NavPopulationEditToggle"  //Bind Home to population edit mode.
bind pgup "exec L4D2_Navmesh_CFG-main/!Navmesh"                  //Bind PageUp to enable navmesh mode.
bind pgdn "exec L4D2_Navmesh_CFG-main/!Navmesh_undo"             //Bind PageDown to disable navmesh mode.
echo "Write new config using: host_writeconfig 	!navundo_defaultbinds.cfg"
```
You can edit the keybinds if you want. I just happen to not use these keys for anything yet.<br>
  
⚠️ **Warning:** !Navmesh.cfg writes a config file based on your current settings in order to not overwrite your keybinds. But this includes all settings like resolution, volume, FOV, ect.<br>
    If you ever change your settings, you should run ``host_writeconfig !navundo_defaultbinds.cfg`` to make sure toggling navmesh edit mode won't revert your settings.
  
3. add ```exec !exec.cfg``` to your launch options.
<img src="pictures/exec.jpg"/>
</details>
