# 原來你在做這個 — Podcast 網站

主持人：子柏（曾子柏）。這個 repo 是節目的官方網站，用 GitHub Pages 架站，之後會接上網域 wydzp.com（尚未購買）。

## 結構
- `index.html`：整個網站，單一檔案（HTML + CSS 都在裡面，沒有 build 步驟）。
- `.nojekyll`：讓 GitHub Pages 直接提供檔案，不經過 Jekyll。

## 頁面排版（請維持）
1. 最上面：節目名稱、一句定位、主持人。
2. 收聽分流：紅色主按鈕「網頁直接聽」（Firstory），下面 YouTube / Apple Podcasts / Spotify / KKBOX / Pocket Casts。
3. 集數跳轉按鈕（#ep4、#ep3…），網址加 #epN 可直接停在該集。
4. 每集一張「來賓工作卡」，新的在上：集數＋日期、標題、來賓姓名＋職稱、一段「他在做什麼」、三個重點、「收聽這集」＋連到來賓單位的按鈕、資料來源。
5. 不要放來賓姓氏的圓形頭像（主持人要求拿掉）。

## 平台連結
- Firstory（所有平台）：https://open.firstory.fm/user/cmp20wl3c0dck01wd58iuanfn
- YouTube：https://www.youtube.com/@WYDZP
- Apple Podcasts：https://podcasts.apple.com/tw/podcast/id6828685996
- Spotify：https://open.spotify.com/show/7EGUvdtVhwmiSWgUsp4kiA
- KKBOX：https://podcast.kkbox.com/tw/channel/P_NxOT1b7808rfP76C
- Pocket Casts：https://pca.st/pyt0hct4

## 集數
- EP1（2026.11.04）林宇凡｜MR. LIVING 居家先生 共同創辦人 → mrliving.com.tw
- EP2（2026.11.07）劉柏良｜老永昌碾米廠 第五代執行長 → 目前連 Google 地圖（待換官網）
- EP3（2026.11.15）葉時昊 Hank Yeh｜工研院資通所 副經理 → itri.org.tw
- EP4（即將上架）郭明宗｜小叮噹科學主題樂園 總經理 → 目前連 Google 地圖（待換官網）；標題是暫定的
- 預告：楊玉玲｜心路基金會 處長 → 心路官網與捐款頁（加 UTM，註明節目不經手款項）

## 待辦
- 「收聽這集」目前都連 YouTube 頻道首頁，要換成各集單集連結。
- EP4 正式標題、上架日期。
- 老永昌、小叮噹的官網或粉專網址。
- 買好 wydzp.com 後：加 `CNAME` 檔（內容 `wydzp.com`），在註冊商設定 DNS 指向 GitHub Pages。

## 內容原則
- 來賓資料只寫查得到出處或來賓本人確認過的內容，每張卡片底下列資料來源。
- 職稱以主持人提供的為準，上線前請來賓確認。
- 捐款連結一律連到對方官網，並註明節目不經手任何款項。
