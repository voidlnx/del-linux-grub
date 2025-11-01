# Windows CMD (Admin):

diskpart

select disk ***disk***

sel part ***Windows,EFISystem***

assign letter z:

exit

bcdboot c:\windows /s z: /f all

bcdedit.exe /enum firmware

bcdedit.exe /delete {***ID***}
