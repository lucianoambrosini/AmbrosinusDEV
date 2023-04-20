# AmbrosinusDEV | Win SD launcher

[![GitHub release](https://img.shields.io/badge/release-v1.1.1-blue)](https://github.com/lucianoambrosini/Ambrosinus-Toolkit/blob/main/latest_version.txt)
[![GitHub release date](https://img.shields.io/badge/last%20release%20date-April_2023-green)](https://bit.ly/WinSDlauncher)
[![GitHub support forum](https://img.shields.io/badge/Support%20forum-Help-critical)](https://discourse.mcneel.com/t/ambrosinus-toolkit/147124?u=ambrosinus)
[![GitHub license](https://img.shields.io/github/license/lucianoambrosini/Ambrosinus-Toolkit?color=orange)](https://github.com/lucianoambrosini/Ambrosinus-Toolkit/blob/main/LICENSE)

**Win SD launcher** is a *Windows OS App (.EXE)* that simplifies the launching task of the AUTOMATIC1111 project locally, a wonderful project allows users to run Stable Diffusion and ControlNET locally on their machines. **WinSDlauncher** makes launching the application quicker and easier (as I said it is only for "lazy" designers I use it a lot 😉)
<br>
### ✔️ Please download this app only from this OFFICIAL source
<br>

<div align="center">
<img src="https://ambrosinus.altervista.org/blog/wp-content/uploads/2023/03/v111_01.png" width="25%" height="25%">
&nbsp &nbsp
<img src="https://ambrosinus.altervista.org/blog/wp-content/uploads/2023/03/v111_02.png" width="25%" height="25%">
&nbsp &nbsp
<img src="https://ambrosinus.altervista.org/blog/wp-content/uploads/2023/03/v111_03.png" width="25%" height="25%">
</div>

### Info components
This tool allows you to set (only once from the first start) the path of the folder where you installed Stable Diffusion (and related expansions such as ControlNET) on your machine. *With v1.1.1 is not required to run the App as a Windows Administrator, simply install your Stable Diffusion from AUTOMATIC1111 in a folder easily accessible - for instance, I have installed it on my Desktop.*
<br>

**Video demo [click here](https://youtu.be/EjUSKjRKKlI)**
<br>

## Requirements
**1)** AUTOMATIC1111 project installation: [Read full instructions here](https://ambrosinus.altervista.org/blog/ai-as-rendering-eng-sd-controlnet-locally/#part1)
<br>
**2)** Add these strings to **"webui-user.bat"** (or replace yours with these totally):
```
@echo off
set PYTHON=
set GIT=
set VENV_DIR=
set COMMANDLINE_ARGS=--api --lowvram --theme dark --autolaunch
git pull
call webui.bat
```
<br>
<br>

**Enjoy your Design exploration!** 😉

**P.S.:** This is my first APP/Utility for Windows OS but it is functional for its intended purpose.
