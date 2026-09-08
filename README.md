# 线性代数及其应用 · 学习笔记

>本仓库是学习教材 **Lay, Lay & McDonald《Linear Algebra and Its Applications》(6th ed., 2022)** 时整理的个人笔记。

---

## 目录结构

```text
Linear algebra/
├── chapter1.ipynb            # 第 1 章笔记：线性方程组 / 向量 / 线性变换 / 线性模型
├── chapter2.ipynb            # 第 2 章笔记：矩阵代数 / 逆矩阵 / LU / 子空间与秩
├── picture/
│   ├── chapter_1_picture/    # 第 1 章用图（1-1.png ~ 1-33.png）
│   └── chapter_2_picture/    # 第 2 章用图（2-1.png ~ 2-55.png）
└── README.md
```
---

## 内容概览

### `chapter1.ipynb` — 线性代数中的线性方程

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 1.1 | Systems of Linear Equations 线性方程组 | 线性方程、方程组与解集、增广矩阵、三种初等行变换 |
| 1.2 | Row Reduction and Echelon Forms 行化简与阶梯形 | 行阶梯形 / 行最简形、主元、自由变量、相容性判定 |
| 1.3 | Vector Equations 向量方程 | 向量、线性组合、张成空间 Span |
| 1.4 | The Matrix Equation **A**x = **b** | 矩阵方程与列空间、用列向量观点看 Ax=b |
| 1.5 | Solution Sets of Linear Systems 解集 | 齐次 / 非齐次方程组的解集结构（零空间 + 特解） |
| 1.6 | Applications of Linear Systems 线性系统应用 | 实际问题的线性系统建模 |
| 1.7 | Linear Independence 线性无关 | 线性无关 / 相关、含零向量的集合、列向量判定 |
| 1.8 | Introduction to Linear Transformations 线性变换引论 | 线性变换定义、值域、线性性质 |
| 1.9 | The Matrix of a Linear Transformation 线性变换的矩阵 | 标准矩阵、单射 / 满射判定（秩角度） |
| 1.10 | Linear Models in Engineering, Science, and Statistics | 电路网络、人口迁移 / Markov 链、数学建模 |
| 补充 | Supplementary Exercises 46–47 | Givens 旋转、满射与零空间的关系 |


### `chapter2.ipynb` — 矩阵代数

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 2.1 | Matrix Operations 矩阵运算 | 加 / 数乘 / 乘法（行‑列法则）、转置、矩阵幂、矩阵乘法的几何意义与适用范围 |
| 2.2 | The Inverse of a Matrix 矩阵的逆 | 逆的定义与唯一性、2×2 行列式、Gauss‑Jordan 求逆、逆的列观点与数值考量 |
| 2.3 | Characterizations of Invertible Matrices 可逆矩阵的特性 | 可逆矩阵定理（12 条等价命题）、循环蕴含证明、条件数、病态矩阵与数值稳定性 |
| 2.4 | Partitioned Matrices 分块矩阵 | 分块乘法、Schur complement、分块上三角 / 对角矩阵的求逆 |
| 2.5 | Matrix Factorizations 矩阵分解 | LU 分解、前代 / 回代、部分主元、分解在工程（电路）中的应用 |
| 2.6 | Leontief Input‑Output Model 列昂惕夫投入产出模型 | 经济投入—产出的矩阵建模 |
| 2.7 | Applications to Computer Graphics 计算机图形学应用 | 齐次坐标、2D/3D 旋转 / 平移 / 缩放、透视投影 |
| 2.8 | Subspaces of ℝⁿ | 子空间、列空间、零空间、基、主元列 |
| 2.9 | Dimension and Rank 维数与秩 | 坐标向量、维数、秩、秩定理、基定理、同构思想 |
| 补充 | Supplementary Exercise 20 | 反对易矩阵（anti‑commuting matrices） |


---

## 学习进度

- [x] 第 1 章 Linear Equations in Linear Algebra（已整理）
- [x] 第 2 章 Matrix Algebra（已整理）
- [ ] 后续章节（持续更新中…）

---

## 参考教材

- David C. Lay, Steven R. Lay, Judi J. McDonald. *Linear Algebra and Its Applications*, 6th Edition. Pearson, 2022.
