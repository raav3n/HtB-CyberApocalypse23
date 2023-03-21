# Artifacts of Dangerous Sightings (medium)
## Description 
Pandora has been using her computer to uncover the secrets of the elusive relic. She has been relentlessly scouring through all the reports of its sightings. However, upon returning from a quick coffee break, her heart races as she notices the Windows Event Viewer tab open on the Security log. This is so strange! Immediately taking control of the situation she pulls out the network cable, takes a snapshot of her machine and shuts it down. She is determined to uncover who could be trying to sabotage her research, and the only way to do that is by diving deep down and following all traces ...

## Initial thoughts 
We are given a vhdx file which esentially a virtual ahrd disk (typically for VMs). I figured I could use something like Autopsy or FTK Imager to analyze all of its contents.

## Finding 1
I figured some file or command would be hidden somewhere. One of the first places I thought to look was the Windows Taks and sure enough there seems to be a powershell script hidden with a long encrypted string being passed.