# image

[![validate-images](https://github.com/gehlelwira-wq/image/actions/workflows/validate-images.yml/badge.svg)](https://github.com/gehlelwira-wq/image/actions/workflows/validate-images.yml)

一个用于测试 GitHub 图片/文件托管与 SSH push/pull 链路的仓库。

## 在线预览

GitHub Pages 启用后访问：<https://gehlelwira-wq.github.io/image/>

## 内容

- [`images/hello-dsh.svg`](images/hello-dsh.svg) — 由 DSH 推送的示例 SVG
- [`images/README.md`](images/README.md) — 图片目录说明
- [`LICENSE`](LICENSE) — Apache License 2.0

## 添加图片

1. 把图片放进 `images/`（支持 SVG/PNG/JPG/GIF/WebP）。
2. SVG 会在 push 后由 GitHub Actions 自动做 XML 校验。
3. 提交并推送：

```bash
git add images
git commit -m "Add image: <name>"
git push
```

## 克隆

```bash
git clone git@github.com:gehlelwira-wq/image.git
```

> 本机已配置 `url.git@github.com:.insteadOf https://github.com/`，直接复制 HTTPS 地址也会自动改用 SSH。

## 最近验证

- 2026-10-18：SSH push / pull、全新 clone、GitHub Actions 自动校验均已配置。
