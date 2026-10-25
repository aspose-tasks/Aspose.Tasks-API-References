---
title: "RollupType enum"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RollupType enum. Toplama rollup tipini belirtir"
type: docs
weight: 1950
url: /tr/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Toplama (rollup) türünü belirtir.

```csharp
public enum RollupType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Null | `0` | Null rollup tipini gösterir. |
| Maximum | `1` | Maksimum rollup tipini gösterir. |
| Minimum | `2` | Minimum rollup tipini gösterir. |
| Count | `3` | Count rollup tipini gösterir. |
| Sum | `4` | Toplam rollup tipini gösterir. |
| Average | `5` | Ortalama rollup tipini gösterir. |
| AverageFirstSublevel | `6` | Ortalama İlk Alt Seviye rollup tipini gösterir. |
| CountFirstSublevel | `7` | Sayım İlk Alt Seviye rollup tipini gösterir. |
| CountNonsummaries | `8` | Sayım Özet Olmayanlar rollup tipini gösterir. |

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


