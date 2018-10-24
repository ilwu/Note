# Note

## Markdown 語法說明中文版

https://github.com/othree/markdown-syntax-zhtw


## 移除專案中不需要的參考
URL:
https://marketplace.visualstudio.com/items?itemName=battas.ResolveUR-ResolveUnusedReferences

說明:
僅供參考, 不建議自動移除, 有些第三方lib使用到, 但未在專案中使用的也會被移除


##Chocolatey

Will 保哥的開發人員工具軟體清單 ( 最新 2017 年版 )
https://blog.miniasp.com/post/2017/09/13/Will-2017-Ultimate-Developer-Tool-Software-List.aspx

Installing Chocolatey (in power shell)
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

Installing ChocolateyGUI
choco install ChocolateyGUI

## PowerShell 實現 tail 功能
Get-Content -Path "C:\scripts\test.txt" -Wait

## 加速 powershell 開啟

http://blog.xuite.net/haoming/mypoint/166267497-%E5%8A%A0%E5%BF%ABPowershell%E9%96%8B%E5%95%9F%E9%80%9F%E5%BA%A6

Set-Alias ngen @(
dir (join-path ${env:\windir} "Microsoft.NET\Framework") ngen.exe -recurse |
sort -descending lastwritetime
)[0].fullName
[appdomain]::currentdomain.getassemblies() | %{ngen $_.location}


## Window 10 Telnet
執行
dism /online /Enable-Feature /FeatureName:TelnetClient

開始右鍵->應用程式與功能->程式和功能
