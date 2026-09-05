# 明信片意境海报 Skill

[English version](README.en.md)

这是一个把照片转成 3:4 旅行明信片意境海报的可复用图像生成 Skill。

## 核心结构

- 上半部：忠实保留原始照片。
- 下半部：把地点或人物动作提炼成留白充足的水彩记忆。
- 中间：清楚的上下 50/50 分区，不使用厚重边框。
- 信息层：默认使用克制的主标题和短分隔线；地点、年份按用户要求添加，年份只在用户提供或确认时使用。

## 两个系列

- 场景系列：城市、河流、自然、建筑、道路和日落。水彩只保留 1–3 个地点识别线索，主体中等偏小，留白要大于细节。
- 人物系列｜Watercolor Motion：运动、旅行、家庭和人物动作。严格保留动作骨架、身体重心、四肢方向、姿态、运动轨迹和人物关系。

人物水彩默认缩小到正常复现尺度的 60%–75%；如果画面仍拥挤，可以继续缩小到 60% 以下。人物只是记忆锚点，留白和整体意境才是主角。

## 怎么用

1. 将这个目录作为 `postcard-memory-poster` Skill 安装到你的 Skill 目录。
2. 在支持 Skill 的 Codex 环境中调用 `$postcard-memory-poster`。
3. 上传一张照片；指定场景系列或人物动态系列，也可以让 Skill 自动判断。
4. 如果有要求，再指定标题、地点、年份、无文字或其他信息层内容。

示例：

```text
$postcard-memory-poster
把这张照片做成 Watercolor Motion 人物系列。
人物缩小一些，保留大面积留白；只保留一行英文标题和一条细分隔线。
```

## 公开仓库说明

这个仓库只发布 Skill 规则、视觉参考和使用文档，不发布用户提供的照片，也不发布生成出来的照片海报。图片应作为本地输入或本地输出使用，不要提交到 GitHub。

完整规则见 [`SKILL.md`](SKILL.md)、[`references/art-direction.md`](references/art-direction.md) 和 [`references/art-direction-en.md`](references/art-direction-en.md)。
