---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API Reference"
description: "위험 분석 결과를 나타냅니다."
type: docs
weight: 262
url: /ko/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

위험 분석 결과를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | 지정된 위험 유형에 대한 [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) 인스턴스를 반환합니다. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | 위험 분석 보고서를 PDF 형식으로 스트림에 저장합니다. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | 위험 분석 보고서를 PDF 형식으로 지정된 파일 경로에 저장합니다. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


지정된 위험 유형에 대한 [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) 인스턴스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| itemType | int | 지정된 위험 유형; [RiskItemType](../../com.aspose.tasks/riskitemtype) 열거형의 값 중 하나일 수 있습니다. |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


위험 분석 보고서를 PDF 형식으로 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 위험 분석 보고서를 저장할 스트림. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


위험 분석 보고서를 PDF 형식으로 지정된 파일 경로에 저장합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 지정된 파일 이름. |

