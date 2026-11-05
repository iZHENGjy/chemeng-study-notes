---
type: tutorial
course: "CME223"
week: 3
tutorial: 5
topics:
  - linear_atomic_density
  - planar_atomic_density
  - bcc_fcc_geometry
related_lectures:
  - "[L03_crystal_structures_defects](L03_crystal_structures_defects.md)"
---

# Tutorial 5 — 原子密度(线密度 + 面密度)

> [!NOTE]
> - **所属课程**: CME223
> - **关联笔记**: [L03_crystal_structures_defects](L03_crystal_structures_defects.md)
> - **涉及核心概念**: Linear Atomic Density, Planar Atomic Density, BCC, FCC
> - **题型**: 6 道(1 个概念 + 4 个计算 + 1 个工程意义)

---

## 本次公式速查

| 公式 | 含义 | 来源 |
|---|---|---|
| $\rho_l = \dfrac{\text{原子直径数 (沿方向)}}{\text{选定长度}}$ | 线密度 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| $\rho_p = \dfrac{\text{平面内原子中心数}}{\text{选定面积}}$ | 面密度 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| BCC: $a = 4R/\sqrt{3}$, N=2, CN=8 | BCC 几何 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |
| FCC: $a = 2\sqrt{2}R$, N=4, CN=12 | FCC 几何 | [L03_crystal_structures_defects](L03_crystal_structures_defects.md) |

## 本次数据与常数

| 元素 | 结构 | 原子半径 R |
|---|---|---|
| V (钒) | BCC | **0.132 nm** |
| Cu (铜) | FCC | **0.128 nm** |
| Ni (镍) | FCC | **0.1245 nm = 1.245 Å** |

---

## Problem 1

> What do you understand about atomic density?

**涉及知识点**: Atomic Density

### 解答

**Atomic density** = 单位长度 / 面积 / 体积内的原子数。三种类型:

| 类型 | 公式形式 | 单位 |
|---|---|---|
| **Volume Density** $\rho_v$ | 单胞质量 / 单胞体积 | g/cm³ 或 Mg/m³ |
| **Linear Density** $\rho_l$ | (沿某方向 [uvw] 长度上原子直径数)/ 长度 | atoms/m, atoms/nm |
| **Planar Density** $\rho_p$ | (某面 (hkl) 内原子中心数)/ 面积 | atoms/m² |

**关键概念**:线密度和面密度都是**方向/平面相关**的——不同方向 [uvw] 或不同面 (hkl) 的密度不同。

**3 个影响因素**(L03 知识块 10):
1. **Atomic mass** 原子质量
2. **Interatomic forces** 原子间力
3. **Crystal structure** 晶体结构(BCC/FCC/HCP)

**重要性**:
- 决定**滑移系**(密堆面是滑移面 → 影响延展性)
- 决定**衍射强度**(高密度面 → 强衍射峰)
- 决定**反应活性**(高密度面化学惰性更强;低密度面/边缘原子活泼)

---

## Problem 2

> V (BCC),R = 0.132 nm,求 [110] 和 [111] 方向的线密度。**Ans: ρ_[110] = 2.320 atoms/nm, ρ_[111] = 3.788 atoms/nm**

**涉及知识点**: BCC 几何, Linear Density

### 思路与估算

BCC: $a = 4R/\sqrt{3} = 4 \times 0.132 / \sqrt{3} = 0.305$ nm

- **[110]**:沿面对角线,长度 = $a\sqrt{2}$。BCC 的 (110) 面**不过体心**,所以 [110] 线只截 2 个角原子各 1/2 = **1 atom**。
- **[111]**:沿体对角线,长度 = $a\sqrt{3} = 4R$(BCC 的密排方向)。截 2 个角原子各 1/2 + 1 个体心 = **2 atoms**。

### (a) ρ_[110]

长度 = $a\sqrt{2} = 0.305 \times 1.414 = 0.4313$ nm

$$\rho_{l[110]} = \frac{1 \text{ atom}}{0.4313 \text{ nm}} = \boxed{2.32 \text{ atoms/nm}} ✓$$

### (b) ρ_[111]

长度 = $a\sqrt{3} = 0.305 \times 1.732 = 0.5283$ nm = $4R$

$$\rho_{l[111]} = \frac{2 \text{ atoms}}{0.5283 \text{ nm}} = \boxed{3.79 \text{ atoms/nm}} ✓$$

### 验证一致性
- 课件答案 2.320 / 3.788 atoms/nm,本计算 2.32 / 3.79 一致 ✓
- ρ_[111] > ρ_[110]:BCC 的 **[111] 是密堆方向**(原子相切),[110] 不是

**易错**:
- BCC [110] 不过体心(体心不在 (110) 面上)→ 只 1 个原子
- BCC [111] 是密堆方向(原子从角到体心到角)→ 2 个原子
- 长度公式:[110] 是 $a\sqrt{2}$,[111] 是 $a\sqrt{3}$
- 别把 BCC 当 FCC 来算

