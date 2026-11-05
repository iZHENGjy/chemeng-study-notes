---
type: tutorial
course: "CME223"
week: 2
tutorial: 3
topics:
  - chemical_bonds
  - coulomb_force
  - covalent_diamond
  - hydrogen_bonding
  - dipole_moment
related_lectures:
  - "[L02_atomic_structure_bonding](L02_atomic_structure_bonding.md)"
---

# Tutorial 3 — 原子结构与键合(II)

> [!NOTE]
> - **所属课程**: CME223
> - **关联笔记**: [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md)
> - **涉及核心概念**: Metals/Metalloids/Nonmetals, 3 类主键, Coulomb 力, 共价键, 氢键, 偶极矩
> - **重要**: 本份 tutorial 完全是 L02 内容(化学键 + 库仑力 + 偶极矩),**没有 L03 晶体内容**。讲师把 L02 拆成了 T2 + T3 两份。

---

## 本次公式速查

| 公式 | 含义 | 来源 |
|---|---|---|
| $F_{attr} = \dfrac{Z_1 Z_2 e^2}{4\pi\varepsilon_0 a^2}$ | 库仑吸引力(取大小) | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $F_{rep} = \dfrac{nb}{a^{n+1}}$ | 排斥力 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $a_0 = r_{cation} + r_{anion}$ | 平衡距离 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $\mu = q \cdot d$ | 偶极矩 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| Bond order ↑ → length ↓ → energy ↑ | 键级关系 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |

## 本次数据与常数

| 符号 | 值 |
|---|---|
| $e$ | $1.602 \times 10^{-19}$ C |
| $\varepsilon_0$ | $8.85 \times 10^{-12}$ C²/(N·m²) |
| $1$ Debye | $3.336 \times 10^{-30}$ C·m |
| K⁺ 价 | +1(IA 族,失 4s¹) |
| Ca²⁺ 价 | +2(IIA 族,失 4s²) |
| O²⁻ 价 | -2(VIA,得 2 个 2p) |

---

## Problem 1

> Give TWO(2) differences between metals, metalloids and non-metals.

**涉及知识点**: 周期表分类

**推荐 2 条对比**:

| 性质 | Metals | Metalloids | Nonmetals |
|---|---|---|---|
| **导电性** | 良导体(电子海) | **半导体**(可掺杂) | 绝缘 |
| **化学行为** | 低电负性,**易失电子→阳离子** | 中等电负性 | 高电负性,**易得电子→阴离子** |

**例**:
- Metals:Fe, Cu, Al, Na
- Metalloids:**B, Si, Ge, As, Sb, Te**(周期表斜线带)
- Nonmetals:C, N, O, F, Cl

**易错**:
- 不要写"金属硬,非金属软"(反例:Na/K 软,金刚石硬)
- 不要写"金属总固体"(Hg 液态)
- "Metalloid" 中文是**类金属**,不是"金属合金"

---

## Problem 2

> Compare THREE(3) primary bonds in TWO(2) aspects.

**涉及知识点**: Ionic, Covalent, Metallic

**注意**: Primary 不包括 Secondary(Van der Waals/H 键)。

### 推荐 2 个对比维度

**Aspect 1 — 形成机制**:
- **Ionic**:金属(低 χ)**完全转移**电子给非金属(高 χ),库仑静电
- **Covalent**:相近电负性原子**共享电子对**
- **Metallic**:阳离子 + 离域**电子海**

**Aspect 2 — 方向性**:
- **Ionic**: **无方向**(各向同性静电)
- **Covalent**: **有方向**(轨道沿空间特定方向,如 sp³ 109.5°)
- **Metallic**: **无方向**(电子海各向均匀)

### 完整数据(供其他维度选)

| 维度 | Ionic | Covalent | Metallic |
|---|---|---|---|
| 键能 | **600-1500** kJ/mol | 150-1000 | 100-800 |
| Δχ | > 1.7 | < 1.7 | ≈ 0 |
| 例子 | NaCl, MgO | 金刚石, F₂ | Fe, Cu |
| 导电 | 固态绝缘,熔/水溶导 | 绝缘(石墨例外) | **良导** |
| 力学 | 硬而脆 | 硬而脆 | 强而韧,**可锻** |

