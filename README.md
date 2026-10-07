# Project Pulsar：plum 开源头壳模型修复版

本项目是 [@vuicoo](https://github.com/vuicoo) 的开源 Kigurumi 头壳模型 [plumKigurumi-](https://github.com/vuicoo/plumKigurumi-) 的修复版，修复了几何节点和布尔系统中的问题。修复后，前后壳的结构与原作者演示视频一致，并且可以直接用于 3D 打印。

具体修改内容见 [Fix_History.md](Fix_History.md)。

## 文件

- `ProjectPulsar_Base.blend`：修复后的工程文件

## 使用说明

- 需要 **Blender 5.1 或更高版本**。
- 开启布尔后，前后壳重算约 2～3 秒。
- 前壳「前后基准值」可调范围是 0～0.85，再往后风扇口会离前后分界线太近。
- 后壳「圆角位置」：0 = 分界线底部没有圆弧缺口，数值越大缺口越大；原作者演示视频的效果约为 0.037。
- 如果视口里出现斜向长条或黑块，请关闭视口着色设置中的 Shadow。这是视口渲染的伪影，不是模型问题。

## 导出 STL

- 前壳（`前壳配置`）和后壳（`后壳配置`）**分别导出**：选中一个，导出时勾选「仅选中项」。两个壳放进同一个 STL，切片软件会把接缝判成非流形边。
- 工程单位是米，导出时把「缩放」设为 **1000**，STL 才是毫米。

## 字体

刻字使用的 HarmonyOS Sans SC Bold 已打包进 `.blend`，版权归华为所有，按其字体许可协议使用。

## 许可

原始模型作者：[@vuicoo](https://github.com/vuicoo)（[视频简介](https://twitter.com/i/status/1741975998399439042)）。本修复版与原项目相同，按 **GNU GPL v3** 发布，详见 [LICENSE](LICENSE)。