---

## Problem 3

> Cu (FCC),R = 0.128 nm,求 [111] 方向线密度。**Ans: 1.595 × 10⁹ atoms/m**

**涉及知识点**: FCC 几何, Linear Density

### 思路与估算

FCC: $a = 2\sqrt{2}R = 2 \times 1.414 \times 0.128 = 0.3621$ nm

**FCC [111] 是体对角线方向**:
- 长度 = $a\sqrt{3} = 0.3621 \times 1.732 = 0.6271$ nm
- 但 FCC 在 [111] 方向**只有两端的角原子**(面心原子不在体对角线上)
- 原子数 = 2 × 1/2 = **1 atom**

### 解答

$$\rho_{l[111]} = \frac{1}{0.6271 \text{ nm}} = 1.595 \text{ atoms/nm}$$

转 atoms/m:
$$\rho_l = 1.595 \times 10^9 \text{ atoms/m} = \boxed{1.595 \times 10^9 \text{ atoms/m}} ✓$$

> [!TIP]
> **关键对比:FCC [111] vs BCC [111]**
> - **FCC [111]**:体对角线**不密排**(体心和面心都不在 [111] 上)→ 1 atom
> - **BCC [111]**:体对角线**密排**(过体心)→ 2 atoms
> 这是 BCC 和 FCC 一个易混淆点!

**易错**:
- FCC [111] 不是密堆方向(密堆是 (111) **面**而不是 [111] **方向**)
- 单位转换:1 nm = 10⁻⁹ m,所以 atoms/nm × 10⁹ = atoms/m

---

## Problem 4

> Ni (FCC),原子半径 1.245 Å,求 (100) 面的面密度。

**涉及知识点**: FCC, Planar Density

### 思路与估算

R = 1.245 Å = 0.1245 nm
FCC: $a = 2\sqrt{2}R = 2 \times 1.414 \times 0.1245 = 0.3522$ nm = 3.522 Å

**FCC (100) 面**:
- 是一个 a × a 的方块
- 4 角各 1/4 + 1 个面心(完整)= 1 + 1 = **2 atoms**

### 解答

面积 = $a^2 = (0.3522 \text{ nm})^2 = 0.1240 \text{ nm}^2$

$$\rho_{p(100)} = \frac{2}{0.1240 \text{ nm}^2} = 16.13 \text{ atoms/nm}^2$$

转 atoms/m²:
$$\rho_p = 16.13 \times 10^{18} = \boxed{1.61 \times 10^{19} \text{ atoms/m}^2}$$

> 题目没给课件答案,但 FCC (100) 面密度对照可查 — 这个量级正确(典型值 1-2 × 10¹⁹)

**易错**:
- FCC (100) 面有 **5 个原子位置(4 角 + 1 面心)**,但角原子只有 1/4 在面内:4×1/4 + 1 = **2 atoms**
- 不要算成 4 个或 5 个

---

## Problem 5

> V (BCC),R = 0.132 nm,300 K 下求 (011) 面的面密度。**Ans: 1.522 × 10¹⁹ atoms/m²**

**涉及知识点**: BCC, Planar Density

### 思路与估算

V (BCC): $a = 4R/\sqrt{3} = 4 \times 0.132 / 1.732 = 0.3050$ nm

**BCC (011) 面**(等价于 (110)):
- 是一个矩形 $a \times a\sqrt{2}$(对角矩形)
- 4 角各 1/4 + 1 个体心(完整,体心**在** (011) 面上)= 1 + 1 = **2 atoms**

### 解答

面积 = $a \times a\sqrt{2} = a^2\sqrt{2} = (0.3050)^2 \times 1.414 = 0.0930 \times 1.414 = 0.1316 \text{ nm}^2$

$$\rho_{p(011)} = \frac{2}{0.1316 \text{ nm}^2} = 15.20 \text{ atoms/nm}^2$$

转 atoms/m²:
$$\rho_p = 15.20 \times 10^{18} = \boxed{1.52 \times 10^{19} \text{ atoms/m}^2} ✓$$

### 一致性验证
- 课件答案 1.522 × 10¹⁹ atoms/m²,本计算 1.52 × 10¹⁹ 一致 ✓
- BCC (110)/(011) 是 BCC 的**最密堆面**(虽然 BCC 不是 close-packed 结构,但 {110} 是 BCC 内最密的)

**易错**:
- BCC (110)/(011) 面**包含体心**(体心在矩形中央)→ 2 atoms
- 矩形面积 = $a \times a\sqrt{2}$,**不是** $a^2$(那是 (100) 面)
- 不要把 BCC (100) 算成 BCC (110):
  - BCC (100):4×1/4 = 1 atom,面积 $a^2$
  - BCC (110):4×1/4 + 1 = 2 atoms,面积 $a^2\sqrt{2}$

