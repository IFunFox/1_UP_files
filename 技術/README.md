## 技術
---

    雙因認證(Two-Way Factor)可以防止下列何者攻擊?
    (A)阻斷式服務攻擊    (B)SQL 資料隱碼攻擊
    (C)密碼側錄攻擊      (D)中間人攻擊

---
'''

    阻斷式服務攻擊Dos
    1.多台攻擊一台
    2丟入大量封包使電腦當機
    
    SQL 資料隱碼攻擊
    1.在輸入的字串之中夾帶SQL指令，在設計不良的程式當中忽略了字元檢查
    2.只要是支援批次處理SQL指令的資料庫伺服器，都有可能受到攻擊。
    
    密碼側錄攻擊
    1.又稱keylogger
    2.錄製鍵盤上的每個按鍵來尋找密碼

    中間人攻擊
    1.MITM
    
'''
---

    [7]網際網路中主要的通訊協定模式有兩種 OSI 7 層及 TCP/IP 協定組，
    請問在這兩個通訊協定模式中，負責傳輸封包（Packet）及選擇路徑（Routing），是那一層的工作？ 
    (A) 實體層（Physical Layer） (B) 資料鏈結層（Data-Link Layer） 
    (C) 網路層（Network Layer） (D) 應用層（Application Layer）
    
    實體層
    資料鏈結層
    網路層
    應用層
    
---
### 作業系統 資訊安全策略:
---

    請問針對作業系統訂定的資訊安全策略中，
    下列何種安全模式中「檔案持有者」可授權決定「其他使用者」存取該檔案的權限？ 
    (A) 自由存取控制（Discretionary Access Control，DAC） 
    (B) 強制性存取控制（Mandatory Access Control，MAC） 
    (C) 角色存取控制（Role-based Access Control，RBAC） 
    (D) 屬性存取控制（Attribute-based Access Control，ABAC） 

---

---

    自由存取控制（Discretionary Access Control，DAC） 
    1.根據主體（如用戶、進程或 I/O 設備等）的身份和他所屬的組限制對客體的訪問。
    2.可以直接（或間接）地將訪問權限賦予其他主體（除非受到強制存取控制的限制）。
    
    強制性存取控制（Mandatory Access Control，MAC） 
    1.通常是一個行程或執行緒，物件可能是檔案、目錄、TCP/UDP埠、共享記憶體段、I/O裝置等。主體和物件各自具有一組安全屬性。
    2當主體嘗試存取物件時，都會由作業系統核心強制施行授權規則——檢查安全屬性並決定是否可進行存取。
    3任何主體對任何物件的任何操作都將根據一組授權規則（也稱策略）進行測試，決定操作是否允許。在資料庫管理系統中也存在存取控制機制。
    
    角色存取控制（Role-based Access Control，RBAC）
    1.不同於強制存取控制以及自由選定存取控制
    2.將【權限賦予角色】
    
    屬性存取控制（Attribute-based Access Control，ABAC） 
    1.存取控制
    
---

---
    請問此 cat ~/.bash_history 指令的目的為?
    (A) 列出使用者目錄
    (B) 列出系統目錄 dir
    (C) 列出使用者曾經下過的指令  cat ~/.bash_history 
    (D) 列出系統安裝歷史
---

