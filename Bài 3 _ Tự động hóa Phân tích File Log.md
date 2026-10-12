1\. Sơ đồ luồng dữ liệu  
Get-Content (stdout) $\rightarrow$ | $\rightarrow$ Select-String (stdin/stdout) $\rightarrow$ | $\rightarrow$ Measure-Object (stdin)  
2\. Câu lệnh PowerShell   
(Get-Content access.log | Select-String "TIMEOUT" | Measure-Object \-Line).Lines 