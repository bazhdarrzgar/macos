## Step 1 

* installing all this tool:

    - OpenCore: https://github.com/acidanthera/opencorepkg/releases

    - ProperTree: https://github.com/corpnewt/ProperTree

    - MountEFI: https://github.com/corpnewt/MountEFI

    - OC-Gen-X: https://github.com/Pavo-IM/OC-Gen-X/releases

## Step 2

* go to the AppStore -> Search for ( "monterey" ) -> click to "get"

## Step 3

* go to "Disk Utility" -> Click to "View" -> choose "show all devices" -> Click to "usb drive" -> click to "Erase" -> Format should be "Mac OS Extended (Journaled) -> Name is "MyVolume" -> click to "Erase"

## Step 4

* search for "terminal" -> type "sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume" 


## Step 5

* open "OC_Gen-X" program -> in "System Type" tab select "Alder Lake" -> in "Kext" tab select "Graphics" tab choose "WhateverGreen" option -> in "Kext" tab select "Audio" tab choose "AppleALC" -> in "Kext" tab select "Ethernet" tab and choose "IntelMausi" -> in "SMBIOS" tab choose "iMac20,1" -> after that click to "generate"


## Step 6

* download all depedency in this link "https://dortania.github.io/Getting-Started-With-ACPI/ssdt-methods/ssdt-prebuilt.html#laptop-ice-lake" -> after that copy all this file to "EFI/OC/ACPI"


## Step 7

* open terminal and open file "MountEFI.command" with this command "python3 MountEFI.command" -> choose your usb drive it should be some thing like this "Install macOS Big Sur ( disk3s2 ) -> now drag "EFI" folder to "EFI" partition


## Step 8

* open "ProperTree.command" with python3 in terminal -> go to file "open" select "EFI" folder and "OC" and "config.plist" -> follow the video here "https://www.youtube.com/watch?v=Gaosub7FRf4&t=2755s&ab_channel=freeCodeCamp.org" in time "51:25"


