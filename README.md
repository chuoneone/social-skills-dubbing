# 配音課 Skill（dubbing-lesson）

讓學生替卡通短片逐句配音，當場把全班的聲音合成影片一起看。

## 使用流程

安裝後，告訴 AI「我想做一堂配音課」，它會：

1. **先問你想教什麼**，以及學生年級、人數與可用時間
2. **跟你討論劇本**，提出方向、寫出台詞，改到你滿意為止
3. **等你同意才開始製作**，做出配音簡報，需要時附上 A4 學習單

## 特色

- **不用後端、不用帳號**：只靠瀏覽器內建功能，也不依賴外部程式庫
- **聲音不上傳**：錄音只存在教室那台電腦的瀏覽器
- **可以重錄**：每句錄完自動播放，不滿意再錄一次；前後空白和音量會自動處理
- **當場看成果**：按下首映就播放並合成影片，可下載 MP4 或 WebM
- **附完整範例**：〈手機借我玩一下〉用借手機的情境練習拒絕，約 25 分鐘

## 怎麼用

### 當成 AI Skill 使用

把整個資料夾放到 Claude Code 的 skills 資料夾：

```bash
git clone https://github.com/chuoneone/social-skills-dubbing ~/.claude/skills/dubbing-lesson
```

然後說：「我想做一堂配音課。」

### 直接用範例上課

下載 `assets/slides-template.html` 和 `assets/worksheet-template.html`，放到支援 https 的網站（例如 GitHub Pages），或用本機伺服器開啟：

```bash
python -m http.server
```

再用 Chrome 或 Edge 開啟，上課前先試錄一句並跑一次首映。

## 需要的環境

- Chrome 或 Edge（影片格式依瀏覽器版本而定，新版多半是 MP4，否則是 WebM）
- 教室電腦有麥克風
- 透過 https 或 localhost 開啟；直接雙擊檔案時麥克風權限可能不穩

## 使用提醒

學生的聲音是個人資料。影片若要公開分享，請另外取得學生與監護人同意；下課可在首映頁按「下課清除所有錄音」。

## 授權

[MIT](LICENSE)：可以自由使用、修改與分享，請保留授權聲明。
