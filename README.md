# 🌱 Green-Contributions

这是一个通过 GitHub Actions 自动生成提交记录的仓库，旨在帮助你保持 GitHub 贡献图的活跃度。只需配置一次，即可实现：

- **每天自动提交**：北京时间 4:00 自动生成多次提交（默认 12 次），让你的贡献格每天保持深绿色。
- **批量填充历史**：支持手动触发，一次性生成从指定日期到今天的提交记录，用于补全过去的贡献日历。

## 🚀 快速开始

1. **创建仓库**：在 GitHub 上创建一个新仓库（推荐设为 Private）。
2. **添加工作流**：在仓库中创建 `.github/workflows/fill-history.yml` 文件。
3. **修改配置**：将文件中的 `user.email` 和 `user.name` 修改为你自己的 GitHub 账号信息。
4. **开启权限**：在仓库设置中开启 Actions 的写权限（Settings -> Actions -> General -> Workflow permissions -> Read and write permissions）。
5. **手动运行**：在 Actions 页面手动触发一次以补全历史或测试功能。

## ⚠️ 注意事项

- 邮箱必须与 GitHub 账号验证的邮箱一致。
- 批量填充会执行强制推送（`git push --force`），请确保仓库中没有其他重要代码。
