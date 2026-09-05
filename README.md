# 明信片意境海报 Skill / Postcard Memory Poster

这是一个把照片转成 3:4 旅行明信片意境海报的可复用图像生成 Skill。
It turns photographs into 3:4 editorial postcard-memory posters.

## 两个系列

- 场景系列：城市、河流、自然、建筑、道路和日落。
- 人物系列：运动、旅行、家庭和人物动作；使用 `Watercolor Motion`，重点是动作骨架、人物关系和真实运动方向，而不是静态水彩肖像。人物水彩默认缩小到正常复现尺度的 60%–75%；留白不足时可继续缩小，意境优先。
- Scene series: cities, rivers, nature, architecture, roads, and sunsets.
- People series: movement, travel, family, and human gestures. Use `Watercolor Motion` to preserve the action skeleton, relationships, and physical direction of motion.
- In the people series, start at 60%–75% of the normal readable figure scale and reduce further when needed. Negative space and atmosphere take priority.

## 固定结构

- 上半部：忠实原始照片。
- 下半部：留白充足的水彩记忆。
- 信息层：默认是克制的主标题和短分隔线；地点、年份按系列和用户要求添加，年份只在有来源时使用。
- Top half: faithful original photograph.
- Bottom half: an airy watercolor memory with generous paper space.
- Text layer: a restrained title and short divider by default; add location and year only when requested or confirmed.

## 怎么用｜How to use

1. 将这个目录作为 `postcard-memory-poster` Skill 安装到你的 Skill 目录。
2. 在支持 Skill 的 Codex 环境中调用 `$postcard-memory-poster`。
3. 上传一张照片；指定场景系列或人物动态系列（也可以让 Skill 自动判断）。
4. 可选指定说明语言和海报文字语言。

Install this folder as `postcard-memory-poster`, invoke `$postcard-memory-poster`, and attach one photograph. You may select the series, response language, and poster-text language.

### 中文请求示例｜Chinese example

```text
$postcard-memory-poster
用中文说明，做成场景系列；海报标题、地点和年份使用英文。
```

### English request example

```text
$postcard-memory-poster
Explain in English. Create a Watercolor Motion poster from this photo and keep the poster title in English.
```

### 双语请求示例｜Bilingual example

```text
$postcard-memory-poster
中英双语说明，人物系列，海报文字只保留一行英文标题和一条分隔线。
```

语言切换的完整规则见 [`references/language-switching.md`](references/language-switching.md)。

完整视觉规则见 [`SKILL.md`](SKILL.md)、[`references/art-direction.md`](references/art-direction.md) 和英文版 [`references/art-direction-en.md`](references/art-direction-en.md)。

## 样例｜Examples

这些 PNG 是已验证过的风格样例，不是生成时必须逐像素复制的模板：

- 场景系列 / Scene series: [`melbourne-bayside-watercolor-memory-v1.png`](melbourne-bayside-watercolor-memory-v1.png)、[`melbourne-yarra-river-editorial-poster.png`](melbourne-yarra-river-editorial-poster.png)
- 人物系列 / People series: [`watercolor-memory-person-blue-v2.png`](watercolor-memory-person-blue-v2.png)、[`watercolor-memory-person-blue-v1.png`](watercolor-memory-person-blue-v1.png)

These examples show the intended balance: a faithful photograph above, a smaller watercolor memory below, and negative space that carries the atmosphere.

当前目录中的 PNG 是这一风格的历史成品记录，不作为生成时必须复制的具体画面。
