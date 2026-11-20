# Monday Marketing · IG 內容管理台

公開網站：任何人都可以睇；編輯名單上嘅同事撳「團隊登入」用 email 連結登入後可以編輯。

- 資料庫：Supabase 專案 `mm-ig-desk`（Singapore）
- 趨勢參考：每日早上 7:40（香港時間）由 Claude 排程自動搜尋並加入 Supabase `trends` 表
- 加 / 減編輯：Supabase → SQL Editor
  ```sql
  insert into public.editors (email) values ('name@company.com');
  delete from public.editors where email = 'name@company.com';
  ```
