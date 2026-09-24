# 线性代数及其应用 · 学习笔记

>本仓库是学习教材 **Lay, Lay & McDonald《Linear Algebra and Its Applications》(6th ed., 2022)** 时整理的个人笔记。

---

## 目录结构

```text
Linear algebra/
├── chapter1.ipynb            # 第 1 章笔记：线性方程组 / 向量 / 线性变换 / 线性模型
├── chapter2.ipynb            # 第 2 章笔记：矩阵代数 / 逆矩阵 / LU / 子空间与秩
├── chapter3.ipynb            # 第 3 章笔记：行列式 / Cramer 法则 / 面积与体积
├── chapter4.ipynb            # 第 4 章笔记：向量空间 / 零空间与列空间 / 基与维数 / 基变换 / 信号与差分方程
├── picture/
│   ├── chapter_1_picture/    # 第 1 章用图（1-1.png ~ 1-33.png）
│   ├── chapter_2_picture/    # 第 2 章用图（2-1.png ~ 2-55.png）
│   └── chapter_3_picture/    # 第 3 章用图（3-1.png ~ 3-21.png）
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


### `chapter3.ipynb` — 行列式

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 3.1 | Introduction to Determinants 行列式引论 | 2×2 / 3×3 行列式（Sarrus 对角线法则）、余子式与代数余子式、余子式展开定理（定理 1）、三角矩阵的行列式（定理 2）、行列式的面积直观 |
| 3.2 | Properties of Determinants 行列式的性质 | 行变换对行列式的影响（定理 3：行替换不变 / 行交换变号 / 行倍乘缩比）、用行化简计算行列式、可逆性判据（定理 4）、转置（定理 5）、乘积（定理 6）、行列式的多重线性性 |
| 3.3 | Cramer's Rule, Volume, and Linear Transformations 克拉默法则、体积与线性变换 | Cramer 法则（定理 7）、伴随矩阵求逆（定理 8）、面积与体积（定理 9）、线性变换对面积 / 体积的缩放（定理 10）、用外积（混合积）与多重线性性推导 Cramer 法则、椭圆 / 椭球面积体积、与前后章节的联系 |
| 习题 | 3.1 43–44, 47–51；3.2 37–42, 51–54；3.3 23, 25–26, 31, 39–41 | 随机矩阵数值验证行列式规律、几何解释（平行四边形 / 平行六面体 / 椭球体积）、伴随矩阵与 Cramer 法则的数值与运算量对比 |


### `chapter4.ipynb` — 向量空间

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 4.1 | Vector Spaces and Subspaces 向量空间与子空间 | 向量空间 10 条公理、由公理推出的基本性质、典型空间（实数组空间、信号空间、多项式空间）、子空间三条件、Span 是子空间 |
| 4.2 | Null Spaces, Column Spaces, Row Spaces 零空间、列空间、行空间 | 零空间（隐式定义）与列空间（显式定义）、定理 2/3、行空间等于列空间的转置、两者对比表、线性变换的核与值域 |
| 4.3 | Linearly Independent Sets; Bases 线性无关集与基 | 线性无关 / 相关的抽象定义、定理 4、基的定义、张成集定理（定理 5）、主元列构成列空间的基（定理 6）、行等价保持行空间（定理 7） |
| 4.4 | Coordinate Systems 坐标系 | 唯一表示定理（定理 8）、坐标向量与坐标映射、坐标变换矩阵、坐标映射是同构（定理 9）、用坐标向量判断线性相关性 |
| 4.5 | The Dimension of a Vector Space 维数 | 维数良定义（定理 10、11）、有限维与无限维、子空间维数不超过全空间维数（定理 12）、基定理（定理 13）、秩与零化度、秩定理（定理 14）、可逆矩阵定理续（m–q） |
| 4.6 | Change of Basis 基的变换 | 定理 15、坐标变换矩阵（列 = 旧基向量的新坐标）、正反变换矩阵互为逆矩阵、实数组空间中的行化简算法、三组基之间的传递关系 |
| 4.7 | Digital Signal Processing 数字信号处理 | 信号空间与常见信号（脉冲、单位阶跃、常数、交替、Fibonacci、指数）、移位变换、线性时不变（LTI）变换（定理 16）、移动平均滤波、长度 n 的信号空间同构于 n+1 维实数组空间（定理 17）、有限支撑信号空间无限维（定理 18） |
| 4.8 | Applications to Difference Equations 差分方程 | Casorati 矩阵与 Casoratian 检验、n 阶线性差分方程、辅助方程与试探解、定理 19（初值唯一解）、定理 20（齐次解空间为 n 维）、基本解组、非齐次通解结构、化为一阶方程组 |
| 习题 | 4.1 5–8, 19–20, 30, 33–37, 40–42, 44–46；4.2 40–41, 43, 45–46, 50–52；4.3 18, 36, 38, 41–42, 46–48；4.4 27–30, 38, 40–42；4.5 51–54；4.6 7, 9, 16, 19–22；4.7 10, 12, 14, 25, 27, 30, 32；4.8 17, 23–24, 27, 31, 35 | 子空间判定与公理证明、弹簧振子与连续函数空间、子空间的交与和、列空间与零空间判定、多项式与三角函数族的线性无关、晶格坐标、扩充基、升幂与降幂公式及积分应用、移动平均滤波、Fibonacci 通解、差分方程建模 |
| 总结 | 第四章总结表 | 逐节核心概念与关键结论汇总；主线：任何 n 维实向量空间都与 n 维实数组空间同构 |


---

## 学习进度

- [x] 第 1 章 Linear Equations in Linear Algebra（已整理）
- [x] 第 2 章 Matrix Algebra（已整理）
- [x] 第 3 章 Determinants 行列式（已整理）
- [x] 第 4 章 Vector Spaces 向量空间（已整理）
- [ ] 第 5 章及以后（持续更新中…）

---

## 参考教材

- David C. Lay, Steven R. Lay, Judi J. McDonald. *Linear Algebra and Its Applications*, 6th Edition. Pearson, 2022.
