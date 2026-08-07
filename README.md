# RaidSummon

> **This is a fork** of [isitLoVe/RaidSummon](https://github.com/isitLoVe/RaidSummon) with fixes for the current Classic Era client, pending review upstream ([PR #63](https://github.com/isitLoVe/RaidSummon/pull/63), [PR #64](https://github.com/isitLoVe/RaidSummon/pull/64)). If you just want the original addon, use the Download link below instead.
>
> **What's fixed here that isn't in the upstream release yet:**
> - **Summon/target buttons working again** — after a recent client update, left-click-to-target and right-click-to-summon on the name list silently stopped doing anything (no error, just nothing happened). Root cause was two separate bugs: the addon was resolving the wrong in-game unit for a given raid member in some raid compositions, and the button template it used to fire the click action (`SecureActionButtonTemplate`) stopped dispatching correctly on the current client — swapped to `SecureUnitButtonTemplate`, which works.
> - **New: Auto-Remove In Range** — queued players are now automatically dropped from the summon list once they're already close enough to you (e.g. they walked there, got a portal, or someone else summoned them), so you don't waste time/mana summoning someone who doesn't need it. On by default, toggle it off in `/rs config` if you don't want it.
>
> To use this fork: download this repo's `RaidSummon` folder into your `Interface/AddOns` folder the same way you would the original.

## Download
https://www.curseforge.com/wow/addons/raidsummon

## Classic Season of Discovery
Guess im in for the fun, stay tuned for updates and donate ;)  

## Usage
Raidmembers can type a special keyword in the raidchat (123, summon, sum or port)  
Their names will be added to the summon list and syned to all warlocks using the addon  
The name can be left clicked to target the raidmember  
CTRL+left click to remove a member from the list (synced - name will be removed from all addon users)  
Finally summon the member with right click and send a message to the raid / whisper (member will be removed from the list - synced)  
Drag the frame by holding SHIFT+left click  
![RaidSummon Frame](https://raw.githubusercontent.com/isitLoVe/RaidSummon/master/pics/RaidSummon_Frame.PNG)
![RaidSummon RightClick](https://raw.githubusercontent.com/isitLoVe/RaidSummon/master/pics/RaidSummon_RightClick.PNG)
![RaidSummon Whisper](https://raw.githubusercontent.com/isitLoVe/RaidSummon/master/pics/RaidSummon_Whisper.PNG)

## Configuration
Open the configuration menu with /rs config or /raidsummon config or via the addon menu  
![RaidSummon Help](https://raw.githubusercontent.com/isitLoVe/RaidSummon/master/pics/RaidSummon_Help.PNG)

## Combat Lockdown
Due to Blizzard restrictions it is not possible to update the summon frame during combat, however after leaving combat it may take up to 10 seconds for the name to be displayed.

## Bugs
Please report any bugs to my GitHub site at https://github.com/isitLoVe/RaidSummon/issues

## Support RaidSummon development
If you want new features or are able to code a nicer interface, (FrameXML) feel free to send a pull request via Github.  
I am not a full time developer. It is either play the game or try to add new features to the addon (guess the priority :D).  
[![paypal](https://www.paypalobjects.com/en_US/DK/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate?hosted_button_id=EV2ARKPS8G2DW)
