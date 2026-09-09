---
title: "ExtendedAttribute.DateValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttribute özelliği. Tarih türleri (Date, Start, Finish) olan öznitelikler için bir değer alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

Tarih türündeki (Date, Start, Finish) öznitelikler için bir değeri alır veya ayarlar.

```csharp
public DateTime DateValue { get; set; }
```

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | [`AttributeDefinition`](../attributedefinition/) özelliği başlatılmamışsa veya mevcut öznitelik bir tarih özniteliği değilse fırlatılır. |

## Örnekler

Genişletilmiş özniteliğin öznitelik tanımını nasıl değiştireceğinizi gösterir.

```csharp
var project = new Project();

// yeni görev genişletilmiş öznitelik tanımı oluştur
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// Özniteliğe bir formül ekle.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// Genişletilmiş öznitelik oluştur
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// yeni bir tarih genişletilmiş öznitelik tanımı oluştur
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// Özniteliğe bir formül ekle.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