---

## Problem 6

> 解释 linear atomic density 和 planar atomic density,讨论它们在化工材料应用中的意义。

**涉及知识点**: 原子密度, 滑移, 催化

### 解答

### 概念

**Linear Atomic Density** $\rho_l$ — 沿某 **方向** [uvw] 单位长度内的原子直径数:
$$\rho_l = \frac{\text{atomic diameters intersected}}{\text{selected length}}$$

**Planar Atomic Density** $\rho_p$ — 某 **平面** (hkl) 内单位面积的原子中心数:
$$\rho_p = \frac{\text{atom centers in plane}}{\text{selected area}}$$

**关键**:**方向/平面不同,密度不同**。这种"各向异性"导致材料性质方向性。

### 化工材料中的 5 个应用意义

#### 1. 滑移系判定 → 决定金属延展性

- **Slip systems**(滑移系)= 密排面 + 密排方向
- FCC 的 {111}⟨110⟩(4 个密排面 × 3 个方向 = 12 个滑移系)→ 延展性最好
- BCC 的 {110}⟨111⟩、{211}⟨111⟩ 等 → 12 个但 CRSS 高
- HCP 只有 (0001)⟨11-20⟩ → 3 个 → 难塑性变形

**化工意义**:压力容器、管线选材时,FCC 比 HCP 抗冲击好(滑移系多 → 不脆断)。

#### 2. 衍射强度 → 决定 XRD 谱线

- **高 ρ_p 的面 → 强衍射峰**(更多原子参与衍射,相位叠加更强)
- 例:FCC 第一峰 (111) 面密度高 → 主峰
- 这是 XRD 物相鉴定的基础

**化工意义**:催化剂相分析(钯黑、铂黑结构鉴定),反应器表面结晶度测定。

#### 3. 表面催化活性 → 决定催化效率

- **低 ρ_p 的面通常活性高**(原子配位不饱和,更愿意键合反应物)
- 例:**Pt(111) vs Pt(100)** 对 CO 氧化活性差 10 倍以上
- **Fe(111)** 是合成氨(Haber-Bosch)的活性面

**化工意义**:催化剂设计(纳米晶面工程)、贵金属负载量优化。

#### 4. 腐蚀方向性 → 决定材料寿命

- 低 ρ_p 面(原子稀疏)→ 化学攻击容易切入 → 优先腐蚀
- 晶界(原子排列断裂区)是腐蚀首攻位置
- 多晶材料晶粒越小 → 晶界总长越多 → 抗腐蚀越差(典型反例:细晶材料抗高温蠕变好但抗腐蚀差)

**化工意义**:储罐、反应器选材的腐蚀寿命估算。

#### 5. 离子/原子扩散 → 决定渗碳/扩散反应

- 沿低 ρ_l 方向扩散更快(原子间距大,有"缝隙")
- 例:渗碳钢的 C 扩散在 γ-Fe(FCC,八面体间隙大)更快

**化工意义**:气体分离膜(择优扩散)、催化剂载体浸渍工艺。

### 总结

**ρ_l 和 ρ_p 不只是数学量,而是连接微观晶体结构和宏观工程性能(强度/腐蚀/催化/扩散)的核心桥梁。**

化工工程师选材时,看晶体结构 → 算 ρ_l, ρ_p → 推性能。

---

## 答案速查

| 题号 | 最终答案 | 涉及概念 |
|---|---|---|
| 1 | 三类(volume/linear/planar),3 因素,5 重要性 | Atomic Density |
| 2 | V BCC: ρ_[110]=2.32 / ρ_[111]=3.79 atoms/nm | BCC Linear Density |
| 3 | Cu FCC ρ_[111] = 1.595×10⁹ atoms/m | FCC Linear Density |
| 4 | Ni FCC ρ_(100) = 1.61×10¹⁹ atoms/m² | FCC Planar Density |
| 5 | V BCC ρ_(011) = 1.52×10¹⁹ atoms/m² | BCC Planar Density |
| 6 | 5 个化工意义:滑移/XRD/催化/腐蚀/扩散 | 原子密度的工程意义 |

---

## 知识盲区 / Gaps identified

> [!NOTE]
> - CRSS Critical Resolved Shear Stress — Q6 提到,L03 没详讲
> - Sabatier 原理 + d 带中心 — Q6 催化部分,L02/L03 都没讲
> - Schmid Factor 施密特因子 — 计算实际滑移所需应力时用,L03 没讲
> - 择优扩散 / Anisotropic Diffusion — Q6 提到,L03 没讲
> - **HCP 的密度计算**(本份 tutorial 全是 BCC/FCC 例子,没出 HCP 计算 — 考试可能补)
