#
# WINDOWS 
- [使用powershell get-filehash](https://learn.microsoft.com/zh-tw/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-7.5)
  - 支援
  - 測試
    - 打開powershell
    - `Get-FileHash -Path D:\Test20250611.docx -Algorithm MD5`
    - `Get-FileHash -Path D:\Test20250611.docx -Algorithm SHA384 | Format-List`
