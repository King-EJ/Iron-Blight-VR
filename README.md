# Iron-Blight-VR
VR mod for Iron Blight

<img width="448" height="442" alt="Adobe" src="https://github.com/user-attachments/assets/e9a790b9-a52c-473c-81b5-149531cf32e4" />


IRON BLIGHT VR  -  VR mod for "Iron Blight" (Unity 6000.3, IL2CPP, URP)
=======================================================================

Version 0.1.16 (test build on Quest 3 VDXR).

WHAT IT DOES
------------
* Stereo VR through OpenXR (SteamVR, Meta/Oculus, Virtual Desktop, WMR...).
* You are the player: look around with your head (the game looks where you look), the left stick
  walks where you look, the right stick snap turns. The view rides on the game's camera.
* The gun is in your right hand and fires where you point it (a red laser shows where).
  The flashlight is in your left hand. Using / picking up goes by where you look.
* The VR controllers act as a gamepad for the game's own controls and menus.
* The HUD and menus are on a screen floating in front of you. Head bob is switched off.

INSTALL
-------
1.  unzip into the game folder.
3. Start SteamVR (or your OpenXR runtime), then start the game.

CONTROLS
--------
Left stick ............... walk (toward where you look; LeftStickAsWASD = true for W A S D keys)

Hold left grip + left stick up / right / left ... keys 1 / 2 / 3 (quick slots)

Hold left grip + B ....... M key            Hold left grip + A ..... J key

Right trigger ............ fire (RT)            Right grip ......... aim (LT)

Right stick left/right ... turn                 Right stick up ..... F key

Right stick down ......... RB                   Right stick click .. Q key

Left trigger ............. RB (same as right stick down)

A (tap) .................. A                    Hold A ............. X key

B ........................ B                    X (tap) ............ X button

Y (tap) .................. Space key            Hold Y ............. laser on / off

X + Y together ........... pause (Start)        Hold X ............. Back / View

Left stick click ......... L3                   Both stick clicks .. re-centre

Everything is in BepInEx\config\ironblight.vr.cfg: [Controls] = gamepad buttons, [KeyControls] = keyboard keys.

<img width="1519" height="1036" alt="3cd2e622-fc8f-41f1-b4b4-348ec259ab51" src="https://github.com/user-attachments/assets/0de6fe49-e96f-48c7-964f-9e2f6a44612a" />



MENUS:                  point your right hand at the menu screen - a blue laser shows where -
                        and pull the trigger to click.

                      
BACKPACK:               Xbox gamepad controls (sticks / d-pad move, A select, B back ...), no laser.
                        [Input] BackpackPointer = true brings the point-and-click laser back.
                        
LASER SIGHT:            shows while you hold the right grip (aim) - [Weapons] LaserButton.

NOTES / JOURNAL:        a note you read is shown on the VR screen, like the flat game shows it.
                        Point the blue laser at the note and pull the trigger: right half = next page,
                        left half = previous page. Put it away with X+Y .
                        Only the paper is shown ([Notes] NoteShowClipboard = true adds the clipboard).
                        [Notes] NoteLight = brightness of the note (it gets its own light).
                        
MAP:                    the map is held in your left hand while it is open, facing you.
                        [Map] MapScale = size (changes live), MapOffset = where it sits, MapRotation.
                        In game: map open, hold the right stick click 1.7 s (buzz), then right grip = grab
                        the map and move / turn it, right stick up / down = size, B = default,
                        A (or R3 1.7 s again) = done. Saved as you go.
                        
BIKE:                   cant turn to adjust your body position on bike so interact with bike from rear tire to be in correct position
                       
LASER ADJUST:           hold BOTH grips for 1.7 s with a gun in hand (buzz), let go, then:
                        left grip = grab the yellow start point and put it on the barrel,
                        right stick = steer the laser end, right grip = keep the laser pointing
                        where it points while you turn the gun, B = default,
                        A (or both grips 1.7 s again) = save for this gun. Shots follow the laser.
                        
ARMS:                   the game's arms are hidden on every gun ([Weapons] HideArms).

IN-GAME SETTINGS MENU:  hold Y + left stick click for 1.7 s.

WEAPON PLACEMENT:       hold both stick clicks for 2 s (left grip = grab & move, right stick = size, A = save).

HAND ADJUST:            hold Y + right stick click for 1.5 s.

Issues 
--------------------------------
- Main menu float in front of you so just aim right controller and if you see the word on building to select even if you not looking at building
- cant turn to adjust your body position on bike so interact with bike from rear tire to be in correct position
- sprinting animation or reloading animation weapon will leave your hand
- cant see whats selected on gun mod in backpack just move left stick and press A to attach or remove gun mod

Uses Astien's OpenXR bridge (see BepInEx\plugins\IBVR\LICENSES). Free, non-commercial.
