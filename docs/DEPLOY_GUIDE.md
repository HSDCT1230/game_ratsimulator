# 鼠鼠模拟器 GitHub Pages 部署说明

## 发布文件

仓库根目录保留与 1.0 对齐的正式运行结构：

```text
index.html
bgm/
sound effect/
```

这三项就是 GitHub Pages 需要读取的 2.0 正式版本。`archive/v1.0/` 是旧版归档，`docs/` 和 `tools/` 是维护资料，不影响网页入口。

## 启用 GitHub Pages

1. 打开仓库 `HSDCT1230/game_ratsimulator`。
2. 进入 `Settings` -> `Pages`。
3. Source 选择 `Deploy from a branch`。
4. Branch 选择 `main`，Folder 选择 `/ (root)`。
5. 保存后等待 GitHub Pages 自动部署。

## 更新版本

更新 2.0 或后续版本时，保持根目录文件名不变：

- `index.html`
- `bgm/`
- `sound effect/`

这样旧的访问链接不会变化。需要保留旧版本时，将旧版按同样结构放入 `archive/v版本号/`。