**易错**:
- Secondary 不是 primary
- 金属键 / 离子键**都无方向**
- 共价键有方向

---

## Problem 3

> 求 K⁺ 与 O²⁻ 在 1.5 nm 距离的吸引力。**Ans: 2.05 × 10⁻¹⁰ N**

**涉及知识点**: Coulomb 力

### 思路
$Z_1 = +1, Z_2 = -2, |Z_1 Z_2| = 2$;$a = 1.5 \times 10^{-9}$ m

### 解答

$$|F| = \frac{|Z_1 Z_2| \cdot e^2}{4\pi\varepsilon_0 a^2} = \frac{2 \times (1.602 \times 10^{-19})^2}{4\pi \times 8.85 \times 10^{-12} \times (1.5 \times 10^{-9})^2}$$

分子:$2 \times 2.566 \times 10^{-38} = 5.133 \times 10^{-38}$ C²
分母:$4\pi \times 8.85 \times 10^{-12} \times 2.25 \times 10^{-18} = 2.502 \times 10^{-28}$

$$|F| = \frac{5.133 \times 10^{-38}}{2.502 \times 10^{-28}} = \boxed{2.05 \times 10^{-10} \text{ N}} ✓$$

**易错**:
- K⁺ 是 **+1**(IA 失 4s¹),O²⁻ 是 **-2**(VIA 得 2 个 2p)
- a 必须换 m:1.5 nm = 1.5 × 10⁻⁹ m(不换会差 18 个数量级)
- e² ≈ 2.566 × 10⁻³⁸ C²

---

## Problem 4

> Ca 和 O 离子半径 0.100 nm 和 0.140 nm,求 (i) 平衡引力 (ii) 排斥力(b=1.70×10⁻⁹⁹ N·m⁹, n=8)。**Ans: F_attr=1.599×10⁻⁸ N, F_rep=5.148×10⁻¹² N**

**涉及知识点**: Coulomb 力, 排斥力

### 思路与估算
- $a_0 = r(Ca^{2+}) + r(O^{2-}) = 0.100 + 0.140 = 0.240$ nm
- Ca²⁺(+2) + O²⁻(-2),$|Z_1 Z_2| = 4$

### (i) 吸引力 F_attr

$a_0 = 2.40 \times 10^{-10}$ m,$a_0^2 = 5.76 \times 10^{-20}$ m²

$$|F_{attr}| = \frac{4 \times (1.602 \times 10^{-19})^2}{4\pi \times 8.85 \times 10^{-12} \times 5.76 \times 10^{-20}}$$

分子:$4 \times 2.566 \times 10^{-38} = 1.027 \times 10^{-37}$
分母:$4\pi \times 8.85 \times 10^{-12} \times 5.76 \times 10^{-20} = 6.406 \times 10^{-30}$

$$\boxed{F_{attr} = 1.60 \times 10^{-8} \text{ N}} ✓$$

### (ii) 排斥力 F_rep

$F_{rep} = \dfrac{nb}{a^{n+1}}$,n=8 → 分母 $a^9$

$a^9 = (2.40 \times 10^{-10})^9$:用对数 $\log 2.40 = 0.3802 \times 9 = 3.4218$ → $2.642 \times 10^3$
所以 $a^9 = 2.642 \times 10^{-87}$ m⁹

$$F_{rep} = \frac{8 \times 1.70 \times 10^{-99}}{2.642 \times 10^{-87}} = \boxed{5.15 \times 10^{-12} \text{ N}} ✓$$

**易错**:
- Ca²⁺ 是 **+2**(IIA 失两个 4s)
- $a^{n+1}$:n=8 时是 $a^9$ 不是 $a^8$
- 题目"radii"已是离子半径,不是原子半径
- 验算:F_rep 比 F_attr 小 4 个量级,**理论上 a₀ 处净力 = 0**;但题目数据有简化,以课件答案为准

