---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttribute özelliği. Metin tipindeki öznitelikler için bir değer alır veya ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

'Text' türündeki öznitelikler için değeri alır veya ayarlar.

```csharp
public string TextValue { get; set; }
```

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Eğer [`AttributeDefinition`](../attributedefinition/) özelliği başlatılmamışsa veya geçerli öznitelik bir metin özniteliği değilse fırlatılır. |

## Örnekler

MS Project tarih/saat formüllerini kullanan genişletilmiş özniteliklerin nasıl ekleneceğini gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// ProjDateDiff formülünü ayarlayın ve genişletilmiş öznitelik değerini yazdırın
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// ProjDateSub formülünü ayarlayın ve genişletilmiş öznitelik değerini yazdırın
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// ProjDurConv formülünü hem süre değerli özniteliklere hem de metin değerli özniteliklere ayarlayabiliriz.
// ProjDurConv formülünü süre değerli genişletilmiş özniteliğe ayarlayın ve değerini yazdırın.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// ProjDurConv formülünü metin değerli genişletilmiş özniteliğe ayarlayın ve değerini yazdırın.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Second formülünü ayarlayın ve genişletilmiş öznitelik değerini yazdırın.
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Weekday formülünü ayarlayın ve genişletilmiş öznitelik değerini yazdırın
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


