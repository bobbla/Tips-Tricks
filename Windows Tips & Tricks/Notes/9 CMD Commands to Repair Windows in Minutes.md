
#  9 CMD Commands to Repair Windows in Minutes 

https://www.youtube.com/watch?v=I-T9AjKQlt0

Is your Windows PC freezing, crashing, or losing internet for no reason? Before you reset Windows or pay for repair tools, try these 9 built-in commands first. In this video I walk you through every command step by step, including winget for updating every app at once, sfc and DISM for repairing system files, chkdsk for scanning your drive, ipconfig and netsh for fixing network issues, a PowerShell trick for checking drive health, tasklist and taskkill for closing rogue processes, and powercfg for diagnosing power problems. I also include one bonus tool that can save you from blaming Windows for problems caused by faulty RAM. Every command works on Windows 10 and Windows 11, including 25H2. No paid software, no downloads. 

Commands Used
---------------------------
1. winget upgrade –all and winget upgrade
2. sfc /scannow
3. dism /Online /Cleanup-Image /RestoreHealth
4. chkdsk /r
5. ipconfig /flushdns  
ipconfig /release 
ipconfig /renew
6. netsh winsock reset 
netsh int ip reset  
netsh int space tcp reset
7. powershell "Get-PhysicalDisk | Format-Table FriendlyName, MediaType, HealthStatus, OperationalStatus"
8. tasklist
taskkill /PID [number] /F
taskkill /IM [processname.exe] /F
9. powercfg /energy

Bonus Command
mdsched
