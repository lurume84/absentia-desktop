[![Build Status AppVeyor](https://ci.appveyor.com/api/projects/status/github/lurume84/absentia-desktop?svg=true)](https://ci.appveyor.com/project/lurume84/absentia-desktop)

# Absentia desktop
This application is the container of [Absentia Viewer](https://github.com/lurume84/absentia-viewer) project. It is a chrome-based application (CEF) that loads viewer seamlessly and provides local storage capabilities.

Absentia is an application that automates the Disaster Victim Identification (DVI) process described by [Interpol](https://www.interpol.int/How-we-work/Forensics/Disaster-Victim-Identification-DVI).

## What it does

* Upgrades to last official Absentia Viewer automatically
* Disables CORS

## What it will do


## Installation
Just go to Releases section and download last Absentiaetup.exe installer. It will create a shortcut to the installation folder %localappdata%/Absentia Desktop.

## Usage
This application automatically creates folder %userprofile%/Documents/Absentia.exe. This folder contains all user-related information that is described below

### CrashReports
In case application crashes, a dump will be generated inside this folder. If you want to contribute to its resolution send it to me.

### Download
Github releases will be downloaded here. To force a redownload of viewer just delete versions folder and open application again.

### Html
Contains the downloaded viewer. This is automatically stepped over by viewer updates, also contains your connection token. In case you want to remove credentials remove token.json file.

### Absentia.ini
This is the file you need to modify to configure your desktop application.

## Development Guide
You need vs2017, CMake and Conan. Checkout and execute build.bat

## Compatibility
Windows is the only platform supported at this time. If application does not start up install last Visual Studio Redistributables.
