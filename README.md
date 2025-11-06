# Windows CMD (Admin):

diskpart

list disk

select disk ***disk***

list part

sel part ***Windows,EFISystem***

assign letter z:

exit

bcdboot c:\windows /s z: /f all

bcdedit.exe /enum firmware

bcdedit.exe /delete {***ID***}
