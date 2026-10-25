---
title: "ExtendedAttribute.NumericValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttribute özelliği. Sayısal tipteki öznitelikler için bir değer alır veya ayarlar (Cost Number)"
type: docs
weight: 70
url: /tr/net/aspose.tasks/extendedattribute/numericvalue/
---
## ExtendedAttribute.NumericValue property

Sayısal türdeki (Cost, Number) öznitelikler için değeri alır veya ayarlar.

```csharp
public decimal NumericValue { get; set; }
```

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Eğer [`AttributeDefinition`](../attributedefinition/) özelliği başlatılmamışsa veya [`AttributeDefinition`](../attributedefinition/) özelliğinin özel alan türü 'Cost' ya da 'Number' değilse fırlatılır. |

## Örnekler

Kullanıcı tarafından belirtilen formül kullanılarak değeri hesaplanan özel alanın nasıl ekleneceğini gösterir.

```csharp
var project = new Project();

// yeni görev genişletilmiş öznitelik tanımı oluştur
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Özniteliğe bir formül ekle.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Genişletilmiş öznitelik oluştur
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Genişletilmiş öznitelik için Formülü ayarladık, böylece yalnızca okunur (değer formül kullanılarak hesaplanır).
// Çıktı "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Yalnızca okunur alanın değerini ayarlamayı deneyebilirsiniz, ancak bir etkisi olmayacaktır.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


