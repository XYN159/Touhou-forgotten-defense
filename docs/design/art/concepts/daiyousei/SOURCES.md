# 大妖精 概念图来源

这张是宣传 PV 用的概念静帧，**待用户挑选**，不是游戏正式立绘。

| 项目 | 说明 |
| --- | --- |
| 文件 | `daiyousei_v1.png` |
| 优先级 | P1 |
| 用在 | S10、S30 |
| 外观方向 | 绿色侧马尾，黄色发带，蓝色连衣裙，透明的小妖精翅膀。有点胆小的温柔笑容。第一张翅膀太像琪露诺的冰晶，没有采用；留下的是第二张，翅膀改成较小的圆润虫翅。 |

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
Match ONLY the drawing style of the reference image. Do not copy the reference person. Style: one original cute chibi, hand-drawn flat cel, about 2.5 heads tall, medium deep purple-black outlines, flat color, exactly one hard-edged cooler shadow from the upper left, one small hair highlight, no gradients, not 3D. Wholesome fully clothed child, modest, children's book. Large green eyes, shy gentle closed-mouth smile, soft blush. Full body, both feet visible, slight three-quarter view, centered, oval ground shadow, flat pale cream background.

Character: green hair in a side ponytail with a yellow ribbon. Modest blue knee-length dress, white collar, white socks, blue shoes. Behind her, SMALL fairy wings: only two pairs of soft rounded dragonfly membranes, pale mint and transparent, with a few gentle curves, NOT ice, NOT crystals, NOT diamonds, NOT geometric shards, NOT blue. Wings are smaller than her skirt. Timid kind pose, hands relaxed and simple, no extra fingers.

No shrine maiden outfit, no red bow, no gohei, no ice crystal. No text, no letters, no numbers, no watermark, no thumbnail. Exactly one child.
```
