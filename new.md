# 一站式 AI 平台复刻计划
适合新手 Python，每天执行 Cursor Prompt 手写复刻 AI 平台
总阶段：Phase 0 ~ Phase 5
每阶段包含每日任务、Cursor Prompt、文件路径、示例代码和卡点

---

# Phase 0：项目起步（第 1 周）

## Day 1：Hello World + Flask 启动
**Cursor Prompt:**
"""
目标：创建最小可运行 Flask 项目
文件路径：app/main.py
步骤：
1. 创建 app/main.py
2. 写 GET "/" 返回 "hello world"
3. 注释每行代码解释 Flask 启动流程
4. 提示新手卡点：端口被占用、虚拟环境未激活
"""
**示例代码:**
```python
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
    # 返回最简单的文字
    return "hello world"

if __name__ == "__main__":
    app.run(debug=True)
