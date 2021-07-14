# 安裝需求：
```cmd
1. 安裝git (windows版本)
```
# 建立　III-devops專案
1. 我是選擇>> python+flask+sqlib範本
2. 建立完，會自動跑pipeline測試流程

# 建立　遠端Reposity
```
登入III-gitlab>>新增航港局初始專案 (如：airpotMg) 
```
# 拉　專案到本地端(`D`目錄下)
```cmd
C:\WINDOWS\>> D: # 進入　D: 目錄
D:\>> git clone https://gitlab.com/sicachang/airportMg.git 　# 專案下載到Ｄ目錄下
D:\>> cd airportMg # 進入剛clone後新增的資料夾 D:\airpotMg
D:\cd airportMg\ # 已進入D:\cd airportMg\目錄
```
# 複製　初始程式碼
```git
將航港局專案內容複製到　D:\airpotMg　# 手動複製
```
# 更新　目錄
```git
D:\airportMg>> git add -f . # 表示更新D:\airportMg目錄
D:\airportMg>> git commit -m "已將航港局專案內容複製過來！！！" # 需透過　git commit 提交更新
```

# 提交　更新 (此步驟執行後，iii-deveops會自動啟動測試、部屬等流程)
```git
D:\airportMg>> git push origin main:main
```
1. origin # 此為III-gitlab剛剛複製的目錄位址如：https://gitlab.com/sicachang/airportMg.git #　剛`git clone`時，git已自動將此網址設定為 'origin'
2. main:main ＃前者為本地端分支　`main` 後者　`main` 為III-gitlab/airportMg 上的遠端分支



