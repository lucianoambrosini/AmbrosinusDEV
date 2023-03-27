# AmbrosinusDEV | Win SD launcher

[![GitHub release](https://img.shields.io/badge/release-v1.0.0-blue)](https://github.com/lucianoambrosini/Ambrosinus-Toolkit/blob/main/latest_version.txt)
[![GitHub release date](https://img.shields.io/badge/last%20release%20date-March_2023-green)](https://bit.ly/Ambrosinus-Toolkit)
[![GitHub support forum](https://img.shields.io/badge/Support%20forum-Help-critical)](https://discourse.mcneel.com/t/ambrosinus-toolkit/147124?u=ambrosinus)
[![GitHub license](https://img.shields.io/github/license/lucianoambrosini/Ambrosinus-Toolkit?color=orange)](https://github.com/lucianoambrosini/Ambrosinus-Toolkit/blob/main/LICENSE)

**Win SD launcher** is a *Windows OS App (.EXE)* that simplifies the launching task of the AUTOMATIC1111 project locally.

<div align="center">
<img src="https://ambrosinus.altervista.org/blog/wp-content/uploads/2023/03/WinSDlauncher_App_02_out.jpg" width="30%" height="30%">
</div>

### Info components
This tool allows you to set (only once from the first start) the path of the folder where you installed Stable Diffusion (and related expansions such as ControlNET) on your machine. Then let's launch Stable Diffusion locally and close the process.
Run this App as Administrator, if you forgot to do this never mind close Windows Terminal and then the App.<br>
*It will be restarted automatically as Administrator mode.*
<br>

Video demo [click here](https://youtu.be/E37TKR2qKT4)
<br>

## Requirements
AUTOMATIC1111 project installation: [Read full instructions here](https://ambrosinus.altervista.org/blog/ai-as-rendering-eng-sd-controlnet-locally/#part1)
<br>
Add these strings to **"webui-user.bat"** (or replace yours with these totally):
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
