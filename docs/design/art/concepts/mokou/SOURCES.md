# 藤原妹红 概念图来源

这张是宣传 PV 用的概念静帧，**待用户挑选**，不是游戏正式立绘。

| 项目 | 说明 |
| --- | --- |
| 文件 | `mokou_v1.png` |
| 优先级 | P0 |
| 用在 | S18、S30 |
| 外观方向 | 银白长发，红白大蝴蝶结发饰，白衬衫配红色背带裤。手边一团小火焰。随意，嘴硬心软。 |

## 怎么做的

| 项目 | 说明 |
| --- | --- |
| 工具 | Cursor 云端代理的内置生图。 |
| 参考图 | 已选的灵梦 v2。先去掉右下角 128 预览框，再垫在浅奶油色底上。提示词写明只对齐画风，不要照抄巫女服、红白大蝴蝶结和御币。 |
| 后期 | 用 Python（Pillow）从画面四边把浅奶油色背景抠成透明。白衣服留着，没有抠穿。没有再贴 128 预览框。 |
| 规格 | 1024×1024 PNG，透明底。约 2.5 头身，中等深紫黑描边，平涂加一层硬阴影，正面略侧，全身双脚可见。 |

## 许可

- 东方 Project 的权利归上海爱丽丝幻乐团 / ZUN。这张图是《东方守幻录》的个人免费非商业概念稿。
- 原创生成。没有描官方立绘，没有拼贴，没有把官方图或别人的同人图送进模型。
- 图上没有写「官方」，也没有低俗或丑化的内容。
- AI 生成：是。调用时没有返回底层模型的名字，这里不猜。
- 没有使用来源或许可无法确认的素材。
- 用途：宣传 PV 的概念静帧，**待用户挑选**。不放进 `assets/`，不打进游戏，不是正式立绘。

## 生图提示词

提示词用英文，因为生图接口对英文更稳。负面要求写在同一段里：不要文字、不要水印、不要多余的人。

```
Match ONLY the drawing style of the reference image. Do not copy the reference person. Style: one original cute chibi character, hand-drawn flat cel, about 2.5 heads tall, medium-weight even deep purple-black ink outlines, flat colors with exactly one hard-edged cooler shadow from upper-left light, one small hair highlight, no gradients, not 3D, not painterly. Symmetrical pretty face, large refined amber-red eyes, a small reluctant closed-mouth smile, soft blush. Full body, both feet fully visible, slight three-quarter view, centered with margin, simple oval ground shadow. Flat pale cream background, no scenery.

Draw a different character: a casual girl with long straight silver-white hair and a large red-and-white bow hair ornament at the side of her head. White short-sleeve shirt, red suspenders, red short overalls, dark red trousers, simple brown shoes. A small tidy orange flame floats beside one open hand, not covering her body, no smoke cloud. Relaxed stance, tough-but-kind. Fully clothed and modest. Correct simple hands, no extra fingers. No burns, no gore.

Do not copy the shrine maiden, red hakama, huge back bow, or gohei. No text, no letters, no numbers, no watermark, no signature, no border, no thumbnail. Exactly one person.
```
