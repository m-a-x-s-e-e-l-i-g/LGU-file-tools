# LGU file tools
Convert LGU firmware update package files used by Dacia & Renault MediaNav systems.

## What is LGU?
An LGU file is a firmware update package used by Renault & Dacia MediaNav and R-Link navigation and entertainment systems (which run on Windows CE 6.0).  
The firmware update is usually stored on a USB drive and then installed on the MediaNav.  
[m-a-x-s-e-e-l-i-g/MediaNav-to-Evolution-Upgrade](https://github.com/m-a-x-s-e-e-l-i-g/MediaNav-to-Evolution-Upgrade/) contains a guide on how to upgrade MediaNav, and also contains two LGU files.

## 📦 Downloads
| Version       | Download Link | Notes |
|---------------|---------------|-------|
| v3.04 | [Download](https://github.com/m-a-x-s-e-e-l-i-g/LGU-file-tools/blob/main/releases/lgu2dir_dir2lgu_V3.04.zip) | Translated to English |
| v3.03 FavreMod | [Download](https://github.com/m-a-x-s-e-e-l-i-g/LGU-file-tools/blob/main/releases/lgu2dir_dir2lgu_V3.03_FavreMod.zip) | Made compatible with MN1 6.0.3MD |
| v2.0.1         | [Download](https://github.com/m-a-x-s-e-e-l-i-g/LGU-file-tools/blob/main/releases/lgu2dir_dir2lgu_V2.0.1.zip)         | Fixed some bugs, added the ability to close upgrade.lgu also for MEDIANAV EVO |
| Legacy         | [Download](https://github.com/m-a-x-s-e-e-l-i-g/LGU-file-tools/blob/main/releases/lgu2dir_dir2lgu_legacy.zip)         | Predates known releases |

## Usage
To extract the contents of an LGU file, run the following command in a terminal window:  
`lgu2dir.exe <input lgu file> <output folder>`  

To create an LGU file from a folder, run the following command in a terminal window:  
`dir2lgu.exe <input folder> <output lgu file>`  
example: `.\lgu2dir.exe upgrade.lgu output`  

## Tool.bat Usage
### Main Menu

- `E` — Extract `.lgu` file  
- `C` — Compress `.lgu` file  
- `X` — Exit  

### Extract Options

- `U` — Extract `Upgrade.lgu` → outputs to `Medianav/`  
- `R` — Extract `Upgrade_root.lgu` → outputs to `Medianav/`  

### Compress Options

- `U` — Create `Upgrade.lgu` for MN1 → outputs to `New/`  
- `R` — Create `Upgrade_root.lgu` for MN1 → outputs to `New/`  
- `W` — Create `Upgrade.lgu` for MN2 → outputs to `New/`  

## 📁 Requirements

- External tools: `lgu2dir`, `dir2lgu` must be in the same folder or in PATH.
- `Medianav` and `New` directories must exist or will be used for output.


## Credits
Originally created by FavreMod using tools by djeman.
Uploaded here to keep them accessible and prevent them from getting lost.  

Source code (if you want to compile it yourself):  
[yosicovich/MediaNavMods – lgutool](https://github.com/yosicovich/MediaNavMods/tree/master/pc/lgutool)
