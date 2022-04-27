# WeatherSpyware
 Spyware, wanted to get it off my computer, but still wanted to look at it - found in AppData\Local\Weather, in case anyone had the same problem as me - definitely some personal info on these files, but its aimed at Chrome so who cares

 in-action.jpg is a screenshot of it while working via Task Manager - usually doesn't appear - unsure if thats because chrome wasn't running or it hides itself
 Logfile.CSV is taken from ProcMon at the point of running the original .exe, accidentally only took one entry instead of the many, but you could do this yourself
 Through this I identified AppData\Local\Microsoft\Windows\INetCache\IE\K06D22Z9, a location where an installation .exe and a file containing info about AMD products, my PC being made from these - found it online in a history course of all places - https://www.coursehero.com/file/50202792/rechw1blb/

 Currently, unable to copy across the 'Current Session' file, as it gets used
 There is an uninstall .exe, but i will use ProcMon to see what it actually does - I don't want the malware to be left

 Two main file paths:
    C:\Users\user\AppData\Roaming\Weather - contains actual .exe
    C:\Users\user\AppData\Local\Weather - contains malware files and databases

 The 'credible' side of the app is a joke - a setup.exe that doesn't even run when you install is a sham - the eula is just a copy of the creative commons license
 I am going to see what the uninstall.exe will do, but i wonder if it will remove everything

 The database side I am unfamiliar with, but it appears to be written in SQLite 3 

 What I've done so far:
    Identified the files using WinDirStat
    Recorded processes using ProcMon and Fiddler
    Copied files

 Update:
   Uninstall does work!.. but only for the Roaming 'visible' section, the local is still there
   As of now, I will be deleting these files, and finally get some peace of mind.
   This github will still be here, but abandoned
   I hope this helps anyone who falls into a similar situation, but it most likely wont happen as long as you have an antivirus or common sense

   PS: nw.dll was too large to upload, so I guess it'll be deleted now
       Heres the link that the installer connected to, amongst others: https://kan-web-am.sfo3.digitaloceanspaces.com, https://didiserver.herokuapp.com, https://s3.tebi.io/kan-web-am/reg/, chrome-extension://kallgdibceggeagefefonleiaejmafd/app.html and a useful website: https://www.joesandbox.com/analysis/487057/0/html
