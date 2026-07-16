# 鼠鼠模拟器 2.0

一个纯静态 HTML 鼠鼠养成小游戏。当前正式入口是仓库根目录的 `index.html`。

## 本地运行

双击 `run-local.cmd`，或直接用浏览器打开 `index.html`。

## 目录结构

```text
index.html          2.0 游戏主文件
bgm/                2.0 背景音乐
sound effect/       2.0 正式音效资源
CREDITS.md          音频素材来源、license 与转码说明
archive/v1.0/       1.0 本地版本归档（已忽略，不提交、不发布）
docs/               规则备忘、部署说明、下载证明保管
tools/              开发辅助工具和已接入音效试听页
run-local.cmd       本地快速打开游戏
```

## 发布

`main` 推送到 GitHub 后，由 Cloudflare Pages 自动部署。生产地址：

https://game-ratsimulator.pages.dev/

`archive/` 是本地历史版本目录，已由 `.gitignore` 排除，不进入 GitHub 或线上站点。正式运行资源保持在 `index.html`、`bgm/` 和 `sound effect/`。

## 音频版权处理

- 完整音频来源见 `CREDITS.md`。
- Pixabay BGM 的证明材料保管在 `docs/pixabay-download-proof/`。
- `please-help-me` 已替换为 Mixkit `Creature cry of hurt`，`snap1` 已替换为 Mixkit `Impact of a blow`；当前正式绑定可在 `tools/sfx-replacement-candidates.html` 试听确认。
