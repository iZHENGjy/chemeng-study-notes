---
type: tutorial
course: "CME223"
week: 3
tutorial: 4
topics:
  - crystal_structures
  - bcc_fcc_hcp
  - apf
  - density_calculation
related_lectures:
  - "[L03_crystal_structures_defects](L03_crystal_structures_defects.md)"
  - "[L01_intro_to_materials_science](L01_intro_to_materials_science.md)"
  - "[L02_atomic_structure_bonding](L02_atomic_structure_bonding.md)"
---

# Tutorial 4 — 晶体结构与缺陷(I)

> [!NOTE]
> - **所属课程**: CME223
> - **关联笔记**: [L01_intro_to_materials_science](L01_intro_to_materials_science.md) / [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) / [L03_crystal_structures_defects](L03_crystal_structures_defects.md)
> - **涉及核心概念**: BCC, FCC, HCP, APF, 滑移系, 体积密度

---

## 本次公式速查

| 公式 | 含义 | 来源 |
|---|---|---|
| BCC: $a = 4R/\sqrt{3}$, N=2, CN=8, APF=0.68 | BCC 几何 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| FCC: $a = 4R/\sqrt{2} = 2\sqrt{2}R$, N=4, CN=12, APF=0.74 | FCC 几何 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| HCP: $a = 2R$, c/a=1.633, N=6, CN=12, APF=0.74 | HCP 几何 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| $\rho = \dfrac{n A}{V_{cell} N_A}$ | 体积密度 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |

## 本次数据与常数

| 符号 | 值 |
|---|---|
| $N_A$ | $6.022 \times 10^{23}$ /mol |
| $A_{Ta}$ | 180.90 g/mol(Q5) |
| $\rho_{Ta}$ | 16.6 g/cm³(Q5) |

---

## Problem 1

> Explain how atomic structure controls materials, catalysts, and process performance.

**涉及知识点**: 原子结构, 键合, 催化, 选材

**思路**:从微观→宏观分三层(材料/催化/工艺)讲清。

### 解答

**(a) 对材料性能的控制**:
- 键合类型决定基本属性:
  - 金属键 → 自由电子海 → 导电、导热、延展性好
  - 共价键 → 方向性强 → 高硬度、高熔点、绝缘(金刚石)
  - 离子键 → 静电吸引 → 脆、高熔点、熔融态导电(NaCl)
- 晶体结构(BCC/FCC/HCP)决定:
  - **滑移系数量** → 延展性(FCC > BCC > HCP)
  - APF → 密度、扩散
- 缺陷密度(空位、位错)决定:屈服强度、扩散、蠕变

**(b) 对催化剂性能的控制**:
- **表面原子配位数**:角点/边缘/平台位活性不同
- **晶面取向**:不同 hkl 面活性差几个数量级(Pt(111) vs Pt(100) 对 CO 氧化)
- **电子结构**(d 带中心)决定吸附强度 — Sabatier 原理
- 缺陷与掺杂常是真正活性位

**(c) 对工艺性能的控制**:
- 反应器选材:BCC Fe vs FCC γ-Fe(高温更耐压)
- 热交换器:Cu (FCC) 高导热依赖电子海
- 腐蚀失效:晶界(高缺陷区)是首攻位置
- 加工性:HCP 镁合金滑移系少 → 难冷加工 → 需热成型

**易错**:别只讲强度;要分清"原子结构"(电子)和"晶体结构"(空间)。

---

## Problem 2

> 哪种晶体结构最适合做高压反应器外壳?

**涉及知识点**: FCC, 滑移系, 韧脆转变

**结论**: **FCC 最合适**(典型:奥氏体不锈钢 304/316,γ-Fe 基)

### 解答

| 性能要求 | FCC 表现 | 原因 |
|---|---|---|
| 延展性高 | 12 个滑移系 {111}⟨110⟩,且滑移所需应力低 | 致密面 (111) 容易滑移 |
| 韧性好 | **无明显韧脆转变温度 DBTT** | 滑移系全温度可激活 |
| 强度足够 | 通过固溶+加工硬化 | 缺陷阻碍位错 |
| 耐蚀性 | Cr 形成致密 Cr₂O₃ 钝化膜 | 适合化工腐蚀 |
| 可焊接 | 单相奥氏体焊缝不脆化 | — |

**为什么不选 BCC?**
- 有韧脆转变温度(钢 -20~0°C)→ 低温脆断风险
- BCC 滑移系 {110}⟨111⟩ 的 CRSS 远高于 FCC

**为什么不选 HCP?**
- 只有 3 个独立滑移系(基面 (0001))→ 极脆
- 一受力就裂

**实际工程**:
- 中低压常温:Q345R(BCC,便宜)
- 高压腐蚀低温:**316L 不锈钢**(FCC)
- 极端:Inconel 625(Ni 基 FCC)

**易错**:别只说"FCC 强度高",真正风险是**脆断**。

---

## Problem 3

> What is the significance of atomic packing factor (APF)?

**涉及知识点**: APF, 空间利用率

### 解答

$$\text{APF} = \frac{n \cdot \frac{4}{3}\pi r^3}{V_{cell}}$$

| 结构 | APF |
|---|---|
| SC | 0.52(几乎只 Po) |
| BCC | 0.68 |
| FCC / HCP | 0.74(理论上限) |

**4 个意义**:

1. **空间利用率** — 衡量原子填得多满
2. **关联密度** — γ-Fe(FCC, 8.0 g/cm³)> α-Fe(BCC, 7.87)→ 钢淬火 γ→α 体积膨胀
3. **关联力学** — APF 高 → 密排面多 → 滑移系多 → 延展性好(但 HCP 反例:APF 高但只 1 个基面)
4. **关联熔点 + 扩散** — APF 高 → 原子近 → 熔点高;但间隙小,间隙原子(C/N)扩散慢
   - **反直觉**:渗碳要在 γ-Fe(FCC)做,因为 FCC 八面体间隙(0.414r)实际比 BCC(0.155r)大

**易错**:
- APF 高 ≠ 必定延展性好(HCP 反例)
- APF 高 ≠ 间隙小(FCC 八面体间隙 > BCC)
- 别把 APF 和密度搞混(APF 无量纲,密度还要乘原子量)

---

## Problem 4

> 说出 BCC、FCC、HCP 三种结构的两点不同

**涉及知识点**: BCC, FCC, HCP, 滑移系

### 完整对比表

| 项目 | BCC | FCC | HCP |
|---|---|---|---|
| 单胞原子数 N | 2 | 4 | 6 |
| 配位数 CN | 8 | 12 | 12 |
| a-R | $4R/\sqrt{3}$ | $2\sqrt{2}R$ | $a=2R$, c/a=1.633 |
| APF | 0.68 | **0.74** | **0.74** |
| 密排面 | {110} | **{111}** | **(0001) 基面** |
| 滑移系数量 | 12(高 CRSS) | 12(低 CRSS) | **3(基面)** |
| 延展性 | 中 | **好** | 差 |
| 典型金属 | α-Fe, Cr, W, Mo | γ-Fe, Cu, Al, Ni | Mg, Zn, Ti, Co |
| 韧脆转变 | 有 DBTT | 无 | 极脆 |

### 两个核心差异(答题用)

**差异 1: APF 与配位数**
- BCC: APF=0.68, CN=8
- FCC: APF=0.74, CN=12(理论最致密)
- HCP: APF=0.74, CN=12(同样最致密)
→ 同元素 BCC 密度通常低于 FCC(α-Fe vs γ-Fe)

**差异 2: 延展性与滑移系**
- FCC: 12 滑移系,低 CRSS → 最易冷加工
- BCC: 12 滑移系,高 CRSS,有韧脆转变 → 中等
- HCP: 3 独立滑移系 → 难冷加工,需热成型

**(可选)差异 3: 堆叠序列** — FCC=ABCABC, HCP=ABABAB

**易错**:
- BCC 不是最致密(APF 0.68 不是最高)
- BCC 配位数 8 不是 12
- HCP c/a 理想 1.633,实际偏离(Mg 1.624, Zn 1.856, Ti 1.587)

---

## Problem 5

> Ta 是 BCC 结构,密度 16.6 g/cm³,原子量 180.90 g/mol,求原子半径。**Ans: 0.1432 nm**

**涉及知识点**: BCC, 密度公式

### 思路与估算
1. 由密度公式反解 a
2. 由 BCC 几何 $a = 4r/\sqrt{3}$ 得 $r = a\sqrt{3}/4$

**量级估算**: Ta 重元素(180 g/mol),密度 16.6 ≈ 2 倍 Fe(7.87)。a ≈ 0.33 nm,r ≈ 0.14 nm。

### 解答

**第一步:求 a³**
$$a^3 = \frac{n A}{\rho N_A} = \frac{2 \times 180.90}{16.6 \times 6.022 \times 10^{23}}$$

分子 = 361.80 g/mol;分母 = $9.997 \times 10^{24}$ g/(mol·cm³)
$$a^3 = 3.619 \times 10^{-23} \text{ cm}^3$$

**第二步:开立方**
$$a = (3.619 \times 10^{-23})^{1/3} = 3.307 \times 10^{-8} \text{ cm} = 0.3307 \text{ nm}$$

**第三步:由 BCC 几何 $4r = a\sqrt{3}$**
$$r = \frac{a\sqrt{3}}{4} = \frac{0.3307 \times 1.7321}{4} = \boxed{0.1432 \text{ nm}}$$ ✓

**对照**:与文献 Ta r ≈ 0.143 nm 一致。

**易错**:
- BCC 是 $4r = a\sqrt{3}$,**不是** $4r = a\sqrt{2}$(那是 FCC)
- BCC 单胞原子数 n = **2**(角 8×1/8 + 体心 1)
- 单位:密度 g/cm³ → a 出来是 cm,要 ×10⁷ 转 nm

**变式**:已知 r 反求密度;FCC 用 $a = 2\sqrt{2}r$, n=4。

---

## 答案速查

| 题号 | 最终答案 | 涉及概念 |
|---|---|---|
| 1 | 三层(材料/催化/工艺) | 原子结构 |
| 2 | FCC(奥氏体不锈钢)最佳 | 滑移系, 韧脆转变 |
| 3 | APF 衡量空间利用率,4 个意义 | APF |
| 4 | APF + 滑移系 是核心差 | BCC vs FCC vs HCP |
| 5 | r = 0.1432 nm | 密度公式 |

---

## 知识盲区 / Gaps identified

> [!NOTE]
> - d 带中心理论 — Q1 催化部分提到,L02 没详讲
> - Sabatier 原理 — 同上
> - 韧脆转变温度 DBTT — Q2 提到,L03 没单独讲
> - 八面体间隙 vs 四面体间隙 — Q3 提到 FCC 八面体间隙 0.414r,L03 没系统讲
