---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示风险分析的结果。"
type: docs
weight: 262
url: /zh/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

表示风险分析的结果。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | 返回针对指定风险类型的 [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) 实例。 |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | 以 PDF 格式将风险分析报告保存到流中。 |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | 以 PDF 格式将风险分析报告保存到指定的文件路径。 |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


返回针对指定风险类型的 [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| itemType | int | 指定的风险类型；可以是 [RiskItemType](../../com.aspose.tasks/riskitemtype) 枚举的其中一个值。 |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


以 PDF 格式将风险分析报告保存到流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 用于保存风险分析报告的流。 |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


以 PDF 格式将风险分析报告保存到指定的文件路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 指定的文件名。 |

