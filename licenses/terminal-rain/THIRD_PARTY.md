# 开源来源与许可

## Rezmason/matrix

- 仓库：https://github.com/Rezmason/matrix
- 提交：`5ba90490453ceceb6812d6b1bc658a99a92411d0`
- 许可：MIT，见 `vendor/Rezmason-MIT.txt`
- 复用：`assets/matrixcode_msdf.png` 的内嵌数据；`shaders/glsl/rainPass.frag.glsl` 中 MSDF 中值解码与网格采样的改写；`rainPass.raindrop.frag.glsl` 中随机函数的改写；REGL 全屏三角形的绘制思路。
- 改造：重写时钟、每列模拟、色彩和深度合成；增加鼠标减速、点击流、暂停与清理、离线面板和 React 包装。
- V2 默认使用本机等宽字体生成细字纹理，原 MSDF 字形保留为可选项；新增重复雨段、平滑头部过渡、双尺度高斯柔光和隔离的网页组件封装。
- 未包含或提取 React Bits Pro 的专有源码；名称仅描述所参考的特效类型。

## regl-project/regl

- 仓库：https://github.com/regl-project/regl
- 许可：MIT，见 `vendor/REGL-LICENSE.txt`
- `vendor/regl.min.js` 来自上述 Matrix 仓库对应提交中的捆绑版本；供独立 HTML 使用。
- React 包装通过 npm `regl` 导入。具体测试版本记录于 `verification/react-fixture/package-lock.json`。

许可文件须随再分发版本保留。
