# lumiphone-cn

Lumi Phone 域名站仓库，仅用于 [https://www.lumiphone.cn/](https://www.lumiphone.cn/)。

本仓库不含业务源码。GitHub Actions 会从正式仓库 `Lumi-Phone` 拉取代码构建并部署到 Pages。

## 主仓私密后必配

在本仓 **Settings → Secrets and variables → Actions** 添加：

| Name | 说明 |
|------|------|
| `GH_PAT` | Fine-grained Token：可读 `Lumi-Phone` Contents；主仓触发同步时还需能对本仓跑 Actions |
| `VITE_DISCORD_CLIENT_ID` | Discord 应用 Client ID（与主仓相同） |

主仓 `Lumi-Phone` 也需配置同名 `GH_PAT`，以便正式站部署成功后自动触发本仓同步。
