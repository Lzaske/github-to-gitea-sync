# github-to-gitea-sync

通过 GitHub Actions 将 `Lzaske` 账号下的全部 GitHub 仓库镜像同步到自建 Gitea。

## 行为说明

- 同步对象：Git 提交历史、分支、标签
- 不同步：Issues、Pull Requests、Release 附件、Wiki、权限设置
- Gitea 端仓库应视为只读镜像仓库

## 触发方式

- 手动触发：`workflow_dispatch`
- 定时触发：每 6 小时一次
