# MHtoolX v1.0.0
*A multifunctional interactive mathematical tool / 多功能交互式数学工具*

---

## 📘 Overview | 概述

**MHtoolX v1.0.0** 是一个基于 Python 的命令行交互式数学计算工具，支持多种数学功能，如：
- 基础算术、阶乘、质因数分解、质数检测  
- 几何与三角函数绘图（基于 `turtle`）  
- 统计分析（均值、方差、标准差、中位数、众数）  
- 各类进制转换（十进制、二进制、十六进制）  
- 极坐标与笛卡尔坐标转换  
- 多项式求解与数值积分  
- 自动保存结果与操作历史  

该工具同时提供 **交互式菜单导航** 与 **结果导出功能**，适合教学、科研及学习用途。

---

## 🧮 Features | 功能特性

| 分类 | 功能说明 | 命令编号 |
|------|-----------|-----------|
| 🔢 基础计算 | 加减乘除、平方根、幂次运算、阶乘 | 2, 4, 5, 14 |
| 🔍 数论相关 | 质数表生成、质因数分解、GCD/LCM计算 | 1, 17, 18 |
| 📊 统计分析 | 均值、方差、标准差、中位数、众数 | 9 |
| 🧭 坐标与几何 | 极坐标转换、任意三角形面积、向量点乘 | 15, 25, 26 |
| 🧠 代数与微积分 | 多项式有理根求解、数值积分 | 28, 29 |
| 📈 图像绘制 | 一次/二次函数、三角函数绘制 | 10, 12 |
| 🔤 字符与文件 | JSON搜索、结果导出、操作历史查看 | 16, er, eh, rr, rh |
| ⚙️ 其他 | 圆周率计算、贪心算法、计时器、版本查看 | 3, 8, timer, version |

---

## 🧩 Requirements | 运行环境

**Python Version:** ≥ 3.8  

**依赖模块（部分根据功能自动检测）**：
```bash
turtle
keyboard
math
decimal
json
time
random
```

> 📌 若运行环境不支持 `turtle` 或 `keyboard`，部分功能会自动禁用并提示重启。

---

## 🚀 How to Run | 使用方法

### 1️⃣ 克隆或下载仓库
```bash
git clone https://github.com/<your-username>/MHtoolX.git
cd MHtoolX
```

### 2️⃣ 运行程序
```bash
python MHtoolX-v1.0.0.py
```

### 3️⃣ 使用交互命令
程序启动后输入以下命令：
- `menu`：查看分页菜单  
- `amenu`：查看所有功能  
- `exit`：退出程序  

例如：
```
请输入指令: 2
```
👉 选择功能“计算算术平方根”

---

## 💾 Data & History Management | 数据与历史记录管理

程序会自动在运行目录下生成以下文件：

| 文件名 | 功能说明 |
|--------|-----------|
| `result.json` | 保存历史计算结果 |
| `history.json` | 保存用户操作记录 |
| `number saved.json` | 已保存结果计数 |
| `mode.json` | 是否启用结果保存模式 |
| `No_History.json` | 是否启用操作历史保存 |
| `picture_choice.json` | 图像保存功能开关 |

可通过命令：
- `er`：导出历史计算结果到 `result.txt`  
- `eh`：导出操作历史到 `history.txt`  
- `cr` / `ch`：清空结果或操作历史  

---

## 🖼️ Example | 示例

计算圆周率（蒙特卡洛法）：
```
请输入指令: 3
请选择算法（蒙特卡洛法输3）
请输入取点数量: 100000
是否显示计算进度（1为是，2为否）: 1
圆周率约为 3.14184
```

---

## ⚖️ License | 许可证

MIT License © 2025 QU QI  
详情见：[MIT License](https://opensource.org/licenses/MIT)

---

## 🧠 Author | 作者

**Author:** QU QI  
**Version:** MHtoolX v1.0.0  
**Release Date:** 2025  

---

## 🌐 Future Plans | 后续计划

- 增加 GUI 界面（Tkinter 或 PyQt）
- 支持更复杂的符号计算（基于 `sympy`）
- 增强统计与绘图模块
- 优化输入验证与错误处理机制  
