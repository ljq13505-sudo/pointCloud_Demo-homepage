# 独立主页仓库的手动发布

本地目录：`D:\chatgpt_working\pointCloud_Demo-homepage`。

此仓库和 pointCloud_Demo 算法仓库各有自己的 `.git`、提交历史及 origin。应在这个主页目录执行以下命令。

## 1. 创建 GitHub 空仓库

在账号 ljq13505-sudo 下创建 **pointCloud_Demo-homepage**，公开展示时选择 Public，不勾选自动生成 README、.gitignore 或 License。

## 2. 手动提交

本地已执行 git init -b main。填写你自己的提交邮箱后再执行：

```powershell
Set-Location 'D:\chatgpt_working\pointCloud_Demo-homepage'
git config user.name "ljq13505-sudo"
git config user.email "你的真实提交邮箱"
git status
git add .
git diff --cached --stat
git commit -m "Add point cloud project homepage"
git remote add origin https://github.com/ljq13505-sudo/pointCloud_Demo-homepage.git
git push -u origin main
```

## 3. 开启 GitHub Pages

仓库 Settings → Pages → Source 选择 Deploy from a branch → Branch 选择 main → Folder 选择 **/(root)** → Save。

这里选择仓库根目录，因为 index.html 直接在根目录；不选 /docs。

部署完成后访问 `https://ljq13505-sudo.github.io/pointCloud_Demo-homepage/`。

后续修改页面，执行 git add、git commit 和 git push；Pages 会按配置更新网站。
