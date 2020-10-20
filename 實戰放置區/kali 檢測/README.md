## kali檢查漏洞  
---

檢查自身網路

    ifconfig

網段中有那些系統開啟--->指令: 

    netdiscover -r 10.0.2.0/24<--區段分割ip

確認某主機是否live(活著) 

    ping 主機ip

確認某主機作業系統 

    nmap -O 主機ip

確認主機是否有漏洞 nmap --script vuln 漏洞全檢查      

         也可使用--script smb-vuln-ms08-067.nse -p445   檢測ms08-067此漏洞
                      
註.1  Google hacking最先進的漏洞檢查

---
