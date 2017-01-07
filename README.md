SWTOR-scripts
=============

Enjoy the scripts!

This is where my scripts will go which I make for the Star Wars: The Old Republic game :)

All you need to do is run the exes here which I have converted from the AHK files.

The AHK files are here too of course, so you can look through those or convert them to EXE's yourself if you like.

You might not trust me enough to just download the exe, but I can guarantee you it is safe and I'm a genuinely nice guy :) Your other option is to download the 'ahk' file type instead, but you'll also need to download and install the "AutoHotKey" program (also safe! Look it up).

Snowballs
=============

Use Snowballs script when you're just the right distance between your
companion to use the throw snowball ability, and have clicked on them. I use CTRL+SHIFT+4 to throw snowballs and that's what the script sends. Make sure to run this a little while till you get your first Snow Parcel, then drag the window down so the Accept button is right where the debuff icon is. Windows b starts the script loop, and Windows n pauses it.

Have fun racking up those snow parcels and Happy Life Day! ^^

If you understand some coding, here's the source file's code:

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

Simple isn't it? :)
