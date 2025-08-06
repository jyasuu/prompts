# Powershell

#### 2. **Check Current Execution Policy**
```powershell
Get-ExecutionPolicy
```

#### 3. **Set Execution Policy to Allow Script Execution**
To allow all local scripts to run (but still block unsigned remote scripts), use:
```powershell
Set-ExecutionPolicy RemoteSigned
```

Or, to allow all scripts (less secure):
```powershell
Set-ExecutionPolicy Unrestricted
```

### 🧪 Temporary Bypass (for a single script run)
If you don’t want to change the system-wide policy, you can run a script like this:
```powershell
powershell -ExecutionPolicy Bypass -File .\yourscript.ps1
```


```
Test-NetConnection $IP -port $PORT
```