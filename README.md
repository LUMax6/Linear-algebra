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
├── chapter5.ipynb            # 第 5 章笔记：特征值特征向量 / 特征方程 / 对角化 / 复特征值 / 差分与微分方程 / 马尔可夫链 / 迭代估计
├── chapter6.ipynb            # 第 6 章笔记：内积与正交 / 正交投影 / Gram–Schmidt 与 QR / 最小二乘 / 线性模型 / 内积空间
├── picture/
│   ├── chapter_1_picture/    # 第 1 章用图（1-1.png ~ 1-33.png）
│   ├── chapter_2_picture/    # 第 2 章用图（2-1.png ~ 2-55.png）
│   ├── chapter_3_picture/    # 第 3 章用图（3-1.png ~ 3-21.png）
│   └── chapter_6_picture/    # 第 6 章用图（6-1.png）
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


### `chapter5.ipynb` — 特征值与特征向量

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 5.1 | Eigenvectors and Eigenvalues 特征向量与特征值 | 定义 $Ax=\lambda x$、特征空间（零空间）、三角矩阵特征值（定理 1）、不同特征值对应特征向量线性无关（定理 2）、判断特征向量 / 特征值、差分方程初探 |
| 5.2 | The Characteristic Equation 特征方程 | 特征多项式与特征方程 $\det(A-\lambda I)=0$、行列式性质回顾（定理 3）、0 不是特征值 ⇔ 可逆、相似与相似变换（定理 4）、QR 迭代保持特征值、$\det A=\prod\lambda_i$ |
| 5.3 | Diagonalization 对角化 | 对角化定理（定理 5）、$A=PDP^{-1}$ 的构造步骤、有 n 个不同特征值必可对角化（定理 6）、几何重数 ≤ 代数重数（定理 7）、$A^k=PD^kP^{-1}$ |
| 5.4 | Eigenvectors and Linear Transformations 线性变换的特征向量 | 抽象线性变换的特征值 / 特征向量、B-矩阵与矩阵表示、对角表示定理（定理 8）、相似 = 同一变换在不同基下的矩阵、迹的性质 |
| 5.5 | Complex Eigenvalues 复特征值 | 实矩阵复特征值成共轭对、复向量的实部 / 虚部、旋转 + 缩放基本构件 $C=\begin{bmatrix}a&-b\\b&a\end{bmatrix}$、定理 9：$A=PCP^{-1}$、实部虚部线性无关的证明、不变平面 |
| 5.6 | Discrete Dynamical Systems 离散动力系统 | 差分方程 $x_{k+1}=Ax_k$ 的通解、主导特征值与长期行为、吸引子 / 排斥子 / 鞍点 / 螺线点的几何分类、换元解耦 $y_k=P^{-1}x_k$、种群阶段矩阵模型 |
| 5.7 | Applications to Differential Equations 微分方程应用 | $x'=Ax$ 的特征函数解 $x=ve^{\lambda t}$、解耦、复特征值经欧拉公式提取实解 $y_1,y_2$、几何分类（sink/source/saddle/spiral）与 5.6 的对比、电路（RLC）建模 |
| 5.8 | Iterative Estimates for Eigenvalues 特征值的迭代估计 | 为何难以精确求特征值（阿贝尔-鲁菲尼定理 / 病态）、幂法（严格主导特征值）、收敛速率 $|\lambda_2/\lambda_1|$、反幂法（任意特征值，需初估 $\alpha$）、Rayleigh 商加速 |
| 5.9 | Applications to Markov Chains 马尔可夫链的应用 | 概率向量与随机矩阵、定理 10（1 是特征值）、稳态向量、正则随机矩阵与定理 11（唯一稳态、收敛与初值无关）、求稳态向量的两种方法对比 |
| 专题补充 | ① 相似与对角化（5.3 后）、② 微分算子的特征函数（5.7 后）、③ 马尔可夫链稳态（5.9 后）、④ 数值计算思路（5.8 后） | 相似 = 同一线性变换在不同基下，"能做相似变换"≠"可对角化"；$e^{\lambda t}$ 是微分算子 $D$ 的特征函数、$v$ 是 $A$ 的特征向量；列和为 1 ⇒ 1 是特征值，**正则性**才保证唯一稳态与收敛；QR 迭代（相似变换）把 $\lambda$ 与 $v$ **一起**算出，为第六章 QR 分解铺垫 |
| 总结 | 第五章总结 + 专题补充索引 | 逐节核心方法与关键结论汇总；主线：特征值求法 → 对角化 → 差分方程 / 微分方程 / 马尔可夫链 |


### `chapter6.ipynb` — 正交性与最小二乘

