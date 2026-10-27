$Path = "$env:TEMP\chrome_installer.exe"
Invoke-WebRequest -Uri "https://dl.google.com/chrome/install/latest/chrome_installer.exe" -OutFile $Path
Start-Process -FilePath $Path -Args "/silent /install" -Wait
Remove-Item $Path
