```powershell
Get-Service | Where-Object {$_.Status -eq "Running" -and $_.StartType -eq "Automatic" -and $_.DisplayName.StartsWith("A") }  
```
