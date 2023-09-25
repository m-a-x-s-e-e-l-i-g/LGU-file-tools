# LGU file tools
Convert LGU firmware update package files used by Dacia & Renault MediaNav systems.

## What is LGU?
An LGU file is a firmware update package used by Renault & Dacia MediaNav and R-Link navigation and entertainment systems (which run on Windows CE 6.0).  
The firmware update is usually stored on a USB drive and then installed on the MediaNav.  
[m-a-x-s-e-e-l-i-g/MediaNav-to-Evolution-Upgrade](https://github.com/m-a-x-s-e-e-l-i-g/MediaNav-to-Evolution-Upgrade/) contains a guide on how to upgrade MediaNav, and also contains two LGU files.

## Usage
To extract the contents of an LGU file, run the following command in a terminal window:  
`lgu2dir.exe <input lgu file> <output folder>`  

To create an LGU file from a folder, run the following command in a terminal window:  
`dir2lgu.exe <input folder> <output lgu file>`  
example: `.\lgu2dir.exe upgrade.lgu output`  

## Credits
I have no idea who created these tools, I found them on some forum and they work.
I uploaded them here so they are easier to find and use, and to prevent them from getting lost.
