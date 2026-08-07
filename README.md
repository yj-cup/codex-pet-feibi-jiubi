# Codex 宠物：菲比啾比

菲比啾比是一个 Codex 兼容的 v2 动画宠物。角色采用 Q 版风格：金色长发、紫色大眼、蓝白宽檐帽与蓝黑白制服。

![动作预览](preview/contact-sheet.png)

## 文件

- `pet.json`：宠物清单。
- `spritesheet.webp`：8 列 × 11 行透明动画精灵表。
- `preview/contact-sheet.png`：动作总览。
- `preview/look-directions.png`：16 个观察方向预览。
- `qa/`：结构、方向语义及盲测验证结果。

## 动画

包含 idle、running-right、running-left、waving、jumping、failed、waiting、running、review，以及两行 16 方向观察动画。

- 待机时会眨眼、左右张望并挥手。
- 指针触碰宠物时会挥手回应，不再蹲下。

## 安装

将本仓库复制到 Codex 宠物目录：

```text
%USERPROFILE%\.codex\pets\feibi-jiubi
```

目录中必须保留 `pet.json` 与 `spritesheet.webp`。

## 验证

- `spriteVersionNumber`: `2`
- 精灵表：`1536 × 2288`、RGBA WebP
- 布局：`8 × 11`
- 透明背景残留：`0`
- 结构验证：通过
- 16 方向盲测：通过

部分斜向观察角度仅保留细微水平提示；已通过独立视觉复核。

## 许可

本仓库未声明开源许可。未经授权，不授予复制、修改或再分发权利。
