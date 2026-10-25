---
title: "Enum CalculationType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalculationType enum. Özel öznitelik değerinin hesaplamasının türünü belirtir"
type: docs
weight: 220
url: /tr/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Özel öznitelik değerinin hesaplama tipini belirtir.

```csharp
public enum CalculationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Anlamı, genişletilmiş öznitelik için formül arama tablosu olmadığını ve yalnızca kullanıcı tarafından ayarlanan değeri depoladığını gösterir. |
| Lookup | `1` | Anlamı, genişletilmiş öznitelik değerinin bir arama tablosundaki değerlerle sınırlı olduğudur. |
| Formula | `2` | Anlamı, genişletilmiş öznitelik değerinin [`Formula`](../extendedattributedefinition/formula/) içinde tanımlanan formül kullanılarak hesaplandığıdır. |

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


