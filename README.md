# 社會技巧配音課 Skill（dubbing-lesson）

讓學生替卡通短片逐句配音，當場把全班的聲音合成影片一起看，再用撲克牌局練習同樣的句型。

給 AI 一個社會技巧主題，它會先跟你討論劇本，再做出：

- **互動簡報**：一個 HTML 檔，含配音室、首映與 MP4／WebM 影片合成
- **A4 學習單**：一頁學習單，加一頁老師剪卡

## 特色

- **不用後端、不用帳號**：只靠瀏覽器內建功能，也不依賴外部程式庫
- **聲音不上傳**：錄音只存在教室那台電腦的瀏覽器
- **可以重錄**：每句錄完自動播放，不滿意再錄一次；前後空白和音量會自動處理
- **附完整範例**：〈換不換？好好拒絕〉用「借手機」情境練習拒絕，搭配「交換牌」牌局，約 45 分鐘

## 怎麼用

### 直接用範本上課

下載 `assets/slides-template.html` 和 `assets/worksheet-template.html`，放到支援 https 的網站（例如 GitHub Pages），或用本機伺服器開啟：

```bash
python -m http.server
```

再用 Chrome 或 Edge 開啟，上課前先試錄一句並跑一次首映。

### 當成 AI Skill 使用

把整個資料夾放到 Claude Code 的 skills 資料夾：

```bash
git clone https://github.com/chuoneone/social-skills-dubbing ~/.claude/skills/dubbing-lesson
```

然後說：「幫我做一堂配音課，主題是加入別人的遊戲，七年級 5 個人，一節課。」

## 需要的環境

- Chrome 或 Edge（影片格式依瀏覽器版本而定，新版多半是 MP4，否則是 WebM）
- 教室電腦有麥克風
- 透過 https 或 localhost 開啟；直接雙擊檔案時麥克風權限可能不穩

## 使用提醒

學生的聲音是個人資料。影片若要公開分享，請另外取得學生與監護人同意；下課可在首映頁按「下課清除所有錄音」。
