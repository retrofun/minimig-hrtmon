# HRTMON for MiST/MiSTer

* HRTMON.zip - v2.35

  Copy of https://github.com/mist-devel/mist-binaries/blob/master/cores/minimig-aga/HRTMON.ROM

* hrtmonV2.37WinUAE.zip

  Copy of https://github.com/nretro/Minimig-AGA_MiSTer/blob/MiSTer/releases/hrtmonV2.37WinUAE.zip - Source: [Atari-Forum](http://92.222.181.53/viewtopic.php?f=117&t=32761&sid=de62eff5a8ccd51669812345830beeb2&start=625#p375234)

* hrtmon_2.32_winuae.zip

  Extracted hrtmon.rom v2.32 from [WinUAE commit dddda49](https://github.com/tonioni/WinUAE/blob/dddda495138060d60febe4cc15f03c3461b13e29/hrtmon.rom.cpp)

* hrtmon_2.33_winuae.zip

  Extracted hrtmon.rom v2.33 from [WinUAE commit e7d6f64](https://github.com/tonioni/WinUAE/blob/e7d6f64da6ab5326c1daefbeab4c66c279006f96/hrtmon.rom.cpp)

* hrtmon_2.35_winuae.zip

  Extracted hrtmon.rom v2.35 from [WinUAE commit 5149b28](https://github.com/tonioni/WinUAE/blob/5149b2815e3de7f7db4ed12ae5f90a984b69bbab/hrtmon.rom.cpp)

* hrtmon_2.36_winuae.zip

  Extracted hrtmon.rom v2.36 from [WinUAE commit 10fc0d6](https://github.com/tonioni/WinUAE/blob/10fc0d68f9fb4345a2a0e6f8f947fcb3e61b2a49/hrtmon.rom.cpp)

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

* hrtmon_2.37_winuae.zip

  Extracted hrtmon.rom v2.37 from [WinUAE commit fd35790](https://github.com/tonioni/WinUAE/blob/fd3579099aae18f6abd4ae076196276359e5ed50/hrtmon.rom.cpp)

* winuae-hrtmon.rom-extract-1.0.tar.bz2

  Extracts hrtmon.rom from WinUAE's source file hrtmon.rom.cpp.

  Type
  ```
  make extract
  ```
  and it will download hrtmon.rom.cpp from WinUAE Github repository, compile the extraction tool and extract hrtmon.rom.
