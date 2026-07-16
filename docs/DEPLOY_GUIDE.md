# 鼠鼠模拟器 Cloudflare Pages 部署说明

## 发布方式

GitHub 仓库 `HSDCT1230/game_ratsimulator` 的 `main` 分支与 Cloudflare Pages 项目 `game-ratsimulator` 连接。推送到 `main` 后由 Cloudflare 自动部署：

https://game-ratsimulator.pages.dev/

## 正式运行文件

正式游戏入口和资源保持在：

```text
index.html
CREDITS.md
bgm/
sound effect/
```

`archive/` 只保存于本机，并由 `.gitignore` 排除，因此不会进入 GitHub 或 Cloudflare 部署。`docs/` 与 `tools/` 是维护资料，不被游戏入口引用。

## 更新版本

更新游戏时保持正式运行路径稳定：

- `index.html`
- `bgm/`
- `sound effect/`

旧版本代码可以继续放入本机 `archive/v版本号/`，不要强制加入 Git，也不要把旧版音频或未确认来源素材发布到线上。

## 发布后校验

1. 确认 GitHub 远端 `main` SHA 与本地提交一致。
2. 确认该提交的 `Cloudflare Pages` check run 为 `completed/success`。
3. 打开生产首页并核对本次版本标记、关键音频路径和归档目录不可访问。
