# Causal Inference PPT

基于浙江大学 Beamer 模板制作的因果推理课程汇报幻灯片，主题为：

`End-To-End Causal Effect Estimation from Unstructured Natural Language Data`

## 项目说明

本目录保存 PPT 的 LaTeX 源码、模板样式文件和图片资源。
主要文件如下：

```text
ppt/
├── main.tex      # 演示文稿源文件
├── main.pdf      # 编译后的 PDF
├── zju.sty       # 浙大 Beamer 样式文件（含本地修改）
├── figures/      # logo、背景等图片资源
└── README.md     # 当前说明文档
```

## 编译环境

- TeX Live
- XeLaTeX
- macOS / Linux 均可

建议使用完整版 TeX Live，以避免中文字体、Beamer 主题或图形相关宏包缺失。

## 编译方式

在 `ppt/` 目录下执行：

```bash
xelatex -interaction=nonstopmode -halt-on-error main.tex
xelatex -interaction=nonstopmode -halt-on-error main.tex
```

说明：

- 第一次编译生成辅助文件
- 第二次编译用于稳定目录、页码和交叉引用
- 输出文件为 `main.pdf`

## 常见中间文件

编译过程中通常会生成以下中间文件：

- `main.aux`
- `main.log`
- `main.nav`
- `main.out`
- `main.snm`
- `main.toc`

这些文件不影响源代码本身，提交仓库时通常不需要保留。

## 模板说明

本项目使用的 Beamer 模板来自浙江大学模板，并在本地做了少量调整，例如：

- 修复模板初始化中的编译问题
- 调整页脚显示内容
- 适配当前课程汇报内容

## 致谢

Beamer 模板参考：
[ZJU-Beamer-Template](https://github.com/qychen2001/ZJU-Beamer-Template)
