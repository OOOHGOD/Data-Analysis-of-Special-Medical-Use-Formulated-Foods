**English** | [简体中文](README.zh-CN.md)

# Special Medical-Purpose Food Data Analysis

Three Python notebooks for Problem B of the 2024 Teddy Cup Data Analysis Skills Competition, exploring information for 182 special medical-purpose formulated foods.

**Category:** Data Analysis  
**Stack:** Python · pandas · pdfplumber · Matplotlib · seaborn · Jupyter

## Included work

| Notebook | Focus |
| --- | --- |
| [Task 1](code/任务1.ipynb) | Extract nutrition tables and instruction fields; organize categories and registration information |
| [Task 2](code/任务2.ipynb) | Visualize product/manufacturer characteristics and text-derived summaries |
| [Task 3](code/任务3.ipynb) | Demonstrate a needs-based recommendation example using a Baidu language-model API |

See the Chinese [project summary](项目总结.md) for methods and reproduction notes.

## Setup

Create and activate a virtual environment, then run:

```bash
python -m pip install -r requirements.txt
jupyter notebook
```

Start Jupyter from the repository root and open the notebooks under `code/`.

## Data and configuration

Raw instruction PDFs, Excel/CSV data, competition documents, videos, and outputs are not checked in. The original project provides a [dataset sharing link](https://pan.baidu.com/s/1mwKI2Om83O-cw2POGbWbKA?pwd=m2h1), extraction code `m2h1`. Availability and data rights must be checked separately.

Update file paths and input filenames before running cells. Task 2 includes a Windows Chinese-font path that needs adjustment on other systems. For Task 3, set credentials in the notebook kernel's environment:

```powershell
$env:BAIDU_API_KEY = "your-api-key"
$env:BAIDU_SECRET_KEY = "your-secret-key"
```

Run tasks in order where they consume earlier results. Files such as `result1.xlsx` and `result2.xlsx` are produced locally.

## Limitations

This is a competition analysis and reproduction project. The recommendation example is not a clinical recommendation system. Reproduction requires the corresponding external inputs and API access. The code license does not grant rights to product documents or datasets.

## Author and license

Author / maintainer: [https://github.com/OOOHGOD](https://github.com/OOOHGOD).

Eligible original contributions are under the [MIT License](LICENSE), permitting commercial use and modification with preservation of copyright and license notices in copies or substantial portions. [License scope](LICENSE_SCOPE.md) explains third-party exclusions and upstream terms.
