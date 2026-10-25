# 风栖 · Pocket Park

> 现在，你想去哪里？

一个离线、单文件的放松小作品。灵感来自"公园20分钟效应"：在自然中待上20分钟，压力就会明显下降。风栖把一座口袋公园装进浏览器，不用安装，不用登录。

**在线 Demo：** https://liliyala.github.io/fengqi/
**快速体验：** 在链接后加 `?t=30`，30 秒就能看到偶遇、高潮和离别诗。

## 设计理念

- **轻**：没有分数，没有任务，没有通知。前 5 秒什么都不需要做。
- **慢**：节奏对应 20 分钟，光线、飞鸟、天气一点一点展开，不催促。
- **和你有关**：治愈常常是个人的。你可以带一张自己的照片进来，让它也成为一座公园。
- **不用动手也行**：放松时不必一直点鼠标。可以挥手，也可以什么都不做，看它自己玩。
- **安静地离开**：离开时没有总结页，只有一句诗落在这座公园专属的载体上。
- **不打扰**：不联网，不上传，不收集。只在本机留下你自己的偏好和一本可以随时清空的手记。

## 五扇门

| 场景 | 互动 | 20分钟时的自然现象 | 离别诗的载体 |
| --- | --- | --- | --- |
| 花间 | 点一下，花就开了 | 花瓣飘来，光变成金粉色 | 花瓣 |
| 湖畔 | 涟漪跟着指针走 | 一层薄雾 | 水面倒影 |
| 林下 | 在叶子上写一个字，被风吹走 | 起风，落叶变密 | 落叶 |
| 星野 | 用手指（或鼠标、挥手）在星星之间划线，连成星座，每颗星有一个音符；内置十二星座，点「找星座」选一个，星空会带你过去，亮着的虚线就是它的样子；可以拖动星空（手机上触点已放大） | 一颗流星 | 星光 |
| 定格 | 选一张你自己的照片，画面缓缓推近，光斑漂浮，轻轻划过，光会跟着你 | 色调随旅程变暖，薄雾升起 | 照片之上 |

"定格"是可选的：独属于你的回忆。不选照片，就不会发生任何事。

## 功能

- **20 分钟节奏**：0–5 分钟安静，5–15 分钟光线移动、飞鸟与萤火虫，15–20 分钟黄金时刻，20 分钟出现自然现象，离开时雾气升起、一句诗落下，然后回到封面。
- **偶遇**：每次进入场景，约四分之三的概率在中段遇到一件小事。花间和林下有蝴蝶飞过，湖畔下一场小雨，星野有一点流光漂过。剩下的时候什么也不发生。
- **此刻的光**：按你本地的时间给画面加早晚色调。清晨偏冷，正午通透，傍晚偏暖，夜里偏深。
- **离别诗**：每个场景有多首诗，有古诗（标明出处），也有几句原创的轻语。每次离开随机一首，不会连续重复。
- **手势**：不用鼠标也能玩。
  - 挥手：打开摄像头，在画面前挥手，就像在空中拨动水面、花和星。摄像头画面只在本地用来判断手的移动，不显示，不保存，不上传。需要浏览器授权，线上版本通过 https 可以使用。
  - 漫游：不需要摄像头，什么都不用做，它会自己慢慢玩。
