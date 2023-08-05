PSNope v1.05 by user
---------------

latest additions:
- psid spoofing
- cleanup boot_history.dat etc.
- delete boot_history.dat etc.
- beep to indicate successful rif creation

v1 features:
- activate PSN content
- spoof idps
- fake ofw (remove cfw syscalls)
- firmware independent i.e. no version specific offsets

---------------

Greetings to:
ps3dev-net

---------------

Q&A

Q: I want to activate PSN content. How to get started?
A: 1. create the folders psnope\lic\ on your pen drive
    2. put the rap files of the content you want to activate into the "lic" dir
    3. plug your pen drive into the rightmost usb port of your ps3 (/dev_usb000)
    4. run PSNope

Q: Do i need the "aa" account to make it work?
A: No, you don't.

Q: How can i enable changing my idps?
A: open config.txt, change "spoof_idps=0" to "spoof_idps=1" and set "idps=" to the idps you want to use

Q: Where does it look for config.txt?
A: It looks for config.txt in the following places and uses the first it is able to open:
    1. /app_home/config.txt
    2. /dev_usb000/psnope/config.txt
    3. /dev_hdd0/game/BLES08890/USRDIR/config.txt

Q: I spoofed my idps and and activated some content. Why doesn't it work?
A: Because your idps is part of the decryption algo. Please set "use_spoofed_idps" to "1" to fix it.

Q: Whats a ".klic" file?
A: Its a decrypted ".rap" file. PSNope supports these as well.

Q: How can i disable certain System Calls that may be detected?
A: remove_cfw_syscalls=1

Q: Will PSNope work on future CFWs?
A: It should work as is, because there are no version specific offsets being used (unlike the others).

Q: Is there any chance my console could get bricked by PSNope?
A: Nope ;) no changes are being made to your console's flash.

Q: Can I use the source code or parts of it in my own projects?
A: Sure, as long as your project is open source.




