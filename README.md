@echo off
echo Dim obj_vbscript > %temp%\nft.vbs
echo Set obj_cmd = WScript.CreateObject("WScript.Shell")    >> %temp%\nft.vbs
echo Do While True >> %temp%\nft.vbs
echo  obj_vbscript = obj_cmd.sendkeys("{NUMLOCK}{NUMLOCK}") >> %temp%\nft.vbs
echo  Wscript.Sleep (5000) >> %temp%\nft.vbs
echo Loop >> %temp%\nft.vbs
cscript %temp%\nft.vbs
