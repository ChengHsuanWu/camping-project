# 🏕️ 12/11~12/13 三天兩夜情侶露營精選企劃 (Camping Project)

本專案為針對 **2026/12/11 (五) ～ 12/13 (日)** 三天兩夜情侶露營精心調研整理之互動式 GIS 選址工具與企劃檔案。

---

## 🎯 核心需求指標

1. **地理範圍**：台中（含）以北（新竹、苗栗、台中、桃園）。
2. **營位隱私**：**單帳一區 / 獨立小包區**，階梯或林木遮蔽，確保寧靜不被鄰帳干擾。
3. **免搭帳輕露營**：非動輒萬元的奢華包餐渡假村，而是營區**幫忙搭好帳篷並附睡墊**（自煮炊事保留野趣）。
4. **必備硬體**：冷熱飲水機、五星級高評價乾淨衛浴（無異味、水壓足）。
5. **★ 加分項**：**洗手台水槽具備溫熱水**（寒冬洗菜洗碗去油不凍手）。

---

## 📂 專案檔案結構

```
camping-project/
├── index.html           # 核心互動式網頁 (整合 GIS 地圖、官方訂位連結、實景卡片)
├── camps_data.json      # 10 大營區結構化數據 (含 GPS 經緯度、海拔、走廊標籤)
├── README.md            # 專案與露營選址詳細說明文件
└── camping-project.zip  # 打包好的壓縮檔 (方便直接下載/傳輸/上傳雲端)
```

---

## 🗺️ GIS 地圖圖資說明

本專案網頁 (`index.html`) 已串接台灣本地圖資與國際圖資，於右上角可一鍵切換：
- **內政部國土測繪中心 (NLSC) 台灣通用電子地圖 (WMTS)**：官方在地最權威圖資。
- **Google 地形等高線圖 (Terrain)**：立體山脈等高線，露營看山勢極為實用。
- **Google 標準道路圖 (Roadmap)**：一般導航。
- **國土測繪中心 衛星正射影像 (PHOTO_MIX)**：高空鳥瞰空拍圖。
- **CartoDB Voyager 探險地圖**：商用備援圖磚。

---

## ⛺ 10 大精選營區總覽

| # | 營區名稱 | 縣市 / 海拔 | 單帳一區型態 | 免搭帳模式 | 水槽熱水 | 官方訂位連結 |
|---|---|---|---|---|:---:|---|
| 01 | **尖石・怡然自德** | 新竹尖石 (1,050m) | 梯田階梯獨立少帳區 | 專人代搭帳＋乳膠床 | 🔥 有 | [露營樂訂位](https://www.easycamp.com.tw/Store_2499.html) |
| 02 | **南庄・慢生活** | 苗栗南庄 (300m) | D區獨立雨棚雙人專用 | Coody 充氣帳免搭 | 衛浴有 | [慢生活官網](https://slowlifecamp2016.com/) |
| 03 | **泰安・日光角落** | 苗栗泰安 (830m) | 邊角景觀獨立位 | 特約裝備代搭/露營車 | 🔥 有 | [愛露營訂位](https://m.icamping.app/store/rgjl1119) |
| 04 | **南庄・搭漾 (Tayal)**| 苗栗南庄 (940m) | 高台獨立單帳位 | 裝備出租可協搭 | 🔥 有 | [官方粉專](https://www.facebook.com/tayalcamp/) |
| 05 | **尖石・老爹打樁** | 新竹尖石 (1,200m) | 獨立階梯輕裝小屋 | 不打樁輕露營木屋 | 🔥 有 | [老爹打樁官網](https://pilingdaddy.com/) |
| 06 | **五峰・鹿林道** | 新竹五峰 (800m) | 杉木林獨立少帳棧板 | 全套出租＋專人代搭收 | 衛浴有 | [鹿林道官網](https://www.lulin.com.tw/) |
| 07 | **三灣・鄉町** | 苗栗三灣 (100m) | 厚草皮邊角獨立位 | 帳篷睡墊出租代搭 | 🔥 有 | [露營樂訂位](https://www.easycamp.com.tw/Store_2542.html) |
| 08 | **泰安・司馬限雲端**| 苗栗泰安 (1,200m) | 橘1A等1~2帳獨立包區 | 官網明定出租可代搭 | 衛浴有 | [司馬限官網](https://sihmasian.com/) |
| 09 | **石岡・九甲林** | 台中石岡 (450m) | 樹林木平台前庭 | 南非狩獵帳自煮免搭 | 衛浴有 | [露營樂訂位](https://www.easycamp.com.tw/Store_2384.html) |
| 10 | **拉拉山・天恩農場**| 桃園復興 (1,550m) | 獨立雨棚前庭動線 | 狩獵帳(附卡式爐/鍋具) | 衛浴有 | [露營樂訂位](https://www.easycamp.com.tw/Store_2368.html) |

---

## 🚀 如何移植到遠端專案 (Remote Project)

### 方法一：推送到 GitHub / GitLab 遠端儲存庫 (建議)
```bash
cd camping-project
git init
git add .
git commit -m "feat: complete camping selection with GIS map and booking links"
git branch -M main
git remote add origin <你的遠端Repo網址>
git push -u origin main
```
> **提示**：若在 GitHub 設定中開啟 **GitHub Pages** (Settings -> Pages -> Branch: main -> /root)，即可直接獲得一個公開 HTTPS 網址，你跟女友在手機上隨時點開就能看！

### 方法二：部署至 Vercel / Netlify 一秒上線
- 將本專案資料夾直接拖曳至 [Netlify Drop](https://app.netlify.com/drop) 或透過 Vercel CLI：
```bash
npx vercel
```
立即產生專屬公開網址供手機即時瀏覽。

### 方法三：透過 SSH / Remote Workspace 開啟
若是在遠端 Linux/Cloud 主機上開發：
- 直接將 `camping-project.zip` 上傳並解壓縮至遠端伺服器工作目錄：
```bash
unzip camping-project.zip -d ~/camping-project
```
- 在 VS Code / Antigravity 按 `F1` 選擇 `Remote-SSH: Connect to Host...` 開啟該目錄即可繼續協作！
