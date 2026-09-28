# my-python-project

Python 单元测试 + GitHub Actions 自动化 CI 练习项目。

## 项目结构

```
my-python-project/
├── .github/workflows/
│   └── ci.yml            # GitHub Actions 工作流
├── calculator.py         # 被测试的代码
├── test_calculator.py    # 单元测试
└── requirements.txt      # 项目依赖
```

## 本地运行

```bash
pip install -r requirements.txt
pytest -v
```

## CI

每次 push 或提 PR 时，GitHub Actions 会自动在 ubuntu-latest 上
用 Python 3.11 安装 pytest 并运行 `pytest -v`。
