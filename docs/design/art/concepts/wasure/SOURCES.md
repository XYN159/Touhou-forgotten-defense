# 「忘」剪影场景来源

这张是宣传 PV 用的概念静帧，**待用户挑选**，不是游戏正式立绘。落野忘的外形还没定稿，所以这里只留剪影，不露脸。

| 项目 | 说明 |
| --- | --- |
| 文件 | `wasure_v1.png` |
| 优先级 | P0 |
| 用在 | S31 |
| 规格 | 16:9，1920×1080 PNG。生图接口给出的是 1280×720，再用 Pillow 放大到 1920×1080。 |
| 画面 | 灰色缝隙深处。旧伞、单只手套、八音盒、钥匙扣和空白编号纸牌堆成一座鸟居。鸟居下是一个小个子少女的剪影：长外套，背上一个挂着失物的小木架，身上挂着许多空白纸牌。只看得见轮廓。眼睛位置有两点淡淡的光。低饱和，有雾。图上没有字。 |

## 怎么做的

人物如果直接生成，模型会把脸画出来。这张因此分成两步，保证不露脸：

1. 先生成没有人的 16:9 背景：失物堆成鸟居，门口空着，纸牌是空白矩形。
2. 再在纯绿背景上生成一个剪影外形，然后用 Pillow 把所有非绿色像素压成同一种深紫灰，只在眼睛位置补两个很小、很淡的圆点。头发和外套只留外轮廓，没有五官、没有衣服颜色。
3. 把剪影贴到鸟居门口，双脚留在画面里。

没有使用灵梦 v2 作参考，避免把巫女画进这张悬念镜头。没有使用官方图或别人的同人图。

## 许可

- 东方 Project 的权利归上海爱丽丝幻乐团 / ZUN。这张图是《东方守幻录》的个人免费非商业概念稿。
- 原创生成。没有描官方立绘，没有拼贴，没有把官方图或别人的同人图送进模型。
- 图上没有写「官方」，也没有低俗或丑化的内容。
- AI 生成：是。调用时没有返回底层模型的名字，这里不猜。
- 没有使用来源或许可无法确认的素材。
- 用途：宣传 PV 的概念静帧，**待用户挑选**。不放进 `assets/`，不打进游戏，不是正式立绘。

## 生图提示词

### 背景（没有人）

```
Wide 16:9 flat cel illustration, muted gray-lavender fog, low saturation, not photorealistic, not 3D. Everyday lost objects are piled so they form a Japanese torii gate with a clearly EMPTY doorway in the lower center. Objects: one old umbrella, one single glove, a small music box, a keychain, and many blank paper tags. Tags are empty rectangles with no writing, no scribbles, no letters, no numbers, no glyphs. The ground in front of the torii is empty foggy space, reserved for a figure that is NOT in this picture. No people, no silhouettes, no faces, no human shapes, no animals. No text, no watermark, no border.
```

### 绿底剪影（之后被压成纯色）

```
A single graphic icon on a flat pure chroma-key green background (#00FF00). Subject is ONE solid flat black filled silhouette of a small chibi girl, about 2.5 heads tall, full body, both feet visible, facing forward. The silhouette is a pure black fill with a clean outer contour and absolutely no interior lines, no gray, no shading, no clothes colors, no hair strands, no bangs, no nose, no mouth, no eyes with pupils. The only non-black marks are two tiny round pale-gray dots where the eyes would be. Shape cues in the outer contour only: a large round head, a long coat that flares a little, short legs, simple shoes, and a rectangular wooden rack rising behind her shoulders. Hanging off the rack and the coat are simple bumps in the same black silhouette: an umbrella shape, a glove shape, a small box, a keyring, and several rectangular tag shapes. Centered, generous green margin around the whole figure. No text, no letters, no numbers, no ground, no shadow, no scenery, exactly one silhouette.
```
