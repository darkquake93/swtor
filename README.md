Darkquake's SWTOR Scripts
=========================

Enjoy the scripts!

Proper page with a sexy theme: https://darkquake93.github.io/swtor/
[Donations welcome ;)](https://twitch.streamlabs.com/darkness9t3/)

This is where my scripts will go which I make for the Star Wars: The Old Republic game :)

All you need to do is run the exes here which I have converted from the AHK files.

The AHK files are here too of course, so you can look through those or convert them to EXE's yourself if you like.

You might not trust me enough to just download the exe, but I can guarantee you it is safe and I'm a genuinely nice guy :) Your other option is to download the 'ahk' file type instead, but you'll also need to download and install the "AutoHotKey" program (also safe! Look it up).

The hashes in the scripts represent the Windows key, so this means something like #b:: means the code after that line will be executed when Windows+b is pressed.

Snowballs
=============

Use Snowballs script when you're just the right distance between your
companion to use the throw snowball ability, and have clicked on them. I use CTRL+SHIFT+4 to throw snowballs and that's what the script sends. Make sure to run this a little while till you get your first Snow Parcel, then drag the window down so the Accept button is right where the debuff icon is. Windows+b will start the script loop, and Windows+n will pause it.

Have fun racking up those snow parcels and Happy Life Day! ^^

If you understand some coding, here's the source file's code:

```
#b::
Loop
{
MouseMove, 1403, 827
MouseClick
Sleep 250
MouseClick,right
Sleep 250
Send ^+4
Sleep 15500
} 
#n::Pause
```
Simple isn't it? :) 

Get Mouse Pos
=============

As the name implies, retrieve the mouse's current position. Press Windows+z to display what the position is. I made this just to be able to finetune what position the Snowball script sends the cursor to, so if it's moving the cursor to the wrong place you may be on the wrong resolution and need to edit the ahk file. Windows+z reports the position.

Source Code:

```
#z::
MouseGetPos, xpos, ypos 
Msgbox, The cursor is at X%xpos% Y%ypos%.
```
WTS - Snow Parcels
=============

This is a script with a custom message to sell those parcels, given the prices change all the time plus you may want to say something different. Check it out if you want, but you will definitely need Autohotkey if you want to change this to your liking. With the mouse cursor hovering over the Snow Parcel item in your inventory, just press Windows+i and the script will do the rest. You can choose to send the message right away if you include the Send {Enter} line at the end.

Source Code:

```
ShiftClick()
{
Send {Shift down}
MouseClick
Send {Shift up}
}
#i::
Send /3{Space}
Send WTS 1600x
Sleep 500
ShiftClick()
Send, ,
Send {Space}
Send 99x
Sleep 500
ShiftClick()
Send {Space}for 300k. /W me :)
;Send {Enter}
;Remember to look into coordinates for clicking, it would make this script a lot better!
```
AutoNightlife
=============

Tired of repeatedly right-clicking on those slot machines? Look no further! This script will simply keep right clicking, saving you the hassle and increasing your chances of winning (since you'll technically "be there" right-clicking on one computer while gaming on the other, or simply having this running while you sleep!) Windows+t starts the script loop and Windows+o pauses it.

Source Code:

```
#t::
Loop
{
MouseClick,right
Sleep 500
} 
#o::Pause
```
