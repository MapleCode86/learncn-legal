# RealChinese Legal Pages

隐私政策与服务条款的公开页面（GitHub Pages 托管）。

- `privacy-policy.html` — Privacy Policy（English only, covers iOS + Google Play）
- `terms-of-use.html` — Terms of Use（English only, covers iOS + Google Play）

## 发布到 GitHub Pages（一次性）

1. 在 GitHub 新建仓库 `learncn-legal`（公开）。
2. 把本目录全部文件推上去（master 或 main 均可）：
   ```bash
   cd learncn-legal
   git init
   git add .
   git commit -m "Add LearnCN legal pages"
   git branch -M main
   git remote add origin https://github.com/MapleCode86/learncn-legal.git
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source 选 `main` 分支 `/ (root)`，保存。
4. 几分钟后访问：
   - https://maplecode86.github.io/learncn-legal/privacy-policy.html
   - https://maplecode86.github.io/learncn-legal/terms-of-use.html

## 应用内链接常量（Assets/Scripts/AppConstants/AppConstants.cs）

```
public const string PrivacyPolicyURL = "https://maplecode86.github.io/learncn-legal/privacy-policy.html";
public const string TermsOfUseURL    = "https://maplecode86.github.io/learncn-legal/terms-of-use.html";
```

> 若仓库改名，记得同步更新上面两个 URL。
