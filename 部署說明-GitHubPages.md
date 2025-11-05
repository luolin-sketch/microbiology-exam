# GitHub Pages 部署說明

## 永久免費的部署方式

### 前置需求
- GitHub帳號（免費註冊：https://github.com/signup）

### 步驟一：創建GitHub倉庫
1. 登入GitHub
2. 點擊右上角「+」→「New repository」
3. 設定：
   - Repository name: `microbiology-exam`
   - 選擇「Public」（公開）
   - 不勾選任何初始化選項
4. 點擊「Create repository」

### 步驟二：上傳網站檔案
解壓縮 `microbiology-exam-deploy.zip` 後，有兩種上傳方式：

#### 方式A：網頁上傳（簡單）
1. 在倉庫頁面點擊「uploading an existing file」
2. 將所有檔案拖放到上傳區域：
   - `index.html`
   - `favicon.ico`
   - `assets` 資料夾（需要先壓縮或逐個上傳資料夾內檔案）
3. 在底部填寫commit訊息：`Initial commit`
4. 點擊「Commit changes」

#### 方式B：使用Git命令（進階）
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/microbiology-exam.git
git push -u origin main
```

### 步驟三：啟用GitHub Pages
1. 在倉庫頁面點擊「Settings」
2. 左側選單點擊「Pages」
3. 在「Source」下：
   - Branch: 選擇 `main`
   - Folder: 選擇 `/ (root)`
4. 點擊「Save」

### 步驟四：訪問網站
等待1-2分鐘後，您的網站將可通過以下網址訪問：
```
https://YOUR_USERNAME.github.io/microbiology-exam/
```

## 自訂域名（可選）
如果您有自己的域名，可以在GitHub Pages設定中綁定。

## 更新網站
如需更新內容，只需：
1. 上傳新的檔案到倉庫
2. GitHub Pages會自動重新部署

## 網站資訊
- **教授**：余美萱教授
- **題庫**：418題（考古題60 + 國考風格163 + AI生成195）
- **功能**：完整的線上考試系統

## 優點
- ✅ 完全免費
- ✅ 永久有效
- ✅ 支援HTTPS
- ✅ 可綁定自訂域名
- ✅ 自動備份（Git版本控制）

## 需要幫助？
GitHub Pages文件：https://docs.github.com/pages

