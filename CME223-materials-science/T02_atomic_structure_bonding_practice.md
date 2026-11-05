---
type: tutorial
course: "CME223"
week: 2
tutorial: 2
topics:
  - atomic_structure
  - electron_configuration
  - bohr_model
  - periodic_law
related_lectures:
  - "[L02_atomic_structure_bonding](L02_atomic_structure_bonding.md)"
---

# Tutorial 2 — 原子结构与键合(I)

> [!NOTE]
> - **所属课程**: CME223
> - **关联笔记**: [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md)
> - **涉及核心概念**: 原子组成, 电子构型, Bohr 模型, 电离能, 周期律反常

---

## 本次公式速查

| 公式 | 含义 | 来源 |
|---|---|---|
| $E_n = -\dfrac{13.6}{n^2}$ eV | 氢原子能级 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $\Delta E = E_f - E_i$ | 跃迁能量差 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $E_{photon} = h\nu = \dfrac{hc}{\lambda}$ | 光子能量 | [L02_atomic_structure_bonding](L02_atomic_structure_bonding.md) |
| $\lambda$ (nm) ≈ 1240 / $E$ (eV) | 速查口诀 | $hc = 1240$ eV·nm |

## 本次数据与常数

| 符号 | 名称 | 值 |
|---|---|---|
| $h$ | Planck 常数 | $6.63 \times 10^{-34}$ J·s |
| $c$ | 光速 | $3 \times 10^8$ m/s |
| $1$ eV | 电子伏 | $1.60 \times 10^{-19}$ J |
| $1$ Rydberg | H 电离能 | $13.6$ eV |

---

## Problem 1

> What does atom consist of?

**涉及知识点**: 原子组成

**解答**:

| 粒子 | 位置 | 电荷 | 相对质量 |
|---|---|---|---|
| 质子 (proton) | 核 | $+1.60\times 10^{-19}$ C | $1.673\times 10^{-27}$ kg ≈ 1 amu |
| 中子 (neutron) | 核 | 中性 | $1.675\times 10^{-27}$ kg ≈ 1 amu |
| 电子 (electron) | 电子云 | $-1.60\times 10^{-19}$ C | $9.11\times 10^{-31}$ kg ≈ 1/1836 amu |

**关键**:核占质量(>99.95%),电子云占体积。中性原子 Z = #protons = #electrons。

**易错**:把"质量数 A"和"原子序数 Z"混为一谈;电子质量 ≠ 质子。

---

## Problem 2

> Two importances of atomic structure

**涉及知识点**: 电子构型, 化学键

**解答**(任选两点):

1. **决定化学性质与键合方式**
   价电子分布决定金属/非金属/半金属性质,进而决定形成离子键、共价键、金属键还是 Van der Waals。
   例:Na (3s¹) 易失电子 → 金属键;Cl (3s²3p⁵) 易得电子 → 与 Na 形成离子键 NaCl。

2. **决定物理性质**(导电、导热、力学)
   - 金属键(自由电子海)→ 高导电导热
   - 共价键(定域电子)→ 高硬度、绝缘
   - 离子键 → 脆、固态绝缘但熔融导电

---

## Problem 3

> Two differences between atomic number and atomic mass

**涉及知识点**: 原子序数 Z, 质量数 A

**解答**:

| 比较项 | 原子序数 Z | 原子质量数 A |
|---|---|---|
| 定义 | 核内**质子数** | 核内**质子+中子数**(同位素 A 不同) |
| 取值 | 整数,元素唯一 | 同元素不同同位素 A 不同 |
| 决定 | 化学身份(周期表位置) | 质量与核稳定性 |

---

## Problem 4

> Two reasons why understanding atomic bonding matters in chemical plants

**涉及知识点**: 化学键, 材料选型

**解答**(任选两点):

1. **耐腐蚀性**:化工厂接触强酸/碱/有机溶剂,键合方式决定材料是否被侵蚀。
   - 金属键(碳钢)在 HCl 中迅速腐蚀
   - 共价键聚合物(PTFE)C-F 键能 485 kJ/mol → 几乎全谱耐蚀
   - 离子陶瓷(玻璃/瓷)对酸碱普遍稳定 → 适合反应釜衬里

