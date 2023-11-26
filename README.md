# IDM-Activation-Script
Script to activate or reset IDM 

IDM Activation Script

An open source tool to activate or reset trial of Internet Download Manager
Features

    IDM activation with registry key lock method
    Activation persists even after installing IDM updates
    IDM trial reset
    Fully open source
    Based on transparent batch script

IAS Latest Release

Last Release - v0.8 (10-Aug-2023)
GitHub
Download / How to use it?

    First, fresh install Internet Download Manager. Make sure previous cracks/patches are removed/uninstalled if there are any.
    After that, follow below steps to activate it.

Method 1 - PowerShell

(Recommended)

    On Windows 8.1/10/11, right-click on the windows start menu and select PowerShell or Terminal (Not CMD).
    Copy-paste the below code and press enter
    irm https://massgrave.dev/ias | iex
    You will see the activation options, follow the on-screen instructions.
    That’s all.

Method 2 - Traditional

    Download the file from here
    Right click on the downloaded zip file and extract
    In the extracted folder, run the file named IAS.cmd
    You will see the activation options, and follow onscreen instructions.
    That’s all.

Info
Activation

    This script applies registry lock method to activate Internet download manager (IDM).
    This method requires Internet at the time of activation.
    IDM updates can be installed directly without having to activate again.
    After the activation, if in some case, IDM starts to show activation nag screen, then just run the activation option again.

Reset IDM Activation / Trial

    Internet download manager provides 30 days trial period, you can use this script to reset this Activation / Trial period whenever you want.
    This option also can be used to restore status if in case IDM reports fake serial key and other similar errors.

OS requirement

    Project is supported for Windows 7/8/8.1/10/11 and their Server equivalent.
    PowerShell method to run IAS is supported on Windows 8 and higher.

Advanced Info

    To add a custom name in IDM license info, edit line number 21 in the script file.
    For activation in unattended mode, run the script with /act parameter.
    For reset in unattended mode, run the script with /res parameter.
    To enable silent mode with above two methods, run the script with /s parameter.

How does it work?

    IDM stores the data related to trial and activation in across various registry keys. Some of these keys are locked to protect them from tampering and data is stored in a pattern to track the fake serial issue and the remaining trial days. To activate it, script here simply generate those registry keys by triggering a few downloads in IDM and identifies those registry keys and locks them so IDM can’t edit and view. That way IDM cannot show the warning that it’s activated with a fake serial key.

Troubleshoot

    Browser Integration Fix: Chrome FireFox
    Reach out to us on Discord (signup not required) with an error screenshot.

Changelog

v0.8

    Move the project to Github and massgrave.dev
    Minor bug fixes
    Add an info to inform users that empty registry keys are being deleted when script deletes a lot of the them.



Made with Love ❤️

