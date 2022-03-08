# Useful Commands

## Networking
<code>Get-NetTCPConnection | where Localport -eq PortHere | select Localport,@{Name="Process";Expression={(Get-Process -Id $_.OwningProcess).ProcessName}}</code>

<code>Get-NetTCPConnection | select Localport,@{Name="Process";Expression={(Get-Process -Id $_.OwningProcess).ProcessName}}</code>
