# 耄耋 · Maodie Pet 😾

一只会敲键盘、催回复、报错炸毛、验收哈气的真实照片风格宠物。基于「耄耋」梗制作，适用于支持 Pets 的 ChatGPT Work 环境。

**[领养这只耄耋](https://chatgpt.com/s/sharepet_6ad9c35332288191add36239fb5688ce)** · **[下载精灵图](assets/maodie-spritesheet.png)** · **[下载发布包](https://github.com/Jerryhhhhhh/maodie-pet/releases/latest)**

![耄耋的四个代表动作](previews/main.gif)

## 怎么使用

在已启用 Pets 的对话中发送：

```text
请领养并选用这个宠物：
https://chatgpt.com/s/sharepet_6ad9c35332288191add36239fb5688ce
```

领养会在你的宠物库中创建自己的副本。也可以下载 [PNG 精灵图](assets/maodie-spritesheet.png)，交给支持该格式的宠物工具使用。

## 它会做什么

| 状态 | 动作 |
| --- | --- |
| 待机 | 呼吸、眨眼、小幅抬头 |
| 左右移动 | 自然猫步，分别面向左右 |
| 招呼 | 抬起一只前爪 |
| 跳跃 | 蓄力、腾空、落地 |
| 报错 | 弓背炸毛，进入「棘背龙形态」 |
| 等回复 | 同一只前爪弯回胸前，再向前伸出，连续催两次 |
| 工作 | 两只猫爪交替敲键盘 |
| 成果检查 | 连续四帧张嘴哈气，标准节奏约 **0.73 秒** |
| 看向光标 | 16 个顺时针注视方向 |

哈气是 `review` 状态中的视觉动作。当前 Pets 工具不提供自定义音效或可配置的“每次会话结束”触发器。

## 预览与备用动作

- [全部九组动画](previews/all-states.gif) / [MP4](previews/all-states.mp4)
- [16 方向环视](previews/look-loop.gif)
- [全部帧总览](previews/contact-sheet.png)
- [挠头、托腮备用动画](variants/thinking.gif) / [透明六格图](variants/thinking-strip.png)

备用动画包含 4 帧挠头和 2 帧托腮，最后两帧保持同一只爪。**主版工作动作是打字**，备用动作不会随机穿插；使用备用版需要替换工作动画行并重新验证完整精灵图。

## 文件规格

| 项目 | 值 |
| --- | --- |
| 格式 | 透明 PNG，v2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单格尺寸 | 192 × 208 |
| 有效帧 | 73 |
| 每行帧数 | 6, 8, 8, 4, 5, 8, 6, 6, 6, 8, 8 |

SHA-256：

```text
a6b924845704ff812247841a43b3aff2655297af93dad1198848c9355a9d3932
```

帧顺序、播放时长与方向定义见 [pet.json](pet.json)，验证摘要见 [validation.json](validation.json)。该图集通过了本地结构、动作、方向检查和 Pets 上传前验证。

## 制作与来源

以真实耄耋照片为视觉基准，用内置 ImageGen 制作和编辑动作，再完成背景清理、拼接及逐帧检查。打字版的脸型和浅沙金毛色已与基准对齐。

感谢 [yr-96/meme-library](https://github.com/yr-96/meme-library/tree/4aac9fcefcb753e17cc046fb8da1da7a6581bd6b/examples/sample_lib/maodie_cats) 的表情素材归档。其他参考出处见 [CREDITS.md](CREDITS.md)。

## English

A photo-based Maodie meme cat for ChatGPT Work Pets: keyboard typing, impatient paw taps, a bristling error reaction, and a long hiss during review. Includes nine animation states and sixteen look directions.

Use the **[public adoption link](https://chatgpt.com/s/sharepet_6ad9c35332288191add36239fb5688ce)** in a Pets-enabled conversation, or download the validated sprite sheet. The thinking animation is an optional alternative to typing. Custom audio and configurable session-end triggers are not provided by the current Pets tools.
