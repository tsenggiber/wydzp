# 原來你在做這個 — Podcast 網站

主持人：子柏（曾子柏）。這個 repo 是節目的官方網站，用 GitHub Pages 架站。GitHub 專案在 wydzp 組織底下：wydzp/wydzp.github.io（主持人個人帳號是組織管理員；不要搬回個人帳號，網址不要露出個人帳號名稱）。正式網址 https://wydzp.github.io/ ，之後會接上網域 wydzp.com（尚未購買）。push 到 main 就自動上線。

## 結構
- `index.html`：整個網站，單一檔案（HTML + CSS 都在裡面，沒有 build 步驟）。
- `.nojekyll`：讓 GitHub Pages 直接提供檔案，不經過 Jekyll。

## 頁面排版（請維持）
1. 最上面：節目名稱、一句定位、主持人。
2. 收聽分流：六個一樣大的按鈕（兩欄三列），順序 YouTube、Spotify、Apple Podcasts、KKBOX、Pocket Casts、「網頁直接聽」（Firstory，免裝 App）。不放大的紅色主按鈕（主持人要求拿掉）。
3. 集數跳轉按鈕（#ep4、#ep3…），網址加 #epN 可直接停在該集。
4. 每集一張「來賓工作卡」：最上面是「下集預告」（還沒上架那集），接著「後續預告」，再來已上架的集數新的在上：集數＋日期、標題、來賓姓名＋職稱、一段「他在做什麼」、三個重點、「▶ 收聽這集」小標＋YouTube / Spotify / Apple 三顆一樣大的單集按鈕，下一行是連到來賓單位的按鈕、資料來源。
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
- 楊玉玲｜心路基金會 處長 → 卡片已先從網站拿掉（一次只預告一集）。EP4 上架後再放回來當「下集預告」：完整卡片在 commit 736b96c 的 index.html（`<article class="ep soon" id="next">`，含捐款連結與 UTM、註明節目不經手款項）。

## 待辦
- 更新節奏：每週六上架正片（首頁有「每週六更新」標籤），週五放預告。
- 還沒上架的那一集：卡片用 `ep soon` 樣式＋「下集預告」標籤，不放收聽按鈕，改放「週六上架後開放收聽」。上架後改回一般卡片、加 YouTube / Spotify / Apple 三顆單集按鈕、標籤換成日期。
- EP1–EP3 已有三平台單集連結；EP4 目前是「下集預告」。Spotify 單集網址可從 open.spotify.com 節目頁讀，Apple 用 itunes.apple.com/lookup?id=6828685996&entity=podcastEpisode 查。
- EP2 在 Firstory（同步到 Spotify / Apple）的標題還寫「碾米廠二代」，要到 Firstory 後台改成「第五代」。YouTube 和網站已改好。
- EP4 正式標題、上架日期。
- 老永昌、小叮噹的官網或粉專網址。
- 買好 wydzp.com 後：加 `CNAME` 檔（內容 `wydzp.com`），在註冊商設定 DNS 指向 GitHub Pages；index.html 的 canonical、og:url、JSON-LD url 和 robots.txt、sitemap.xml 裡的網址都要改成 https://wydzp.com/。
- 有節目封面圖後：加 og:image（建議 1200×630）並把 twitter:card 改成 summary_large_image。
- Google Search Console 已用 HTML 檔驗證：google552648b5ef2c90eb.html 必須一直留著，刪掉會失去驗證。

## 內容原則
- 來賓資料只寫查得到出處或來賓本人確認過的內容，每張卡片底下列資料來源。
- 職稱以主持人提供的為準，上線前請來賓確認。
- 捐款連結一律連到對方官網，並註明節目不經手任何款項。
