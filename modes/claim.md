---
description: 保護您的建築不被壞
icon: house-lock
---

# 領地

### 1. 選取區域

* 使用木鋤頭
* `/res select [x y z]`：選取長寬高範圍（以自身為中心）。
* `/res select chunk`：選取目前所在的整個區塊（Chunk）。
* `/res select expand [數量]`：朝視線方向擴張選取範圍。
* `/res select shift [數量]`：朝視線方向移動選取範圍。
* `/res select size`：顯示當前選取範圍的大小。

***

### 2. 建立領地

* `/res create [領地名]`：創建領地。
* `/res remove [領地名]`：刪除領地。
* `/res removeall`：刪除你擁有的所有領地。
* `/res confirm`：確認刪除指令。
* `/res subzone [子領地名]`：在現有領地內創建子領地（須為領地擁有者）。
* `/res auto [領地名] [半徑]`：以自身為中心，在權限許可範圍內自動創建最大領地。
* `/res area [add/remove/replace] [區域ID]`：對領地增加、移除或替換實體區域。

***

### 3. 權限標籤(權限)

此部分用於控制玩家行為。參數通常為 `[true/false/remove]`。

* `/res set [flag] [參數]`：設置領地全域權限。
* `/res pset [玩家名] [flag] [參數]`：設置特定玩家權限。
* `/res gset [群組名] [flag] [參數]`：設置特定群組權限。
* `/res padd [玩家名]`：快速添加玩家至信任名單（同 `pset trusted true`）。
* `/res pdel [玩家名]`：將玩家從信任名單中移除。
* `/res clearflags`：清除領地內所有已設置的標籤。
* `/res reset <residence/all>`：將領地恢復為預設權限標籤。
* `/res check [領地名] [flag] [玩家名]`：檢查特定玩家在該領地的標籤狀態。
* `/res flags`：列出所有可用的標籤（Flags）。
* `/res lset [blacklist/ignorelist] [物品ID]`：管理領地的黑名單或忽略名單。

***

### 4. 資訊查詢

* `/res list [玩家名]`：列出你或特定玩家擁有的領地。
* `/res listall`：列出全服所有領地。
* `/res info [領地名]`：查詢領地詳細資訊（座標、標籤、擁有者）。
* `/res current`：顯示目前站立位置的領地名稱。
* `/res show`：顯示當前領地的物理邊界。
* `/res limits`：顯示你目前受到的領地限制（數量、大小）。
* `/res sublist [領地名]`：列出該領地內的所有子領地。
* `/res area list [領地名]`：列出該領地包含的所有實體區域及其座標。

***

### 5. 其他指令

* `/res tp [領地名]`：傳送到指定領地。
* `/res tpset`：在目前位置設置領地傳送點。
* `/res tpconfirm`：忽略傳送安全警告並強制傳送。
* `/res unstuck`：當卡在領地內時，將自己移至領地外。
* `/res give [領地名] [玩家名]`：將領地所有權轉讓給他人。
* `/res rename [舊名] [新名]`：更改領地或子領地名稱。
* `/res expand [數量]`：朝視線方向擴張已存在的領地規模。
* `/res contract [數量]`：朝視線方向縮小已存在的領地規模。
* `/res message [領地名] [enter/leave] [內容]`：設置進出領地時的提示訊息（可用 `remove` 刪除）。
* `/res mirror [來源領地] [目標領地]`：將權限設置從一個領地複製到另一個。
* `/res kick`：將特定玩家踢出領地。
* `/res command <allow/block/list>`：在領地內允許或封鎖特定指令的使用。
* `/res compass`：將指南針指向領地位置。
* `/res setmain`：設定主領地，使其名稱顯示在聊天頻道前綴。

