---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition özelliği. Özet satırları için özel öznitelik değerinin hesaplama türünü alır veya ayarlar"
type: docs
weight: 260
url: /tr/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Özet satırlar için özel öznitelik değerinin hesaplama türünü alır veya ayarlar.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


