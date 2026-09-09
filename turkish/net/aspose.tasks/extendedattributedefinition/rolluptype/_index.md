---
title: "ExtendedAttributeDefinition.RollupType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinition özelliği. Toplamların nasıl hesaplandığını alır veya ayarlar."
type: docs
weight: 230
url: /tr/net/aspose.tasks/extendedattributedefinition/rolluptype/
---
## ExtendedAttributeDefinition.RollupType property

Toplamların nasıl hesaplandığını alır veya ayarlar.

```csharp
public RollupType RollupType { get; set; }
```

## Açıklamalar

Yazma şu anda yalnızca Xml formatı için desteklenmektedir.

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

* enum [RollupType](../../rolluptype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


