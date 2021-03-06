---------------------------------------------------------------------------------
-- 
-- Arcade: DigDug  port to MiSTer by MiSTer-X
-- 21 September 2019
-- From: https://github.com/MrX-8B/MiSTer-Arcade-DigDug
--
---------------------------------------------------------------------------------
-- FPGA DigDug for XILINX Spartan-6
------------------------------------------------
-- Copyright (c) 2017 MiSTer-X
---------------------------------------------------------------------------------
-- T80/T80s - Version : 0242
-----------------------------
-- TV80 8-Bit Microprocessor Core
-- Based on the VHDL T80 core by Daniel Wallner (jesus@opencores.org)
--
-- Copyright (c) 2004 Guy Hutchison (ghutchis@opencores.org)
---------------------------------------------------------------------------------
-- 
-- 
-- Keyboard inputs :
--
--   F2          : Coin + Start 2 players
--   F1          : Coin + Start 1 player
--   UP,DOWN,LEFT,RIGHT arrows : Movements
--   SPACE/CTRL  : Pump
--
-- MAME/IPAC/JPAC Style Keyboard inputs:
--   5           : Coin 1
--   6           : Coin 2
--   1           : Start 1 Player
--   2           : Start 2 Players
--   R,F,D,G     : Player 2 Movements
--   A/S         : Player 2 Pump
--
--
-- Joystick support.
-- 
-- 
---------------------------------------------------------------------------------
-- 21 September 2019
---------------------------------------------------------------------------------
--   FIXED: wrong aspect ratio in "Vert" mode. 
---------------------------------------------------------------------------------
-- 24 October 2019
---------------------------------------------------------------------------------
--   FIXED: Little problem with CRT and HDMI.
-- CHANGED: Keyboard inputs.
--          Abolished rotation of control direction in Horz mode.
---------------------------------------------------------------------------------

                                *** Attention ***

ROM is not included. In order to use this arcade, you need to provide a correct ROM file.

Find this zip file somewhere. You need to find the file exactly as required.
Do not rename other zip files even if they also represent the same game - they are not compatible!
The name of zip is taken from M.A.M.E. project, so you can get more info about
hashes and contained files there.

To generate the ROM using Windows:
1) Copy the zip into "releases" directory
2) Execute bat file - it will show the name of zip file containing required files.
3) Put required zip into the same directory and execute the bat again.
4) If everything will go without errors or warnings, then you will get the a.*.rom file.
5) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using Linux/MacOS:
1) Copy the zip into "releases" directory
2) Execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using MiSTer:
1) scp "releases" directory along with the zip file onto MiSTer:/media/fat/
2) Using OSD execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

