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
