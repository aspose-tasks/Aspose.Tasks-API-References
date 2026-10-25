---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "リスク分析の結果を表します。"
type: docs
weight: 262
url: /ja/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

リスク分析の結果を表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | 指定されたリスクタイプに対する [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) のインスタンスを返します。 |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | リスク分析レポートを PDF 形式でストリームに保存します。 |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | リスク分析レポートを PDF 形式で指定されたファイルパスに保存します。 |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


指定されたリスクタイプに対する [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) のインスタンスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| itemType | int | 指定されたリスクタイプ; [RiskItemType](../../com.aspose.tasks/riskitemtype) 列挙体の値のいずれかにすることができます。 |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


リスク分析レポートを PDF 形式でストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | リスク分析レポートを保存するストリーム。 |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


リスク分析レポートを PDF 形式で指定されたファイルパスに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fileName | java.lang.String | 指定されたファイル名。 |

