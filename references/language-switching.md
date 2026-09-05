# Language Switching / 语言切换

这个 Skill 支持双语使用，但“回复语言”和“海报文字语言”是两个不同的设置。

## 1. 回复语言｜Response language

| 用户说法 | 模式 | 行为 |
|---|---|---|
| `中文`、`用中文说明` | `zh` | 用中文说明判断、方案和结果 |
| `English`、`explain in English` | `en` | Explain the decision and result in English |
| `双语`、`bilingual`、`中英双语` | `bilingual` | 先中文，后英文；两部分内容保持对应 |
| 未指定 | 自动判断 | Follow the dominant language of the latest user message |

切换只需在请求中加一句话：

```text
用中文说明，把这张照片做成场景系列。
Switch to English and create a Watercolor Motion poster from this photo.
中英双语说明，海报标题保留英文。
```

## 2. 海报文字语言｜Poster text language

可以单独指定海报文字：

- `海报文字用中文 / poster text in Chinese`：标题、地点和年份使用中文。
- `poster text in English`：使用克制的英文标题和英文地点信息。
- `海报文字双语 / bilingual poster text`：只有在用户明确要求时才双语排版，避免破坏留白。
- `无文字 / no text`：移除标题、地点、年份和分隔线。

如果没有指定海报文字语言，默认保留既有样例的英文编辑式标题。用户提供的专有名词、标题、地点或年份必须原样保留，不自动翻译或改写。

## 3. 推荐请求格式｜Recommended request format

```text
$postcard-memory-poster
说明语言：中文 / English / 双语
系列：场景 / 人物动态
海报文字：英文 / 中文 / 双语 / 无文字
标题：可选
地点：可选
年份：可选，仅使用用户提供或确认的信息
请使用这张照片生成一张 3:4 明信片意境海报。
```

English version:

```text
$postcard-memory-poster
Response language: Chinese / English / bilingual
Series: scene / Watercolor Motion
Poster text: English / Chinese / bilingual / none
Title: optional
Location: optional
Year: optional, only if provided or confirmed
Create one 3:4 postcard-memory poster from this photo.
```

## 4. 默认值｜Defaults

- 回复语言：跟随用户最近一条消息。
- 系列：根据照片判断；运动、人物互动和家庭瞬间优先进入 `Watercolor Motion`。
- 海报文字：英文短标题＋短分隔线。
- 地点和年份：只有用户提供或明确确认时才添加。
- 多张照片：每张分别生成，不合成 collage。
