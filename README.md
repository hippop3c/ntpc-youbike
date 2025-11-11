# ntpc-youbike — GitHub Pages 部署說明

## 一鍵部署（新手建議）
1. 到 GitHub 建立 **新的公開 Repository**，名稱可用 `ntpc-youbike`（或任意）。
2. 上傳本資料夾內全部檔案：
   - `index.html`
   - `.nojekyll`
   - `README.md`（可選）
3. 進入 **Settings → Pages**：
   - Source：選 **Deploy from a branch**
   - Branch：選 **main**（或你預設分支），資料夾選 **/**（root）
4. 儲存後等 1～2 分鐘，網站會出現在：`https://<你的帳號>.github.io/<repo-name>/`。

## 若需要自訂網域（選用）
- 到網域 DNS 新增 CNAME 指向 `<你的帳號>.github.io`。
- 在 Repo 根目錄新增 `CNAME` 檔案，內容填你的網域（例如 `bike.example.com`）。

## 本地預覽（避免 file:// CORS）
```bash
python -m http.server 8080
# 然後打開 http://localhost:8080
```