---

## Problem 5

> 金刚石的键合类型?键合和结构如何决定其性质?

**涉及知识点**: 共价键, sp³ 杂化, 金刚石

### 解答

**键类型**: **100% 共价键**(C-C),由 sp³ 杂化形成 4 个等价四面体键(键角 109.5°)。

**关键性质 + 解释**:

| 性质 | 数值 | 结构-键合解释 |
|---|---|---|
| **极硬** | Mohs 10(自然界最硬) | 3D 网络中每个 C 锁死,任何方向变形都打破强方向性共价键 |
| **极高熔点** | **3550 °C** | 键能 711 kJ/mol,熔化要打破整个 3D 网络 |
| **绝缘** | ρ ~ 10¹⁶ Ω·cm,带隙 5.5 eV | 价电子全锁定在共价键中,无自由电子 |
| **高热导** | ~2200 W/(m·K) | 刚性 sp³ 网络 → 声子(晶格振动)极快传播,**不靠电子** |
| **光学透明** | 对可见光透明 | 带隙 5.5 eV >> 可见光能量(1.5-3 eV) |
| **脆** | 沿 (111) 解理 | 共价键有强方向性,无法像金属键滑动 |

**易错**:
- 金刚石没有金属键(这是它绝缘的原因)
- "硬"和"强/韧"不同:金刚石**硬但脆**
- "高热导但绝缘"是因为热导靠声子,不只靠电子
- sp³ 是金刚石,**sp²** 是石墨(性质完全不同:软/导电)

---

## Problem 6

> 水分子的分子内和分子间作用力?

**涉及知识点**: 极性共价键, 氢键

### 分子内 (Intramolecular)

**Polar covalent bonds (O-H)**:
- O 电负性 3.5,H 电负性 2.1,**Δχ = 1.4** → 极性共价
- 电子云偏向 O,O 部分带 δ⁻,H 部分带 δ⁺
- 键能 ~500 kJ/mol(强主键),键长 0.10 nm
- 几何:**键角 104.5°**(略小于 109.5°,因 O 上的 2 对孤对电子排斥更强)

### 分子间 (Intermolecular)

按强度从大到小:

| 类型 | 描述 | 键能 |
|---|---|---|
| **Hydrogen Bond** | δ⁺ H 与邻分子 δ⁻ O 的孤对 → O-H...O 几乎共线;每个 H₂O 形成 **4 个氢键** | 20-50 kJ/mol |
| Dipole-Dipole | 永久偶极相互吸引(实质是氢键的一部分) | 几 kJ/mol |
| London Dispersion | 电子云瞬时涨落 | < 5 kJ/mol |

> [!TIP]
> **氢键是水反常物性的根源**
> - 沸点 100°C 异常高(同族 H₂S 只 -60°C)
> - 冰浮于水(开放六边形 H 键网络 → 体积膨胀)
> - 高比热 / 高表面张力

**易错**:
- 氢键是 **intermolecular**,不是 intramolecular
- O-H 是**极性共价键**,不是普通共价键
- 键角 **104.5°**,不是 109.5°
- 氢键是 secondary 但**最强的次级键**

---

## Problem 7

> 键长与键能的关系(举例)

**涉及知识点**: Bond Order, 键能

### 关系

$$\boxed{\text{Bond order ↑ → length ↓ → energy ↑}}$$

物理原因:键长 ↓ → 核间近 → 电子云重叠深 → 核对电子吸引强 → 拆键能量大。

### 例 1: Carbon-Carbon(必背)

| 键 | Order | 长度 (nm) | 键能 (kJ/mol) | 例子 |
|---|---|---|---|---|
| C−C | 1 | **0.154** | **370** | 乙烷 H₃C-CH₃ |
| C=C | 2 | **0.130** | **680** | 乙烯 H₂C=CH₂ |
| C≡C | 3 | **0.120** | **890** | 乙炔 HC≡CH |

观察:从单到三键,长度缩 22%,键能 ~2.4 倍。

