# 风栖 · Pocket Park

> 现在，你想去哪里？

一个离线、单文件的放松小作品。灵感来自"公园20分钟效应"：在自然中待上20分钟，压力就会明显下降。风栖把一座口袋公园装进浏览器，不用安装，不用登录。

**在线 Demo：** https://YOUR_GITHUB_NAME.github.io/fengqi/
**快速体验：** 在链接后加 `?t=30`，30 秒就能看到高潮和离别诗。

## 四扇门

| 场景 | 互动 | 20分钟时的自然现象 | 离别诗的载体 |
| --- | --- | --- | --- |
| 花间 | 点一下，花就开了 | 花瓣飘来，光变成金粉色 | 花瓣 |
| 湖畔 | 涟漪跟着指针走 | 一层薄雾 | 水面倒影 |
| 林下 | 在叶子上写一个字，被风吹走 | 起风，落叶变密 | 落叶 |
| 星野 | 连星座，可以拖动星空 | 一颗流星 | 星光 |

## 20分钟节奏

- 0–5 分钟：安静，前 5 秒不需要任何操作
- 5–15 分钟：光线慢慢移动，出现飞鸟和萤火虫
- 15–20 分钟：进入黄金时刻，色调更暖更柔
- 20 分钟：出现一个自然现象，不弹文字
- 离开时：雾气升起，一句诗落在专属载体上，然后回到封面

## 运行

下载 `index.html`，双击用浏览器打开即可。建议使用最新版 Chrome、Edge 或 Safari（需要 WebGL2）。

## 技术说明

- 单个 HTML 文件，没有任何第三方依赖
- WebGL2 着色器负责水面、光影和画面形变
- Canvas 2D 负责花瓣、落叶、星座连线和离别诗
- WebAudio 实时合成环境音
- 不发送网络请求，不使用 Cookie 或本地存储，不做埋点
- 林下写的字只存在于屏幕上，叶子飘走后就消失

## 素材

场景与物件均为 AI 生成的吉卜力/日系动画风插画（gpt-image-2），只使用文字提示词，没有使用任何个人照片。

## 隐私

不收集、不上传、不保存任何数据。

## English

Pocket Park (风栖) is an offline, single-file relaxation demo inspired by the "20-minute park effect". Pick one of four doors (spring flowers, a lake, an autumn forest, a starry field), play with small gentle interactions, and let a 20-minute rhythm unfold. When you leave, a short poem appears and mist carries you back to the cover. No network requests, no storage, no tracking. Add `?t=30` to the URL to preview the full journey in 30 seconds.

## License

MIT
