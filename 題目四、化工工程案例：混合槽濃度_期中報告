# 題目四：化工工程案例－混合槽濃度變化  
## Midterm Report - First Order Differential Equation

---

## 1. Problem Statement  
水槽中污染物濃度如何隨時間變化？

---

## 2. Mathematical Modeling（質量守恆）

根據質量守恆（Mass Balance）：

$$
\frac{dC}{dt} = \frac{Q}{V}(C_{in} - C)
$$

Where:

- $C(t)$：槽內濃度  
- $C_{in}$：流入濃度  
- $C_0$：初始濃度  
- $Q$：流量  
- $V$：槽體體積  

---

## 3. Derivation（Separation of Variables）

### Step 1：分離變數

$$
\frac{dC}{C_{in} - C} = \frac{Q}{V} dt
$$

---

### Step 2：積分

$$
\int \frac{1}{C_{in} - C} dC = \int \frac{Q}{V} dt
$$

---

### Step 3：變數代換

令：

$$
u = C_{in} - C \Rightarrow du = -dC
$$

則：

$$
-\ln|C_{in} - C| = \frac{Q}{V}t + K
$$

---

### Step 4：解出 C(t)

$$
C_{in} - C = A e^{-\frac{Q}{V}t}
$$

$$
C(t) = C_{in} - A e^{-\frac{Q}{V}t}
$$

---

### Step 5：代入初始條件

當 $t=0$，$C(0)=C_0$：

$$
C_0 = C_{in} - A
$$

$$
A = C_{in} - C_0
$$

---

## 4. Final Solution

$$
\boxed{
C(t) = C_{in} + (C_0 - C_{in}) e^{-\frac{Q}{V}t}
}
$$

---

## 5. Engineering Significance（工程意義）

### （1）時間常數

$$
\tau = \frac{V}{Q}
$$

- 決定系統反應速度  
- $t = \tau$ → 約 63.2% 接近穩態  
- $t \approx 5\tau$ → 幾乎達穩態  

---

### （2）濃度變化特性

- 若 $C_0 > C_{in}$ → 濃度下降（稀釋）  
- 若 $C_0 < C_{in}$ → 濃度上升（累積）  
- 最終：

$$
C(t) \rightarrow C_{in}
$$

---

### （3）變化進度

| 時間 | 濃度變化 |
|------|--------|
| $1\tau$ | 63.2% |
| $3\tau$ | 95% |
| $5\tau$ | 99%以上 |

---

### （4）實際應用

- 廢水處理（污染物稀釋）  
- 連續攪拌反應器（CSTR）  
- 環境工程（水體污染分析）  

---

## 6. Summary

本題為典型一階微分方程，解為指數趨近穩態形式，廣泛應用於化工與環境工程系統分析。
