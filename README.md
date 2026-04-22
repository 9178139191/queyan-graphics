# 確演图形引擎 · QueYan Graphics Engine

版本 1.0.0    |    许可证 AGPL v3    |    WebGL 2.0    |    PBR管线

確演图形引擎为確演OS之二维与三维图形渲染核心，基于WebGL 2.0实现可编程渲染管线。场景图采用节点-组件架构，支持局部坐标系与变换继承。纹理管理器实现延迟加载与Mipmap生成。动画引擎支持关键帧插值与30余种内置缓动函数。

技术特征

- 渲染管线支持顶点着色器与片元着色器，实现PBR材质与IBL光照
- 场景图实现视锥剔除与遮挡查询，减少绘制调用
- 粒子系统采用GPU模拟，支持10000粒子并发
- 字体渲染基于SDF距离场，支持描边、阴影、渐变

性能指标

绘制批次：约200批次每帧
三角面数：约50000面每帧
纹理内存：约64MB
帧率：稳定60fps

编译与部署

git clone https://github.com/9178139191/queyan-graphics
cd queyan-graphics
npm install
npm run build

---

English Abstract

QueYan Graphics Engine is a WebGL 2.0 based programmable rendering pipeline featuring PBR materials with IBL lighting, a scene graph with frustum culling, GPU-simulated particle systems supporting 10000 concurrent particles, and SDF-based font rendering with stroke and shadow effects.

GNU Affero General Public License v3.0

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program. If not, see https://www.gnu.org/licenses/.

Copyright © 2026 確演OS. 保留所有权利。
