# pointCloud_Demo-homepage

pointCloud_Demo 的独立静态项目主页。作者为 Jiaqi Liu，单位为 Harbin Institute of Technology。

## 内容

- 参考 LiteMesh 项目主页顶部布局：灰色背景、衬线大标题、蓝色作者与单位名称、校徽，以及 Paper / Video / Code 图标。
- 三枚资源图标仅展示，不提供论文、视频或代码跳转。
- 正文简要介绍 STL 表面采样、归一化、PCA、多起点 ICP 和双向平均最近点距离。
- 结果图及分数来自 pointCloud_Demo 的程序生成示例，不包含原历史模型库。

## 文件

```text
index.html        网页内容
style.css         布局与样式
icon/             哈尔滨工业大学校徽和三个资源图标
images/results.png  示例点云结果图
.nojekyll         静态 Pages 标记
PUBLISHING.md     手动发布说明
```

这是纯 HTML / CSS 页面，没有 Python 后端或前端构建步骤。双击 index.html 即可预览；也可以在本目录运行 `python -m http.server 8000 --bind 127.0.0.1`，访问 `http://127.0.0.1:8000/`。

## 两个仓库的关系

算法仓库：`https://github.com/ljq13505-sudo/pointCloud_Demo`

主页仓库：`https://github.com/ljq13505-sudo/pointCloud_Demo-homepage`

主页预期网址：`https://ljq13505-sudo.github.io/pointCloud_Demo-homepage/`

以上主页仓库和网址需在你完成发布后才能访问。本次只准备本地文件，不进行提交或推送。

## 资源来源

布局参考：[LiteMesh homepage](https://ochenglino.github.io/LiteMesh-homepage/)。校徽及三个资源图标沿用其 `icon/` 中相应资源，保留用于用户指定的参考外观。正文、作者信息和点云结果已替换为本项目内容，资源原有权利归其各自权利人所有。

示例图展示 2048 点 / 模型、6 个起点、最多 35 轮 ICP 的计算结果；图中的缩略点云用于展示已知对应关系，不作为真实检索准确率的证据。
