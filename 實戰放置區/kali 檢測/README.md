檢查自身網路ifconfig

網段中有那些系統開啟--->指令: netdiscover -r 10.0.2.0/24<--區段分割ip

確認某主機是否live(活著) nmap -O 主機ip
                        ping 主機ip

確認某主機作業系統 nmap -O 主機ip

確認主機是否有漏洞 nmap --script vuln 
                      --script smb-vuln-ms08-067>.nse -p445