2. **耐温与机械强度**:键能直接关系到熔点。
   - 共价/离子 → 高熔点(SiC > 2000°C),适合炉衬
   - 金属键 → 中高熔点+韧性,适合压力容器
   - Van der Waals(PE)→ 低熔点(~120°C),只能常温管道

---

## Problem 5

> H 原子从 n=3 跃迁到 n=2,求 (a) 光子能量 (b) 频率 (c) 波长 (d) 吸收还是发射 (e) 属于哪个谱系

**涉及知识点**: Bohr 模型, 氢原子光谱

### 思路与估算
- n=3→n=2 是巴尔末系第一条线 H_α(可见光红区)
- **量级估算**:ΔE ≈ 13.6 × 5/36 ≈ 1.89 eV ≈ 3 × 10⁻¹⁹ J
- λ ≈ 1240/1.89 ≈ 656 nm(红光)

### 解答

**(a) 光子能量**:
$$\Delta E = -\frac{13.6}{9} - \left(-\frac{13.6}{4}\right) = 13.6 \times \frac{5}{36} = \boxed{1.889 \text{ eV}}$$
转 J:$E = 1.889 \times 1.60 \times 10^{-19} = \boxed{3.02 \times 10^{-19} \text{ J}}$

**(b) 频率**:$\nu = E/h = 3.02 \times 10^{-19} / 6.63 \times 10^{-34} = \boxed{4.55 \times 10^{14} \text{ Hz}}$

**(c) 波长**:$\lambda = c/\nu = 3 \times 10^8 / 4.55 \times 10^{14} = \boxed{659 \text{ nm}}$ (红光)

**(d) 发射**:从高能级 n=3 → 低能级 n=2,体系能量减小 → 释放光子 → **emission**。

**(e) 巴尔末系 (Balmer series),H_α 线**:终态 n=2 的所有跃迁都属此系,659 nm 在可见红光区。
- Lyman 系(n→1):紫外
- Balmer 系(n→2):可见
- Paschen 系(n→3):红外

**易错**:ΔE 公式正负号写反 → 记"光子能量 |ΔE| 取正"即可。

---

## Problem 6

> Electron configuration 概念,写 Li 的电子构型

**涉及知识点**: 电子构型, Aufbau, Pauli, Hund

**电子构型**:描述电子在主壳层(n)和亚壳层(s/p/d/f)中的分布。三大规则:
1. **Aufbau**:从低能级填到高
2. **Pauli**:每轨道最多 2 个电子,自旋反平行
3. **Hund**:简并轨道先各占 1 个 ↑,再配对

**Li (Z=3)**:
$$\boxed{\text{Li}: 1s^2\,2s^1 = [\text{He}]\,2s^1}$$

含义:1s² 是芯,2s¹ 是价电子。Li 易失这个 2s¹ → 表现为 +1 价金属(碱金属)。

---

## Problem 7

> 解释电子激发与光子发射;能量差与频率关系

**涉及知识点**: Bohr 模型, 光的粒子性

**(a) 激发**:吸收能量(光/热/电场/碰撞)等于能级差时,电子从低能级跃迁到高能级。激发态不稳定(~10⁻⁸ s)。

**发射**:激发态电子自发回到更低能级,释放单光子,能量恰好 = 能级差。能级离散 → 光子能量离散 → **线状光谱**。

**(b) 关系**:
$$\boxed{\Delta E = h\nu = \frac{hc}{\lambda}}$$

ΔE ↑ → ν ↑ → λ ↓(更紫外/X-ray)
ΔE ↓ → ν ↓ → λ ↑(更红外/微波)

---

## Problem 8

> 电离能与材料导电性的关系

**涉及知识点**: 电离能, 导电性

**解答**:

