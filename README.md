
## 流程
> 1~4步骤一步到位方法：fillRect/strokeRect/drawImage
0. translate/rotate/scale - 定义坐标相关信息
1. beginPath - 创建路径起始点，定义一个新的图形环境
2. rect/arc/lineTo/bezierCurveTo/... - 使用路径绘制命令画出路径
3. closePath - 闭合路径。使用fill可忽略
4. fill/stroke/drawImage? - 开始绘图

## 思考
- 主canvas负责整合渲染所有子canvas
- 子canvas一般按功能划分。动画部分的图画单独分成一个canvas，静态部分类似

## 疑问
- 什么时候需要beginPath/closePath
- 哪些api是跟路径(path)相关的
- fill/stroke相关的api有哪些？
  - fillText
  - drawImage ?
- translate/rotate对接下来画图生效，对画布已存在的内容无作用
- canvas的坐标系