- **环境音与背景音乐**：环境音由 WebAudio 实时合成。背景音乐可选"安静"、"轻快"，也可以选"我的音乐"，加载你电脑上的一个音频文件（只在内存里播放，不上传，不保存）。湖畔的水声会跟着手势和指针响起。
- **时长可选**：封面可以选 5 / 10 / 20 分钟，节奏按比例缩放。第一次来可以先走 5 分钟。
- **设置**：封面右上角的齿轮里可以调整九项：声音、手势、呼吸、位置、提示音、睡眠、倾斜、字号（标准 / 大 / 特大）、动效（"轻柔"会少一些闪动，默认跟随系统的减少动态设置）。每一项下面都有一行小字说明。
- **睡眠**：设置里选 10 / 20 / 30 分钟，声音和画面慢慢变暗，到点后只剩一句“晚安”，轻触屏幕回到封面。适合睡前在星野里待一会儿。
- **呼吸**：默认关闭。打开后，画面上有一圈很淡的光，扩大 4 秒时吸气，收拢 6 秒时呼气，圈里会淡淡写着“吸气”“呼气”。圈的位置可选偏上 / 居中 / 偏下。“提示音”打开后，吸气时有一阵轻风渐起、呼气时慢慢散去，各带一声低低的钟音，随圈的起伏同步（全部由页面现场合成，不联网，也不依赖设备的语音）。
- **倾斜**：默认关闭。在手机上打开后，倾斜手机，画面会轻轻移动，每跨过一个区间响起一个音符。iPhone 会请求“动作与方向”权限。方向数据只用来移动画面，不记录，不上传。
- **分享诗卡**：离别诗之后可以选择"留下这一刻"，在本地生成一张 1080×1440 的诗卡图片并保存。在定格里，诗卡的背景就是你自己的照片。不联网，不上传。
- **手记**：在本机累计来过几次、一共待了多久、遇见过哪些离别诗、连过哪些星座（十二星座都能集）。多次访问后能翻开看到。可以随时清空。
- **全屏**：支持一键全屏，更沉浸。iPhone 上可用"添加到主屏幕"获得类似效果。
- **自适应与友好**：加载时有提示；设备吃力时自动降低渲染精度；切到后台时自动静音。

## 运行

下载 `index.html`，双击用浏览器打开即可。建议使用最新版 Chrome、Edge 或 Safari（需要 WebGL2）。

URL 参数（用于演示）：

- `?t=30`：把 20 分钟压缩成 30 秒
- `?h=21`：假装现在是 21 点，用来预览早晚色调

## 技术说明

- 单个 HTML 文件，没有任何第三方依赖
- WebGL2 着色器负责水面、光影和画面形变
- Canvas 2D 负责花瓣、落叶、蝴蝶、雨、星座连线和离别诗
- WebAudio 实时合成环境音
- 手势：摄像头画面缩到 64×48 后做帧差，得到手的移动方向，再转成和鼠标一样的指针事件。漫游用同样的事件路径，由程序生成轨迹
- 不发送网络请求，不使用 Cookie，不做埋点。只用 localStorage 保存两项本机数据：偏好（`fengqi.set.v1`，仅字号、时长、减少动态、呼吸引导及其位置和提示音六项）和手记（`fengqi.memo.v1`）
- 诗卡由 Canvas 2D 在本地绘制成 PNG，不经过网络
- 林下写的字只存在于屏幕上，叶子飘走后就消失

## 素材

场景与物件均为 AI 生成的吉卜力/日系动画风插画（gpt-image-2），只使用文字提示词，没有使用任何个人照片。

## 隐私

不上传任何数据，不使用任何第三方服务。

- 你选的照片和"我的音乐"文件只在当前页面的内存里，直接读成画面或声音，不经过网络，不写入存储。离开"定格"回到封面，就从内存里清掉；刷新页面也一样。
- 打开摄像头时，画面只在本地做运动判断，不显示、不录制、不上传。随时可以在"手势"里关掉。
- 本机只保存两样东西：偏好设置（字号、时长、减少动态、呼吸引导及其位置和提示音）和手记（访问次数、累计时长、见过的诗、连过的星座名）。里面没有照片、音乐、摄像头画面。手记可以在页面里清空，也可以清除浏览器站点数据。

## English

Pocket Park (风栖) is an offline, single-file relaxation demo inspired by the "20-minute park effect". Pick one of five doors (spring flowers, a lake, an autumn forest, a starry field, and a place of your own, "定格", made from a photo you choose), play with small gentle interactions, and let a 20-minute rhythm unfold. Small encounters (a butterfly, a light rain) drift by now and then, and the light follows your local time of day. You can play without a mouse: wave at your camera, or let it wander on its own. Pick 5, 10 or 20 minutes (or a sleep mode that slowly dims the sound and screen), add an optional breathing ring, tilt your phone for gentle parallax and soft notes, add background music (including a local file of your own), and keep a small journal of your visits. When you leave, a short poem appears, and you can save it as a poem card generated locally on your device; then mist carries you back to the cover. No network requests, no uploads, no tracking. Only your display preferences and the clearable journal are kept in localStorage. Your photo, music file and camera frames stay in memory and never leave your device. Add `?t=30` to the URL to preview the full journey in 30 seconds.

## License

MIT
