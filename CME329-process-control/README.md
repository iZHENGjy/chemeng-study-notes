---
type: course-moc
course: CME329
title_en: Process Control and Instrumentation
title_zh: 化工过程控制
semester: 2026-Fall
tags:
  - 化工
  - 化工过程控制
  - 课程笔记
  - 主笔记
  - MOC
last_updated: 2026-10-19
---

# 📘 **CME329 · 化工过程控制** · 主笔记

> Process Control and Instrumentation · 用反馈与动态模型让化工过程稳定运行在设定值
> 讲师：
> 教材：Seborg, Edgar, Mellichamp & Doyle, *Process Dynamics and Control*

> [!NOTE]
> **关于这份笔记**
> 整门课的**主索引（MOC）**。上课期间按周追加；结课后升级成完整版（知识地图 + 决策树）。
> 课件文件名沿用旧课号 CME209，tutorial 用新课号 CME329，二者是同一门课。

## 按周索引

<!-- ingest-lecture 每次处理完一节课，在这行下面追加一个 Week 段 -->

## Week 1

过程控制导论：控制回路四要素（Process / Sensor / Controller / FCE），CV / MV / DV 分类，用搅拌混合槽对比反馈（FB）与前馈（FF）控制，精馏塔四步设计法，控制层级与 APC 的经济效益。

- [L01_intro_to_process_control](L01_intro_to_process_control.md)

**本周疑问**:
- 比例控制律 $w_2 = \bar w_2 + K_c(x_{SP} - x)$ 能否消除稳态偏差？
- 精馏塔 5 个变送器与 5 个阀如何配对？

## Week 2

Laplace 变换：定义、常用变换表、解 ODE 与部分分式、FVT/IVT、时滞；传递函数的定义与性质（增益、阶数、可实现性、加法/乘法）；用偏差变量由搅拌加热槽推出 $K/(\tau s+1)$；非线性模型的两种线性化方法（液位储罐）。

- [L02_laplace_transform_and_transfer_function](L02_laplace_transform_and_transfer_function.md)

**本周疑问**:
- 复根、重根情况下的部分分式怎么做？
- 线性化模型在离操作点多远仍然可信？

## Week 3

一阶、二阶与复杂过程的动态响应：标准输入信号，一阶阶跃/斜坡响应（63.2% @ τ），积分过程，二阶三种阻尼与性能指标，零极点对响应的影响（超调、反向响应），时滞 $e^{-\theta s}$ 与 Skogestad 半数规则 FOPTD 近似。

- [L03_first_second_order_dynamic_response](L03_first_second_order_dynamic_response.md)

**本周疑问**:
- 调节时间按 ±5% 还是 ±2%？
- 何时 FOPTD 不够用、要改 SOPTD？
