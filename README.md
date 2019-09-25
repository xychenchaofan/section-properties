![alt text](logo.png "sectionproperties")

[![Build Status](https://travis-ci.com/robbievanleeuwen/section-properties.svg?branch=master)](https://travis-ci.com/robbievanleeuwen/section-properties) [![Documentation Status](https://readthedocs.org/projects/sectionproperties/badge/?version=latest)](https://sectionproperties.readthedocs.io/en/latest/?badge=latest)

一个用有限元法分析任意截面截面特性的python库（程序主体由Robbie van Leeuwen完成，汉化工作由陈超凡完成）。 *sectionproperties* 可用于确定结构设计中使用的截面特性也可以可视化由作用力和弯矩组合产生的横截面应力。

[Subscribe](http://eepurl.com/dMMUeg) to the mailing list!

## Installation:

了解更多安装信息, 参照此处 [documentation](https://sectionproperties.readthedocs.io/).

### UNIX (MacOS/Linux):

```
$ pip install sectionproperties
```

### Windows

Install *meshpy* by downloading the appropriate [installation wheel](https://www.lfd.uci.edu/~gohlke/pythonlibs/#meshpy).

Navigate to the location of the downloaded wheel and install using pip:

```
$ cd Downloads
$ pip install MeshPy‑2018.2.1‑cp36‑cp36m‑win_amd64.whl
```

Once *meshpy* has been installed, *sectionproperties* can be installed:

```
$ pip install sectionproperties
```

## Documentation:

*sectionproperties* 有一个完整的python api文档，您可以在找到 [https://sectionproperties.readthedocs.io/](https://sectionproperties.readthedocs.io/). 要了解更多关于程序背后的理论、实现和更多示例，请访问作者的博客  [https://robbievanleeuwen.github.io/](https://robbievanleeuwen.github.io/).

## Current Capabilities:

### Pre-Processor:
- [x] Python API
- [x] Custom section geometry input 输入自定义截面几何图形 
- [x] Common section geometry generators 常见截面几何形状生成
- [x] Multiple geometry merging 多个几何图形合并
- [x] Geometry cleaning
- [ ] JSON input file
- [ ] .dxf import
- [x] Quadratic triangular mesh generation 二次三角网格生成 
- [x] Composite material properties 组合材料特性

### Cross-Section Analysis:
- [x] Global axis geometric section properties（整体坐标系中截面特性）:
  - [x] Area 面积
  - [x] First moments of area 静距
  - [x] Second moments of area 惯性矩
  - [x] Elastic centroid 弹性中心
- [x] Centroidal axis geometric section properties（形心轴中截面特性）:
  - [x] Second moments of area
  - [x] Elastic section moduli
  - [ ] Yield moment 屈服弯矩
  - [x] Radii of gyration
  - [x] Plastic centroid
  - [x] Plastic section moduli
  - [x] Shape factors
- [x] Principal axis geometric section properties（形心主轴中截面特性）:
  - [x] Second moments of area
  - [x] Elastic section moduli
  - [ ] Yield moment 屈服弯矩
  - [x] Radii of gyration
  - [x] Plastic centroid 塑性中心
  - [x] Plastic section moduli
  - [x] Shape factors
- [x] Warping section properties（翘曲特性）:
  - [x] Torsion constant
  - [x] Warping constant
- [x] Shear section properties（剪切特性）:
  - [x] Shear centre (elastic method) 
  - [x] Shear centre (Trefftz's method)
  - [x] Shear areas (global axis) 剪切面积（整体坐标系）
  - [x] Shear areas (principal axis) 剪切面积（形心主轴）
- [x] Cross-section stresses 截面应力

### Solver:
- [x] Direct solver 直接法求解器
- [x] CGS iterative solver CGS迭代求解器 
- [x] Sparse matrices 稀疏矩阵

### Post-Processor:
- [x] Plot geometry 绘制几何图形
- [x] Plot mesh 绘制网格划分
- [x] Plot centroids 绘制中点
- [x] Plot cross-section stresses 绘制截面应力
- [x] Retrieve cross-section stresses 
- [ ] Generate cross-section report 生成截面报告
- [ ] Export to Paraview

### Additional Modules:
- [ ] Optimisation 结构优化
- [ ] Reinforced Concrete 钢筋混凝土
- [ ] Steel 钢结构
