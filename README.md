# Auto Downloader: Spotify & Visual Studio Code

This project provides a simple Windows batch script that downloads Spotify and Visual Studio Code installers. It’s useful for quickly setting up a new machine or sharing tools with others.

⸻

# 📦 Files Included
	•	setup-tools.bat — The batch file that handles downloading

⸻

# 🚀 What It Does

When you run the script:
	
 1.	It displays:
 
download all
click any key to continue

2.	Waits for a key press.
	
 3.	Downloads:
	•	SpotifySetup.exe from the official Spotify server
	
 •	VSCodeSetup.exe from the official Visual Studio Code server
	
 4.	Saves the installers in the same folder as the script.


# 📥 How to Use

Step 1: Download or Clone This Repository

Using Git:
git clone https://github.com/Jayden4400338/Spotify-vsc-download-.git

Or click the green Code button above and download the ZIP.

# Step 2: Run the Script
	
1. Locate the setup-tools.bat file in File Explorer.
	
 2.	Double-click it to run.
	
 3.	(Optional) Right-click and select Run as administrator if needed.

# Step 3: Wait for Downloads

After pressing a key, the script will download:
	•	SpotifySetup.exe
	•	VSCodeSetup.exe

Both will appear in the same folder.


# 🛠️ How the Script Works

Here’s the code used in setup-tools.bat:

@echo off
echo download all
echo.
echo click any key to continue
pause >nul

echo.
echo Downloading Spotify...
powershell -Command "Invoke-WebRequest -Uri https://download.scdn.co/SpotifySetup.exe -OutFile SpotifySetup.exe"

echo.
echo Downloading Visual Studio Code...
powershell -Command "Invoke-WebRequest -Uri https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user -OutFile VSCodeSetup.exe"

echo.
echo Downloads complete.
pause

# 🔄 Optional: Convert to EXE

If you want to turn the batch script into an .exe file:

1.	Download Bat To Exe Converter
	
 2.	Open it and select setup-tools.bat
	
 3.	Click Compile to generate a .exe


# ⚠️ Notes
•	Requires PowerShell (available by default on Windows 10/11).
	
 •	Requires internet access.
	
 •	Files are downloaded directly from official sources.

# 📄 License

This project is licensed under the MIT License — free to use, modify, and share.

