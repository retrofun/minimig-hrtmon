# HRTMON for MiST/MiSTer

* HRTMON.zip - v2.35

  Copy of https://github.com/mist-devel/mist-binaries/blob/master/cores/minimig-aga/HRTMON.ROM

* hrtmonV2.37WinUAE.zip

  Copy of https://github.com/nretro/Minimig-AGA_MiSTer/blob/MiSTer/releases/hrtmonV2.37WinUAE.zip - Source: [Atari-Forum](http://92.222.181.53/viewtopic.php?f=117&t=32761&sid=de62eff5a8ccd51669812345830beeb2&start=625#p375234)

* hrtmon_2.37_mist.zip

  Latest [HRTMON.ROM](http://www.whdload.de/whdload/Tools/) 2.37 with command _reboot_ fix

  ```
  HRTMON.ROM 2.37 for MiST
  http://www.whdload.de/whdload/Tools/

  Compiled with vasm 1.8f
  http://sun.hasenbraten.de/vasm/

  Patch hrtmon_2.37_mist.patch:
  -changes blk.l to dcb.l in src/disassemble.c for vasm
  -configures HRTmon as cartridge ROM
  -sets build date in version string (28.04.2019)
  -fixes crash of reboot command


  # lha x hrtmon237.lha
  # cd hrtmon
  # mv SPRfont.raw sprfont.raw
  # patch -p1 < hrtmon_2.37_mist.patch
  # cd src
  # vasmm68k_mot -I/media/amigadevelopercd/NDK/NDK_3.1/Includes\&Libs/include_i -I.. -m68010 -Fbin -o HRTMON.ROM HRTmonV2.s


  65796144f7956c2aeceb9d4559316f8b  HRTMON.ROM
  ```

* winuae-hrtmon.rom-extract-1.0.tar.bz2

  Extracts hrtmon.rom from WinUAE's source file hrtmon.rom.cpp.

  Type
  ```
  make extract
  ```
  and it will download hrtmon.rom.cpp from WinUAE Github repository, compile the extraction tool and extract hrtmon.rom.