### 例 2: F₂ / O₂ / N₂(必背)

| 分子 | Order | 键能 (kJ/mol) |
|---|---|---|
| F₂ | 1 | **160** |
| O₂ | 2 | **498** |
| N₂ | 3 | **945** |

观察:键级 1→3,键能几乎 6 倍增长。这就是 **N₂ 极稳定、F₂ 易反应**的原因。

**易错**:不要把关系说反,是"短→强"。

---

## Problem 8

> 解释 secondary bonding,给 2 个偶极矩例子

**涉及知识点**: Secondary Bond, Dipole Moment

### Secondary Bonding 解释

**Weak electrostatic attractions between electric dipoles**,源自正负电荷分离。

| 项目 | 数据 |
|---|---|
| 键能 | **0.1 - 50 kJ/mol**(主键的 1/10 到 1/1000) |
| 偶极矩 | **μ = q · d**(电荷 × 距离) |
| 决定 | 低熔点、易挥发、低硬度 |

**3 类**:
1. **Fluctuating Dipole**(London 色散力)— 电子云**瞬时**不对称
2. **Permanent Dipole-Dipole** — 分子结构永久不对称
3. **Hydrogen Bond** — 最强的 secondary

### Example 1: Fluctuating Dipole(He / Ar 等惰性气体)

- He 单原子,平均 μ = 0(对称)
- 但**瞬间** 2 个电子可能偏一侧 → 临时偶极
- 诱导邻居 → 同步偶极 → 弱吸引
- 这就是 He 在 4.2 K 才液化的原因

### Example 2: Permanent Dipole(H₂O 或 CH₃Cl)

**(a) H₂O**:
- O-H 极性键 + 弯曲 104.5° → 偶极不抵消
- $\mu \approx 1.85$ D = $6.17 \times 10^{-30}$ C·m

**(b) CH₃Cl**:
- 不对称四面体(3 H + 1 Cl)→ 偶极不抵消
- $\mu \approx 1.87$ D
- **对比**:**CH₄ 对称 → μ = 0**(尽管单 C-H 有微弱极性)

> [!TIP]
> **关键对比**
> CH₄(对称)μ = 0 vs CH₃Cl(不对称)μ ≠ 0 — L02 课件 Slide 54 核心例子。

**易错**:
- CH₄ μ = 0(分子整体对称),但单 C-H 是极性键 — 别把"分子整体偶极"与"键的极性"混
- 氢键属 secondary 但**最强**(20-50 kJ/mol)
- "涨落偶极" = "London 色散力"(同一种力两个名)
- He 间也有键,只是极弱

---

## 答案速查

| 题号 | 最终答案 | 涉及概念 |
|---|---|---|
| 1 | 导电性+电子转移倾向 | 周期表分类 |
| 2 | 形成机制+方向性 | 3 类主键 |
| 3 | F = 2.05×10⁻¹⁰ N | Coulomb |
| 4 | (i) F_attr=1.60×10⁻⁸ N (ii) F_rep=5.15×10⁻¹² N | Coulomb + Repulsion |
| 5 | 100% 共价(sp³)→ 硬+绝缘+高熔点+高热导 | 金刚石 |
| 6 | 内:极性共价 O-H;间:氢键(主)+ 偶极 + 色散 | 氢键 |
| 7 | Bond order ↑ → length ↓ → energy ↑ | 键级 |
| 8 | Secondary 弱电偶极吸引;He(涨落)+ H₂O(永久) | 偶极矩 |

---

## 知识盲区 / Gaps identified

> [!NOTE]
> - Born exponent n — Q4 用 n=8,但教材常用 n=9,这两个值哪个更准?
> - Debye 单位 — μ 单位 Debye 怎么和 SI 单位 C·m 换算?(1 D = 3.336×10⁻³⁰ C·m)
> - 偶极矩矢量合成 — H₂O 怎么从两个 O-H 偶极算出净 1.85 D?(用矢量加法,涉及 cos 104.5°/2)
> - Hydration shell — 水溶解离子化合物的微观机制(Q6 变式)
