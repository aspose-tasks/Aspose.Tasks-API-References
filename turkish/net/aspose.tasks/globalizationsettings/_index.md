---
title: "GlobalizationSettings sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GlobalizationSettings sınıfı. Projelerin küreselleştirme ayarlarını temsil eder."
type: docs
weight: 720
url: /tr/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Projenin küreselleştirme ayarlarını temsil eder.

```csharp
public class GlobalizationSettings
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Formülde kullanılan boolean 'false' literalı için bir dize alır. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Tarih alanı için formülde kullanılan "NA" (boş değer) literalını alır. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Formülde kullanılan boolean 'true' literalı için bir dize alır. |

## Açıklamalar

Önerilen yöntem, proje boyunca kültürden bağımsız literal ve biçimler kullanmaktır. Ancak, bir proje kültüre özgü literal kullanıyorsa, bu sınıf bu literaların formül‑hesaplama motoru tarafından ayrıştırılmasına yardımcı olmak için kullanılabilir.

## Örnekler

Projenin dil‑spesifik ayarlarının nasıl ayarlandığını gösterir.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Genişletilmiş öznitelik oluştur
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


