# 结界的尽头场景来源

这张是宣传 PV 用的概念静帧，**待用户挑选**，不是游戏正式立绘。画面里没有人。

| 项目 | 说明 |
| --- | --- |
| 文件 | `barrier_end_v1.png` |
| 优先级 | P1 |
| 用在 | S23 |
| 规格 | 16:9，1920×1080 PNG。生图接口给出的是 1280×720，再用 Pillow 放大到 1920×1080。 |
| 画面 | 没有天和地的灰紫空间。失物堆成山：旧电器、玩具、雨伞、信封。远处一座模糊的鸟居。零星光点往深处飘。信封和物品上没有字。 |

## 怎么做的

| 项目 | 说明 |
| --- | --- |
| 工具 | Cursor 云端代理的内置生图。 |
| 参考图 | 没有用角色参考图，避免把人画进来。 |
| 后期 | 只做了等比放大，没有改内容。 |

## 许可

- 东方 Project 的权利归上海爱丽丝幻乐团 / ZUN。这张图是《东方守幻录》的个人免费非商业概念稿。
- 原创生成。没有描官方立绘，没有拼贴，没有把官方图或别人的同人图送进模型。
- 图上没有写「官方」，也没有低俗或丑化的内容。
- AI 生成：是。调用时没有返回底层模型的名字，这里不猜。
- 没有使用来源或许可无法确认的素材。
- 用途：宣传 PV 的概念静帧，**待用户挑选**。不放进 `assets/`，不打进游戏，不是正式立绘。

## 生图提示词

```
A wide 16:9 story illustration, flat cel animation, muted gray-purple, soft fog, not photorealistic, not 3D. A void with no sky and no ground, only gray-violet mist. Huge piles of forgotten everyday things form hills: old boxy appliances, simple toys, closed umbrellas, sealed blank envelopes. Envelopes and objects have no writing, no letters, no numbers, no logos, no fake glyphs. Far in the depth, one blurred Japanese torii gate, soft and out of focus. A few small pale light motes drift deeper into the mist, away from the viewer.

No people, no characters, no faces, no human silhouettes, no animals. No text, no watermark, no signature, no border, no UI. Quiet and empty.
```
