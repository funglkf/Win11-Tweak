# Win11-Tweak

## Skip network when install 

In the page ask you connect to network, press `SHIFT+F10` to bring up a command prompt window and run `oobe\bypassnro`.
Computer will restart, and now you can select `I don't have internet`.



## Get Full Context Menus

![pic1](https://cdn.mos.cms.futurecdn.net/Pn8KWFS4fKhyFaUVP9FrGQ-1200-80.png)

1. Open regedit
2. Navigate to HKEY_CURRENT_USER\SOFTWARE\CLASSES\CLSID\
3. Create a new key called `{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}`
4. Create a new key called InprocServer32
5. Open the (Default) key in InprocServer32 and set its value to blank, then click OK.

![pic1](https://cdn.mos.cms.futurecdn.net/mdvovDoH5NAGyC2YYGN9gR-1200-80.png)

6. Close registry editor and reboot.

You will now see the classic-style context menu. If you want to revert back to the default, limited context menu, delete the InProc32 key.


## Remove Cortana

1. Open Windows Terminal as **administrator**. 
2. Run `Get-AppxPackage *Microsoft.549981C3F5F10* | Remove-AppxPackageand press Enter.`


