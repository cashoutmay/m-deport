## May Deport
This resource is made by `may2high` on discord. We perserve all rights to this resource and if caught exporting this resource or stealing it you will be delt with by the law. We do not accept any thefts.

https://www.youtube.com/watch?v=G0Ck1_bT7GI

# Dependencies [interact-sound](https://github.com/plunkettscott/interact-sound) & [ox_lib](https://github.com/overextended/ox_lib)
## Don't change the resource name ## 

**may-deport** Is a player management script that allows authorized users to deport players to a specified location by default it is Cayo Perico.
This resource supports ACE Permissions, Sound Effects, Input Dialogs, NativeUI Integration, and Discord Logging. 

## Installation
1. Place May deport inside your script folder
2. Make sure you also have these resources installed
    - ox_lib
    - interact-sound
3. Add the resources and start them
## Refrence below    
ensure May-Deport
ensure ox_lib
ensure interact-sound

## Sound Config
1. Make sure you have a sound file with the *.ogg*
2. Go to interact sound folder and follow these steps
    - Client -> html --> sounds
3. Place the file in the sounds folder and go back to the config in the **may-deport**    
4. Keep or change the sound file below *Sound settings*

## Ace Permissions
Only players with the ACE `deport.player` can deport if `Config.UseAce` is true.
If ACE is disabled, all players can use the deport function.

add_ace group.admin deport.player allow

## Exporting
*/deport [player id]*
By default the chat command is on. If you wish to use the export instead of the chat command disable the command in the settings.

exports['may-Deport']:DeportPlayer()

With the exporting inside of menus it wil open our own *Input Dialog* to enter to players id which is supported by ox_lib.
Here is an example below using it inside of a *NativeUI* menu.

               local deport = NativeUI.CreateItem('Deport', 'Deports player to cayo perico') 
                LEOMenu:AddItem(deport)
                depot.Activated = function(ParentMenu, SelectedItem)
                        exports['may-deport']:DeportPlayer()
                end

## Webhooks
1. Add your webhook inside of *sv_config*
2. When a player is deported it will show
    - Players Name:
    - Officers Name:
    - Date:

## Tips 
Make sure sound matches inside of the sound settings in `config`
Check that ox_lib is running to make sure there is 0 errors with notifications and input dialog
If the players are not getting deported, make sure the ACE Perms are good and then check the player ID again
If you seem to still have any issues please contact on via discord `may2high` for more help.
