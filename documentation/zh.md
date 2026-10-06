<!-- ELUCENIA technical documentation · anion-gap · zh · no clinical/professional/rights approval -->

# 阴离子间隙（校正值与 delta-delta）

[条件、来源与许可](https://elucenia.org/zh/tools/anion-gap)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 钠

`na`

mEq/L · 范围: 100–180

### 氯离子

`cl`

mEq/L · 范围: 60–140

### 碳酸氢根

`hco3`

mEq/L · 范围: 2–50

### 白蛋白

`alb`

g/dL · 选填 · 范围: 0.5–6

## 方法版本

AG不含K+；Figge 1998校正2.5×(4−白蛋白)；ΔAG基准12/ΔHCO₃基准24

## 已记录的公式

阴离子间隙 = Na⁺ − (Cl⁻ + HCO₃⁻).

白蛋白校正值 = AG + 2.5 × (4.0 − 白蛋白（g/dL）).

Δ比值 = (AG − 12) ÷ (24 − HCO₃⁻).

## 限制与适用人群

阴离子间隙的参考值取决于实验室方法，且存在个体差异。异常值不能确定唯一病因，也可能反映实验室误差。不得仅凭ΔAG/ΔHCO3比值判断混合性酸碱紊乱；还需要临床和实验室资料。计算中采用的白蛋白校正与参考值，需要核对相应变体的来源。

## 参考文献

- [Kraut JA, Madias NE. Serum anion gap: its uses and limitations in clinical medicine. Clin J Am Soc Nephrol, 2007.](https://doi.org/10.2215/CJN.03020906)

- [Figge J, Jabor A, Kazda A, Fencl V. Anion gap and hypoalbuminemia. Crit Care Med, 1998.](https://doi.org/10.1097/00003246-199811000-00019)

- [Rastegar A. Use of the ΔAG/ΔHCO3− ratio in the diagnosis of mixed acid-base disorders. J Am Soc Nephrol, 2007.](https://doi.org/10.1681/ASN.2006121408)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

阴离子间隙正常


### 2

阴离子间隙正常：如果存在代谢性酸中毒，则为高氯性


### 3

阴离子间隙升高：由未测定胆阴离子（乳酸、酮体、尿毒症、毒物）引起的代谢性酸中毒

| 结果详情 | |
| --- | --- |
| 经白蛋白校正的阴离子间隙 | 30.0 mEq/L |
| Delta 比值（ΔAG/ΔHCO₃⁻） | 1.29：单纯高 AG 酸中毒 |


### 4

阴离子间隙升高：由未测定胆阴离子（乳酸、酮体、尿毒症、毒物）引起的代谢性酸中毒

| 结果详情 | |
| --- | --- |
| 经白蛋白校正的阴离子间隙 | 17.0 mEq/L |
| Delta 比值（ΔAG/ΔHCO₃⁻） | 0.83：高 AG 酸中毒合并正常 AG 酸中毒 |


### 5

阴离子间隙升高：由未测定胆阴离子（乳酸、酮体、尿毒症、毒物）引起的代谢性酸中毒

| 结果详情 | |
| --- | --- |
| Delta 比值（ΔAG/ΔHCO₃⁻） | 4.50：高 AG 酸中毒合并代谢性碱中毒（或代偿性慢性呼吸性酸中毒） |

