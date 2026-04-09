# PBPK模型中肝脏代谢酶机制与微分方程

## 一、基本概念

在PBPK模型中，肝脏代谢酶（如CYP450、UGT等）的作用可以统一表示为：

> **内在清除率（CLint）**

它代表在没有血流限制时，肝脏本身的代谢能力。

---

## 二、生理过程

肝脏代谢过程可以分为三个步骤：

1. 血流进入肝脏（QH）
2. 药物进入肝细胞（受fu、转运影响）
3. 被酶代谢（CLint 或 Vmax/Km）

---

## 三、代谢动力学表达

### 1. 线性代谢

v = CLint × C_hep

---

### 2. 非线性（Michaelis-Menten）

v = Vmax × C_hep / (Km + C_hep)

---

## 四、PBPK肝脏微分方程

### 1. 基本形式

肝脏药量变化：

 dA_liver/dt = QH × (Cin - Cout) - v_met

---

### 2. 展开形式（线性代谢）

 dA_liver/dt = QH × (Cin - C_liver/Kp) - fu × CLint × C_liver

---

### 3. 非线性代谢形式

 dA_liver/dt = QH × (Cin - C_liver/Kp) - (Vmax × fu × C_liver)/(Km + fu × C_liver)

---

## 五、关键参数说明

| 参数 | 含义 |
|------|------|
| QH | 肝血流量 |
| CLint | 内在清除率 |
| fu | 游离分数 |
| Kp | 组织分配系数 |
| Vmax | 最大代谢速率 |
| Km | 米氏常数 |

---

## 六、fu的重要性

只有游离药物参与代谢：

 C_free = fu × C_total

---

## 七、IVIVE放大

体外到体内转换：

 CLint_in vivo = CLint_in vitro × MPPGL × Liver weight

---

## 八、与经典肝清除率关系

 CLH = QH × fu × CLint / (QH + fu × CLint)

该公式是PBPK模型在稳态下的解析形式。

---

## 九、进阶模型

### 1. Permeability-limited模型

 dA_hep/dt = PS × (C_blood - C_cell) - CLint × C_cell

---

### 2. 加入转运体

 Uptake: v = PS_active × C_blood

 Efflux: v = PS_efflux × C_cell

---

## 十、总结

PBPK中肝酶的数学本质：

> **肝脏变化 = 血流输入 - 血流输出 - 酶代谢**

核心参数：CLint + fu + QH

---

## 十一、应用建议（ADC/PBPK）

- 小分子payload：建议使用 permeability-limited + CLint
- ADC本体：需考虑内吞 + 溶酶体释放 + 非线性

---

（完）

