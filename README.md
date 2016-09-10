##DifferentSLI Auto NVIDIA® Driver Patcher and Signer by Ember
####What it is
---
This patcher will automatically patch and sign "nvlddmkm.sys" for NVIDIA® drivers for 64-bit systems to enable SLI™ with different cards.
####To use
---
1. Install original NVIDIA® drivers
2. Put cards together you want to SLI™
3. Reboot
4. (A) (For < 372.XX series drivers) Copy original "nvlddmkm.sys" from "C:\Windows\System32\drivers\" and put it in the same folder as the patcher.
4. (B) (For >= 372.XX series drivers) The original "nvlddmkm.sys" file is stored in a directory under "C:\Windows\System32\DriverStore\FileRepository". The name may vary by install, but it will always start with "nv_dispi.inf", go to Device Manager -> "Display Adapters" section -> (Right Click GPU) -> "Properties" -> "Driver" tab -> "Driver Details" button -> to find the specific install location of "nvlddmkm.sys". Copy "nvlddmkm.sys" from this lcation to the same folder as the patcher.
5. Run "DifferentSLIAuto.exe" and press patch, if everything went well it will say that patching was successful, if not contact Ember on techPowerUp! and do not continue.
6. Log in as Administrator
7. UAC must be disabled
8. (A) (For < 372.XX series drivers) Run Install.cmd
8. (B) (For >= 372.XX series drivers) Run Install.cmd, then copy the "nvlddmkm.sys" file installed at "C:\Windows\System32\drivers\" by Install.cmd to the same "nv_dispi.inf" directory used in step 4b
9. Reboot

Windows Test Sign Mode MUST be enabled for the patched drivers to load!
####FAQ
---
   Q: Completely uninstalling DifferentSLIAuto  
   OR  
   Q: SignTool lists multiple certificates suitable for signing  
   A: Follow all steps in post below  
   http://www.techpowerup.com/forums/threads/sli-with-different-cards.158907/page-54#post-3215633  
####History
---
   version 1.4 19/03/16 Supporting WHQL 364.51 and up  
   version 1.3.1 23/07/15 Preliminary Windows 10 support  
   version 1.3 20/02/15 First GitHub release, tweaked Install.cmd, updated tools folder  
   version 1.2 16/01/15 Supporting up to WHQL 347.09 and up, tweaked Install.cmd, updated tools folder, corrected dates in changelog, added "License" section, tweaked section titles, tweaked "To use" section, added "FAQ" section  
   version 1.1 26/05/14 Supporting up to WHQL 337.88  
   version 1.0 01/11/13 Initial Release  
####Thanks
---
   anatolymik @ techPowerUp! for the original patch  
   DifferentSLI Auto uses [uFMOD](http://ufmod.sourceforge.net/), [Kurapika's C# Native DLL Mapper](http://forum.exetools.com/showthread.php?t=15309), and sigScan C# Implementation by [atom0s](https://github.com/atom0s)

NVIDIA and SLI are trademarks and/or registered trademarks of NVIDIA Corporation in the U.S. and other countries.
