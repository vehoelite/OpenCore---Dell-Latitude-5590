Sonoma 14.7.2 on a Dell Latitude 5590
Full functioning, everything working to my knowledge.<BR>
Enjoy - VE

Installation<BR><BR>

1<BR>
Using Rufus format a USB (32GB will do) select "Non Bootable", make sure its
GPT and Large FAT32 is the file system -32KB. Format.<BR><BR>

2<BR>
Goto root of formatted USB and clear/delete files placed by rufus and add
EFI -recursively found here to the root of formatted USB IE: E:\EFI or /EFI.<BR><BR>

3  **Install Python3 before proceeding**<BR>
Goto OpenCore and download the latest RELEASE package with included Utilities and
find macrecovery. Goto your native command prompt and type:<BR><BR>

Windows (Python installed from pythons official site)<BR>
python macrecovery.py -b Mac827FAC58A8FDFA22 -m 00000000000000000 download<BR><BR>

Windows (Python was installed from Windows App Store)<BR>
python3 macrecovery.py -b Mac827FAC58A8FDFA22 -m 00000000000000000 download<BR><BR>

Linux based OS<BR>
./macrecovery.py -b Mac827FAC58A8FDFA22 -m 00000000000000000 download<BR><BR>

4<BR>
Copy the output folder com.apple.recovery.boot and BaseSystem.chunklist/BaseSystem.dmg to the 
root of your newly formatted USB.<BR>
IE: E:\com.apple.recovery.boot or /com.apple.recovery.boot<BR><BR>

5<BR>
Reboot system, press F12 during bootup to enter Boot Menu. Select your USB drive and it will
boot you to OpenCore's menu selection. Select No Name / Recovery.<BR><BR>

6<BR>
Boot into Apple Recovery. Select Disk Utility and format a partition large enough to
either Mac OS Extended (Journaled) or Mac OS Extended (Journaled, Encrypted). Exit <BR><BR>

7<BR>
While connected Wifi or Wired, select Reinstall Sonoma MacOS then continue.
After 4 or 5 reboots (Remember to hit f12 after each reboot) you will be greeted with
a flawless? Sonoma 14.7.2.
