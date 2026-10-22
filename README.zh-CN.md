<div align="center">

# 特殊医学用途配方食品数据分析

以 Python Notebook 完成信息提取、数据分析与可视化。

[English](README.md) · **简体中文**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square) [![MIT License](https://img.shields.io/badge/License-MIT-2563EB?style=flat-square)](LICENSE)

</div>

<p align="center">
<a href="#项目概览">项目概览</a> · <a href="#快速开始">快速开始</a> · <a href="#内容导航">内容导航</a> · <a href="#作者与许可">作者与许可</a>
</p>

---

> **项目定位** · 竞赛数据分析


## 项目概览

2024 年第 7 届“泰迪杯”数据分析技能赛 B 题项目，围绕 182 款特殊医学用途配方食品，完成文档信息抽取、描述性分析与可视化，并提供基于 Baidu API 的推荐示例。

## 内容导航

| Notebook | 主要内容 |
| --- | --- |
| [任务 1](code/任务1.ipynb) | 用 pdfplumber 与 pandas 提取营养成分表、说明书字段、分类与注册信息 |
| [任务 2](code/任务2.ipynb) | 产品、生产企业与文本信息的可视化分析 |
| [任务 3](code/任务3.ipynb) | 使用 Baidu LLM API 演示基于需求的推荐流程 |
| [项目总结](项目总结.md) | 方法、成果、局限与复现说明 |

## 快速开始

创建并激活虚拟环境后，在仓库根目录运行：

```bash
python -m pip install -r requirements.txt
jupyter notebook
```

打开 `code/` 中的 Notebook，先检查输入路径，再按任务顺序运行相关单元格。`result1.xlsx`、`result2.xlsx` 等为本地生成结果。

## 数据与 API 配置

原始 PDF、Excel / CSV、赛题文档、视频与输出文件未纳入当前 GitHub 发布范围。原项目提供的[数据分享链接](https://pan.baidu.com/s/1mwKI2Om83O-cw2POGbWbKA?pwd=m2h1)提取码为 `m2h1`；链接可用性和数据授权需分别核对。

- 按本地数据位置调整 Notebook 中的输入路径与文件名。
- 任务 2 使用 Windows 中文字体路径，其他系统需替换为本机字体。
- 任务 3 需要在 Notebook Kernel 对应的环境中配置凭据：

```powershell
$env:BAIDU_API_KEY = "your-api-key"
$env:BAIDU_SECRET_KEY = "your-secret-key"
```

## 资料与复现范围

原始说明书、数据文件、结果、视频与竞赛材料通过 `.gitignore` 排除；GitHub 主要提供可审阅代码、依赖说明与项目总结。原说明书和赛题中的任务要求属于历史材料，不是本 README 新增的开发要求。

本项目用于竞赛分析与方法复现；API 推荐示例不构成临床建议。复现需准备对应输入、环境和 API 权限，代码许可证不覆盖产品资料与 Dataset。

## 作者与许可

作者 / 维护者：[OOOHGOD](https://github.com/OOOHGOD) · 原创贡献：[MIT License](LICENSE)

允许商用和修改；分发软件副本或实质部分时，须保留版权与许可声明。第三方代码、数据、模型和媒体素材保留各自权利，详见 [许可适用范围](LICENSE_SCOPE.md)。
