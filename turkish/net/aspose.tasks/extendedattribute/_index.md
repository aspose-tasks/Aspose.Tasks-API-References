---
title: "Sınıf ExtendedAttribute"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ExtendedAttribute sınıfı. Genişletilmiş öznitelikleri temsil eder"
type: docs
weight: 520
url: /tr/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Genişletilmiş öznitelikleri temsil eder.

```csharp
public class ExtendedAttribute
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Öznitelik tanımını alır. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Tarih türündeki (Date, Start, Finish) öznitelikler için bir değeri alır veya ayarlar. |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | 'Duration' türündeki öznitelikler için değeri alır veya ayarlar. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Bir alanın kimliğini alır. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | 'Flag' türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren değeri alır veya ayarlar. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Genişletilmiş öznitelik değerinin hesaplamasının bir hatayla sonuçlanıp sonuçlanmadığını alır. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Sayısal türdeki (Cost, Number) öznitelikler için değeri alır veya ayarlar. |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | 'Text' türündeki öznitelikler için değeri alır veya ayarlar. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Bir arama değerinin guid'ini alır. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Bu `ExtendedAttribute` örneğinin bir değerinin yalnızca okunur olup olmadığını gösteren bir değeri alır. Bu nesne için [`ExtendedAttributeDefinition`](../extendedattributedefinition/) içinde bir formül veya toplama tanımlıysa true döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Bir genişletilmiş özniteliğin kısa dize temsilini döndürür. |

## Açıklamalar

Şu anda MSP Xml 2003/2007 ve mpp 2003'ten okunan tüm Genişletilmiş öznitelik türleri desteklenmektedir. MSP mpp 2007 için, süreler ve bayraklar dışındaki tüm Genişletilmiş öznitelik okuması desteklenir.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


