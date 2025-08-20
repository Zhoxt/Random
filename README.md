$desk = [Environment]::GetFolderPath('Desktop')
Set-Location $desk
Compress-Archive -Path .\Requirements2 -DestinationPath .\Requirements2.zip -Force
Get-FileHash .\Requirements2.zip
