# MathApp — 私隱政策 + 支援頁

App Store 上架必填嘅兩條 URL,行 GitHub Pages(免費、靜態、無後台)。

| 頁 | 檔案 | URL |
|---|---|---|
| 私隱政策 | `privacy/index.html` | https://coldryan.github.io/mathapp/privacy/ |
| 支援 | `support/index.html` | https://coldryan.github.io/mathapp/support/ |

## 點改

改完 push 上 `main` 就會自動重新部署(大約 1 分鐘)。

```bash
cd ~/Codes/mathapp && git add -A && git commit -m "docs: 改咩" && git push
```

## 硬規矩

- **改咗 app 收集/傳送嘅資料,呢兩頁一定要跟住改。** 三邊要對得返:
  `WiseSage/PrivacyInfo.xcprivacy` · App Store Connect 嘅 privacy nutrition label · 本頁。
  對唔返 = 審核打回。真相層見 `~/Codes/WiseSage/docs/app/07_遙測與閃退報告.md` §4 私隱合約。
- 改內容記得同時更新兩頁底部同 header 嘅日期。
- 中英文對照:中文為準(私隱政策入面寫明咗)。

## 未做

- [ ] **支援 email 未落** — `support/index.html` 同 `privacy/index.html` 各有一段
      `<!-- TODO -->` HTML comment,email 一決定就 uncomment 填返。
      Apple Guideline 1.5 要求支援頁有可用聯絡途徑,**送審前必補**。
