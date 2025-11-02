# MHtoolX v2.1.0 / 多功能交互式数学工具

[English](#english) | [中文](#chinese)

<a name="chinese"></a>
## 中文文档

### 项目简介
MHtoolX v2.1.0 是一个基于 Python 的命令行交互式数学计算工具，支持33+种数学功能，涵盖从基础算术到高级数学模型的广泛领域。该工具提供 **交互式菜单导航** 与 **结果导出功能**，适合教学、科研及学习用途。

### 功能特性

#### 🔢 基础数学运算
- `2` - 计算算术平方根（逐次逼近法/牛顿迭代法）
- `4` - 求n次幂
- `5` - 四则运算（加、减、乘、除）
- `14` - 计算阶乘
- `20` - 计算排列组合

#### 🔍 数论与整数运算
- `1` - 生成质数表（普通方法/埃式筛法）
- `17` - 质因数分解
- `18` - 计算GCD与LCM
- `23` - 质数检测
- `6` - 生成斐波那契数列
- `7` - 计算黄金分割率

#### 📊 统计与数据分析
- `9` - 统计功能（平均值、加权平均值、方差、标准差、中位数、众数）
- `11` - 考试成绩数据整理

#### 📐 几何与三角学
- `15` - 极坐标转换
- `24` - 向量模长计算
- `25` - 计算任意三角形面积
- `26` - 向量点乘
- `21` - 计算三角函数值
- `22` - 弧度角度制转换

#### 🧮 代数与方程求解
- `13` - 求解二次方程
- `28` - 计算整数系数多项式的有理数解

#### ∫ 微积分与高级数学
- `29` - 计算数值积分
- `33` - 对数计算（自然对数和一般对数，使用泰勒展开法）

#### 📈 矩阵与线性代数
- `30` - 三阶方阵行列式计算
- `31` - 矩阵运算（加法、减法、乘法、转置）**← 新增功能**

#### 💰 金融与数学模型
- `32` - 常见数学模型计算（复利计算、半衰期计算、人口增长模型）
- `8` - 找零程序（贪心算法）

#### 🔄 进制与编码转换
- `19` - 十进制转二进制
- `27` - 十进制转十六进制

#### 🎨 图形绘制功能
- `10` - 绘制函数图像（一次/二次函数）
- `12` - 绘制三角函数图像（几何法/代数法）

#### 🔤 文本与文件操作
- `16` - 字符串频数统计&定位

#### ⚙️ 系统与工具命令
- `timer` - 启动计时器
- `version` - 查看版本
- `cs` - 清空屏幕
- `menu` - 查看分页菜单
- `amenu` - 查看所有功能列表
- `language` - 修改语言
- `exit` - 退出程序

#### 💾 数据管理命令
- `rr` - 查看历史计算结果
- `er` - 导出历史计算结果
- `cr` - 清空历史计算结果
- `rh` - 查看操作历史
- `eh` - 导出操作历史
- `ch` - 清空操作历史

### 运行环境

**Python 版本:** ≥ 3.8

**依赖模块**：
```python
turtle
keyboard
math
decimal
json
time
random
os
sys
fractions
collections
```

> 📌 若运行环境不支持 `turtle` 或 `keyboard`，相关功能会自动禁用并提示重启。

### 使用方法

#### 1️⃣ 下载程序
下载 `MHtoolX-v2.1.0.py` 和 `translation.json` 文件

#### 2️⃣ 运行程序
```bash
python MHtoolX-v2.1.0.py
```

#### 3️⃣ 使用交互命令
程序启动后会提示进行初始配置：
- 选择界面语言（中文/英文）
- 是否保存操作历史
- 是否启用计算结果保存功能
- 是否启用图像保存功能
- 是否启用number_saved计数功能

配置完成后，输入功能编号或命令即可使用相应功能。

### 数据与历史记录管理

程序自动在运行目录下生成以下配置文件：

| 文件名 | 功能说明 |
|--------|-----------|
| `result.json` | 保存历史计算结果 |
| `history.json` | 保存用户操作记录 |
| `number saved.json` | 已保存结果计数（可选启用） |
| `config.json` | 程序配置设置（历史保存、结果保存、图像保存等） |
| `translation.json` | 语言翻译字典 |

### 使用示例

#### 计算圆周率（蒙特卡洛法）
```
请输入指令: 3
请选择算法（莱布尼茨级数法输1，几何法输2，蒙特卡洛法输3，拉马努金公式法输4）3
请输入取点数量: 100000
是否显示计算进度（1为是，2为否）1
计算中: 100%
圆周率约为 3.14184
```

#### 矩阵转置操作
```
请输入指令: 31
请选择方法（加法请输1，减法请输2，乘法请输3，转置请输4）4
请输入所要计算矩阵的行数: 2
请输入所要计算矩阵的列数: 3
现在开始设置第1个矩阵:
现在为第1行
请依次输入方阵中的元素(从左往右): 1
请依次输入方阵中的元素(从左往右): 2
请依次输入方阵中的元素(从左往右): 3
1.0 2.0 3.0 
现在为第2行
请依次输入方阵中的元素(从左往右): 4
请依次输入方阵中的元素(从左往右): 5
请依次输入方阵中的元素(从左往右): 6
1.0 2.0 3.0 4.0 5.0 6.0 
结果:
1.0 4.0 
2.0 5.0 
3.0 6.0 
```

#### 修改语言
```
请输入指令: language
Select language / 选择语言 (1 for English, 2 for 中文): 1
Language changed / 语言已更改
The program needs to be restarted. Press the Enter key to continue
程序需要重启，按回车键继续
```

### 文件结构
```
.
├── MHtoolX-v2.1.0.py    # 主程序文件
├── translation.json      # 语言翻译配置
├── config.json           # 程序配置（自动生成）
├── history.json          # 操作历史（自动生成）
├── result.json           # 计算结果（自动生成）
└── number saved.json     # 保存计数（可选生成）
```

### 许可证
MIT License © 2025 QU QI

### 作者
**作者:** QU QI  
**版本:** MHtoolX v2.1.0  
**发布日期:** 20251102

### 更新日志

#### v2.1.0 主要更新：
- **矩阵转置功能**：在功能31中新增矩阵转置运算
- **语言切换优化**：修改语言后自动提示重启程序
- **翻译更新**：同步更新了中英文翻译文件

#### v2.0.0 主要更新：
- **多语言支持**：添加完整的英文翻译系统
- **语言切换**：无需重启即可实时切换语言

---

<a name="english"></a>
## English Documentation

### Project Introduction
MHtoolX v2.1.0 is a comprehensive Python-based command-line interactive mathematical calculation tool supporting 33+ mathematical functions, covering a wide range from basic arithmetic to advanced mathematical models. The tool provides **interactive menu navigation** and **result export functionality**, suitable for teaching, research, and learning purposes.

### Features

#### 🔢 Basic Mathematical Operations
- `2` - Calculate square root (successive approximation/Newton's method)
- `4` - Calculate power
- `5` - Arithmetic operations (addition, subtraction, multiplication, division)
- `14` - Calculate factorial
- `20` - Calculate permutations and combinations

#### 🔍 Number Theory & Integer Operations
- `1` - Generate prime number table (normal method/sieve method)
- `17` - Prime factorization
- `18` - Calculate GCD and LCM
- `23` - Prime number check
- `6` - Generate Fibonacci sequence
- `7` - Calculate golden ratio

#### 📊 Statistics & Data Analysis
- `9` - Statistical functions (average, weighted average, variance, standard deviation, median, mode)
- `11` - Exam score analysis

#### 📐 Geometry & Trigonometry
- `15` - Polar coordinates conversion
- `24` - Calculate vector magnitude
- `25` - Calculate triangle area
- `26` - Vector dot product
- `21` - Calculate trigonometric values
- `22` - Radian-degree conversion

#### 🧮 Algebra & Equation Solving
- `13` - Solve quadratic equation
- `28` - Find rational roots of polynomial

#### ∫ Calculus & Advanced Mathematics
- `29` - Numerical integration
- `33` - Logarithm calculation (natural and general logarithms using Taylor expansion)

#### 📈 Matrix & Linear Algebra
- `30` - Calculate 3x3 matrix determinant
- `31` - Matrix operations (addition, subtraction, multiplication, **transposition**) **← New Feature**

#### 💰 Finance & Mathematical Models
- `32` - Mathematical models (compound interest, half-life, population growth)
- `8` - Change making (greedy algorithm)

#### 🔄 Base & Encoding Conversion
- `19` - Decimal to binary conversion
- `27` - Decimal to hexadecimal conversion

#### 🎨 Graphing Functions
- `10` - Draw function graphs (linear/quadratic)
- `12` - Draw trigonometric function graphs (geometric/algebraic method)

#### 🔤 Text & File Operations
- `16` - String frequency statistics & positioning

#### ⚙️ System & Utility Commands
- `timer` - Start timer
- `version` - View version
- `cs` - Clear screen
- `menu` - View paged menu
- `amenu` - View all functions list
- `language` - Change language
- `exit` - Exit program

#### 💾 Data Management Commands
- `rr` - View calculation history results
- `er` - Export calculation history
- `cr` - Clear calculation history
- `rh` - View operation history
- `eh` - Export operation history
- `ch` - Clear operation history

### Requirements

**Python Version:** ≥ 3.8

**Required Modules**:
```python
turtle
keyboard
math
decimal
json
time
random
os
sys
fractions
collections
```

> 📌 If the runtime environment doesn't support `turtle` or `keyboard`, related functions will be automatically disabled with restart prompts.

### Usage

#### 1️⃣ Download Program
Download `MHtoolX-v2.1.0.py` and `translation.json` files

#### 2️⃣ Run Program
```bash
python MHtoolX-v2.1.0.py
```

#### 3️⃣ Use Interactive Commands
After startup, the program will prompt for initial configuration:
- Select interface language (Chinese/English)
- Whether to save operation history
- Whether to enable result saving
- Whether to enable image saving
- Whether to enable number_saved counting function

After configuration, enter function numbers or commands to use corresponding functions.

### Data & History Management

The program automatically generates the following configuration files in the running directory:

| File Name | Function Description |
|-----------|---------------------|
| `result.json` | Saves calculation history results |
| `history.json` | Saves user operation records |
| `number saved.json` | Saved results count (optional) |
| `config.json` | Program configuration settings (history saving, result saving, image saving, etc.) |
| `translation.json` | Language translation dictionary |

### Examples

#### Calculate Pi (Monte Carlo Method)
```
Enter command: 3
Please select method (1 for Leibniz series, 2 for geometric method, 3 for Monte Carlo, 4 for Ramanujan formula) 3
Please enter number of points: 100000
Show calculation progress? (1 for yes, 2 for no) 1
Calculating: 100%
Pi is approximately 3.14184
```

#### Matrix Transposition
```
Enter command: 31
Enter 1 for addition, 2 for subtraction, 3 for multiplication, or 4 for transposition: 4
Please enter number of rows: 2
Please enter number of columns: 3
Now setting up matrix 1:
Now for row 1
Please enter matrix elements (left to right): 1
Please enter matrix elements (left to right): 2
Please enter matrix elements (left to right): 3
1.0 2.0 3.0 
Now for row 2
Please enter matrix elements (left to right): 4
Please enter matrix elements (left to right): 5
Please enter matrix elements (left to right): 6
1.0 2.0 3.0 4.0 5.0 6.0 
Result:
1.0 4.0 
2.0 5.0 
3.0 6.0 
```

#### Change Language
```
Enter command: language
Select language / 选择语言 (1 for English, 2 for 中文): 1
Language changed / 语言已更改
The program needs to be restarted. Press the Enter key to continue
```

### File Structure
```
.
├── MHtoolX-v2.1.0.py    # Main program file
├── translation.json      # Language translation configuration
├── config.json           # Program configuration (auto-generated)
├── history.json          # Operation history (auto-generated)
├── result.json           # Calculation results (auto-generated)
└── number saved.json     # Save count (optional)
```

### License
MIT License © 2025 QU QI

### Author
**Author:** QU QI  
**Version:** MHtoolX v2.1.0  
**Release Date:** 20251102

### Update Log

#### v2.1.0 Major Updates:
- **Matrix Transposition**: Added matrix transposition operation in function 31
- **Language Switching Optimization**: Automatic restart prompt after language change
- **Translation Updates**: Synchronized Chinese and English translation files

#### v2.0.0 Major Updates:
- **Multi-language Support**: Added comprehensive English translation system
- **Language Switching**: Real-time language switching without restart