| IE 大小 | 行为 | 类型 | 导电性 |
|---|---|---|---|
| **低**(<6 eV,如 Na 5.1, Cu 7.7) | 易失价电子 → 电子海 | 金属 | 良导体(σ ~ 10⁷ S/m) |
| **中**(6-10 eV,如 Si 8.2) | 需热/光激发 | 半导体 | σ 随 T 升 |
| **高**(>10 eV,如 Ne 21.6) | 电子被牢牢束缚 | 绝缘体 | 不导电 |

**逻辑链**:低 IE → 电子易离域 → 自由载流子多 → σ 高。

**工程**:化工导线选 Cu/Al(IE 低);电气绝缘衬里选 PTFE/陶瓷(IE 高)。

**易错**:别把电离能(给走电子)和电负性(吸引电子)混。

---

## Problem 9

> 为何稀有气体 IE 极高?

**涉及知识点**: Z_eff, 闭壳层稳定

**解答**:三个原因:

1. **闭壳层电子构型(最关键)**
   - He: 1s² → n=1 满
   - Ne: 1s² 2s² 2p⁶ → n=2 满(8 电子稳定)
   闭壳是量子能量极小态,拿走一个电子破坏稳定。

2. **有效核电荷 Z_eff 大**
   Slater:Ne 中 Z=10, S≈4.15 → Z_eff ≈ 5.85(本周期最大)。

3. **原子半径小**
   Z_eff/r 大 → 核束缚强。

**数值**:He IE = 24.6 eV(全表第一);Ne IE = 21.6 eV;紧邻碱金属 Li 5.4 / Na 5.1 eV。这是周期表的标志性周期律。

---

## Problem 10

> 为何 Al 的 IE 低于 Mg?(周期律反常)

**涉及知识点**: s/p 亚壳能量差, 半满全满稳定性

**事实**:
- Mg (Z=12): [Ne] 3s² → IE = 7.65 eV
- Al (Z=13): [Ne] 3s² 3p¹ → IE = **5.99 eV**(反常低)

**原因**:

1. **失去的电子来自不同亚壳**
   - Mg 失 3s 电子(s 钻入核近,束缚紧 → 难拿)
   - Al 失 3p 电子(3p 比 3s 高能,径向更外 → 容易拿)

2. **3s² 的屏蔽**:Al 的 3p¹ 被 3s² 屏蔽,Z_eff 略降。

3. **3s² 满亚壳的额外稳定**:Mg 的 3s² 类似闭壳;Al 的 3p¹ 是孤电子,不享有这种稳定。

**类似反常**:
- N (2p³) > O (2p⁴):因 N 的 2p³ **半满**稳定
- P > S 同理
- 凡半满/全满/全空被破坏的位置,都可能 IE 反常下降

---

## 答案速查

| 题号 | 最终答案 | 涉及概念 |
|---|---|---|
| 1 | 质子+中子+电子 | 原子组成 |
| 2 | 化学性质+物理性质 | 电子构型 |
| 3 | Z=质子数;A=质子+中子 | Z 与 A |
| 4 | 耐蚀+耐温 | 化学键 |
| 5 | (a) 1.89 eV (b) 4.55×10¹⁴ Hz (c) 659 nm (d) 发射 (e) Balmer/H_α | Bohr 模型 |
| 6 | Li: 1s² 2s¹ | 电子构型 |
| 7 | ΔE = hν = hc/λ | 光子能量 |
| 8 | 低 IE → 高导电 | 电离能 |
| 9 | 闭壳+Z_eff 大+r 小 | Z_eff |
| 10 | Al 失 3p (3s² 闭壳更稳) | 周期律反常 |

---

## 知识盲区 / Gaps identified

> [!NOTE]
> 解这份 tutorial 时发现的薄弱概念,建议复习:
> - Slater 法则 — 用于定量计算 Z_eff(Q9 提到但 lecture 没详讲)
> - Rydberg 公式 通用形式 $1/\lambda = R(1/n_f^2 - 1/n_i^2)$ — Q5 用 Bohr 公式即可,但 Rydberg 式更通用
> - d 带中心理论 — Q4 工程意义题里如果细讲催化要用,L02 没讲
