---
title: "Enum SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.SummaryRowsCalculationType enum. Özet satırları için özel öznitelik değerinin hesaplama türünü belirtir."
type: docs
weight: 2310
url: /tr/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Özet satırlar için özel öznitelik değerinin hesaplama türünü belirtir.

```csharp
public enum SummaryRowsCalculationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Özet satırları için özel öznitelik değerinin hesaplanmadığını ifade eder. |
| Rollup | `1` | Özet satırları için özel öznitelik değerinin, [`RollupType`](../extendedattributedefinition/rolluptype/) içinde tanımlı toplama işlevi kullanılarak hesaplandığını ifade eder. |
| UseFormula | `2` | Özet satırları için özel öznitelik değerinin, [`Formula`](../extendedattributedefinition/formula/) içinde tanımlı formül kullanılarak hesaplandığını ifade eder. |

## Örnekler

Genişletilmiş öznitelik tanımının hesaplama tipiyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 'Formula' tipinde, yaprak görevler ve özet görevler için değerlerin formül kullanılarak hesaplandığı bir öznitelik tanımı oluştur.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// 'Average' rollup tipini kullanarak özet görevler için değerlerin hesaplandığı bir öznitelik tanımı oluştur.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