| 教材章节 | 主题 | 主要知识点 |
| :--- | :--- | :--- |
| 6.1 | Inner Product, Length, and Orthogonality 内积、长度与正交性 | 内积 $\mathbf{u}\cdot\mathbf{v}=\mathbf{u}^T\mathbf{v}$ 及其性质（定理 1）、长度 / 单位向量 / 距离、正交与勾股定理（定理 2）、正交补、四个基本子空间的正交关系（定理 3：$(\operatorname{Row}A)^\perp=\operatorname{Nul}A$、$(\operatorname{Col}A)^\perp=\operatorname{Nul}A^T$）、$\mathbb{R}^2$ / $\mathbb{R}^3$ 的夹角与相关系数 |
| 6.2 | Orthogonal Sets 正交集合 | 正交组与正交基、定理 4（非零正交组线性无关）、定理 5（正交基下的系数由内积直接给出）、向直线的正交投影、标准正交组与正交矩阵、定理 6（$U^TU=I$）、定理 7（正交变换保内积 / 长度 / 夹角）、投影矩阵 $UU^T$ |
| 6.3 | Orthogonal Projections 正交投影 | 到子空间的正交投影、定理 8（正交分解定理）、定理 9（最佳逼近定理）、定理 10（$\operatorname{proj}_W\mathbf{y}=UU^T\mathbf{y}$）、用正交基展开、最近点与距离的计算 |
| 6.4 | The Gram–Schmidt Process 格拉姆–施密特正交化 | 定理 11 Gram–Schmidt 过程、定理 12 QR 分解（$A=QR$、$R=Q^TA$）、数值稳定性讨论、Householder 反射矩阵与基于正交变换的 QR 算法 |
| 6.5 | Least-Squares Problems 最小二乘问题 | 最小二乘解与最小二乘误差、定理 13 正规方程 $A^TA\hat{\mathbf{x}}=A^T\mathbf{b}$、定理 14 解的唯一性（列线性无关 ⇔ $A^TA$ 可逆）、定理 15 QR 解法、三种解法（正规方程 / QR / 几何投影）对比 |
| 6.6 | Machine Learning and Linear Models 机器学习与线性模型 | 设计矩阵 / 观测向量 / 参数向量、最小二乘直线与回归系数、一般线性模型与多元回归、多项式 / 三角 / 指数模型、“线性”指对参数线性、均值偏差形式、误差平方和分解 $SS(T)=SS(R)+SS(E)$ |
| 6.7 | Inner Product Spaces 内积空间 | 内积公理、加权内积、积分内积 $\langle f,g\rangle=\int_a^b f(t)g(t)\,dt$、Cauchy–Schwarz 不等式（定理 16）与三角不等式（定理 17）、函数空间的正交基与 Gram–Schmidt、Legendre 多项式、极化恒等式 |
| 6.8 | Applications of Inner Product Spaces 内积空间的应用 | 加权最小二乘（化为 $WX\boldsymbol{\beta}\approx W\mathbf{y}$ 的普通最小二乘）、趋势分析（正交多项式与趋势系数）、傅里叶系数与 $n$ 阶傅里叶逼近、正交投影统一视角 |
| 习题 | 6.1 27, 29, 32, 37–42；6.2 33, 35–37, 39, 43–44；6.3 11, 19, 31–32, 35, 37–38；6.4 15, 23, 25, 27, 29–30；6.5 11, 15, 23, 25, 27, 29–31, 33–34；6.6 11, 13, 15–17, 19–20, 23, 25–26；6.7 14, 17, 31, 33–34；6.8 1, 4, 5–7, 10, 15–16 | 四个基本子空间正交关系的数值验证、正交矩阵保长度与夹角、投影矩阵 $UU^T$ 的性质、图案识别与最近点、QR 分解与 Gram–Schmidt 的数值对照、最小二乘的几何与代数解法、开普勒轨道与放射性衰变拟合、多项式速度估计、加权最小二乘与傅里叶逼近 |
| 补充 | 补充 21, 25, 30, 31, 32, 34, 37 | Bessel 不等式、Householder 矩阵（QR 的数值实现）、Rayleigh 商、四个基本子空间的关系、Schur 分解、条件数与相对误差估计 |
| 总结 | 第六章总结表 | 逐节核心公式与定理汇总；主线：内积 → 正交 → 投影 → Gram–Schmidt / QR → 最小二乘 → 线性模型 → 内积空间及其应用 |


---

## 学习进度

- [x] 第 1 章 Linear Equations in Linear Algebra（已整理）
- [x] 第 2 章 Matrix Algebra（已整理）
- [x] 第 3 章 Determinants 行列式（已整理）
- [x] 第 4 章 Vector Spaces 向量空间（已整理）
- [x] 第 5 章 Eigenvalues and Eigenvectors 特征值与特征向量（已整理）
- [x] 第 6 章 Orthogonality and Least Squares 正交性与最小二乘（已整理）
- [ ] 第 7 章及以后（持续更新中…）

---

## 参考教材

- David C. Lay, Steven R. Lay, Judi J. McDonald. *Linear Algebra and Its Applications*, 6th Edition. Pearson, 2022.
