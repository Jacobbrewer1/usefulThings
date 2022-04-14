# Useful Commands

## Git hooks
<code>git config --global core.hooksPath '/C/place path here/nextgen-tools/git-hooks</code>

## Networking
<code>Get-NetTCPConnection | where Localport -eq PortHere | select Localport,@{Name="Process";Expression={(Get-Process -Id $_.OwningProcess).ProcessName}}</code>

<code>Get-NetTCPConnection | select Localport,@{Name="Process";Expression={(Get-Process -Id $_.OwningProcess).ProcessName}}</code>
