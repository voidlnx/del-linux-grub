diskpart

select disk 0

sel part 1

assign letter z:

exit

bcdboot c:\windows /s z: /f all

bcdedit.exe /enum firmware

bcdedit.exe /delete {***ID***}
