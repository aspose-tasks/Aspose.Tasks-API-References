---
title: "RiskAnalysisSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定执行风险分析的设置。"
type: docs
weight: 263
url: /zh/java/com.aspose.tasks/riskanalysissettings/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisSettings
```

指定执行风险分析的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RiskAnalysisSettings()](#RiskAnalysisSettings--) | 初始化 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getIterationsCount()](#getIterationsCount--) | 获取在 Monte Carlo 仿真中使用的迭代次数。 |
| [getPatterns()](#getPatterns--) | 获取包含 [RiskPattern](../../com.aspose.tasks/riskpattern) 类实例的集合。 |
| [setIterationsCount(int value)](#setIterationsCount-int-) | 设置在 Monte Carlo 仿真中使用的迭代次数。 |
### RiskAnalysisSettings() {#RiskAnalysisSettings--}
```
public RiskAnalysisSettings()
```


初始化 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的新实例。

### getIterationsCount() {#getIterationsCount--}
```
public final int getIterationsCount()
```


获取在 Monte Carlo 仿真中使用的迭代次数。默认值为 100。

**Returns:**
int - 在 Monte Carlo 仿真中使用的迭代次数。
### getPatterns() {#getPatterns--}
```
public final RiskPatternCollection getPatterns()
```


获取包含 [RiskPattern](../../com.aspose.tasks/riskpattern) 类实例的集合。

**Returns:**
[RiskPatternCollection](../../com.aspose.tasks/riskpatterncollection) - a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.
### setIterationsCount(int value) {#setIterationsCount-int-}
```
public final void setIterationsCount(int value)
```


设置在 Monte Carlo 仿真中使用的迭代次数。默认值为 100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在蒙特卡罗模拟中使用的迭代次数。 |

