# Internet-Explorer-Reborn

Internet Explorer REBORN is a Windows desktop recreation of the classic Internet Explorer experience, rebuilt as a standalone `.exe` with a retro shell and an optional modern browsing mode.

This project is focused on preserving the look and feel of a 2006-era browser while still making it usable on a modern Windows machine.

## Features

- Classic Internet Explorer-inspired menu bar, toolbar, address bar, and status bar
- Standalone Windows executable
- Saved home page setting
- Saved favorites/bookmarks
- Custom application icon
- `Modern Mode` toggle for Chromium-backed browsing
- In-app modern tabs powered by WebView2

## Current Version

`Internet explorer REBORN 1.0 FOUNDATION edition`

## How It Works

The app supports two browsing modes:

- Classic mode uses the legacy Windows Internet Explorer-style embedded browser control.
- Modern Mode opens a new in-app tab backed by Chromium through WebView2 for better compatibility with modern websites.

This means the project keeps the retro Internet Explorer shell while still allowing newer sites to load in a more capable engine when needed.

## Running The App

Open one of the executables from the build output:

- `1.0\build\Internet Explorer REBORN.exe`
- `1.0\build\Internet Explorer REBORN 1.0.exe`

The build output also includes the required WebView2 support DLLs beside the executable.

## Settings

Use the top menu bar and click `Settings` to open the settings window.

From there you can:

- Change the home page
- Enable or disable `Modern Mode`

Favorites can be added from the `Favorites` menu and are saved between launches.

## Project Structure

- `1.0\Program.cs` - application startup and browser feature configuration
- `1.0\MainForm.cs` - main Internet Explorer-style window and tab behavior
- `1.0\Dialogs.cs` - settings and favorites dialogs
- `1.0\AppSettings.cs` - saved homepage, favorites, and Modern Mode settings
- `1.0\build.ps1` - build script for producing the Windows executable

## Notes

- This is a recreation project and is not affiliated with Microsoft.
- Classic mode is intentionally nostalgic and may not render every modern site correctly.
- Modern Mode is the recommended option for newer websites.

## Beta 1.0

The first public beta includes the retro shell, saved settings, favorites, and Chromium-backed modern tabs.

More updates are planned as the project evolves.
