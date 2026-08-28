# B题：特殊医学用途配方食品数据分析

2024 年（第 7 届）“泰迪杯”数据分析技能赛 B 题项目。项目围绕 182 款特殊医学用途配方食品，完成营养成分与说明书字段提取、生产概况可视化和基于需求的推荐。

GitHub 仓库：[OOOHGOD/Data-Analysis-of-Special-Medical-Use-Formulated-Foods](https://github.com/OOOHGOD/Data-Analysis-of-Special-Medical-Use-Formulated-Foods)

## 目录说明

- `code/任务1.ipynb`：任务 1，说明书字段与营养成分提取、分类和注册证号解析。
- `code/任务2.ipynb`：任务 2，生产概况可视化。
- `code/任务3.ipynb`：任务 3，基于百度文心接口的推荐示例。
- `dataset/`：通过网盘分享的文件：数据链接: https://pan.baidu.com/s/1mwKI2Om83O-cw2POGbWbKA?pwd=m2h1 提取码: m2h1 
- `题目/`：竞赛题目和提交说明 PDF。
- `讲解/`：代码讲解视频、运行教程、更新记录和推荐结果参考文件。
- `项目总结.md`：项目方法、成果、局限和复现说明。

## 本地运行

建议在项目根目录启动 Jupyter，并打开 `code/` 中的任务笔记本。任务 1、2 需要项目外部或本地准备输入数据；任务 3 还需要配置百度 API 环境变量：

```powershell
$env:BAIDU_API_KEY = "your-api-key"
$env:BAIDU_SECRET_KEY = "your-secret-key"
jupyter notebook
```

依赖见 `requirements.txt`。推荐使用虚拟环境安装，不要把 API 密钥写入笔记本或提交到 Git。

## 资料说明

题目 PDF 和提交说明位于 `题目/`，其中的“任务 1/2/3”和提交格式属于赛题要求，不是本 README 的新增开发要求。参赛名单、获奖名单和教学视频属于参考资料，不是代码运行依赖。

项目方法、成果、局限和复现说明见 [项目总结.md](项目总结.md)。

## GitHub 发布范围

GitHub 仓库只发布可审阅的代码、依赖说明、README 和项目总结；原始说明书、Excel/CSV 数据、结果文件、视频和参赛资料由 `.gitignore` 排除，避免仓库过大、重复上传或泄露密钥。
