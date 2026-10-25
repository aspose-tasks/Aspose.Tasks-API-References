---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Projenin küreselleşme diline özgü ayarlarını alır veya ayarlar"
type: docs
weight: 460
url: /tr/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Projenin küreselleştirme (dile özgü) ayarlarını alır veya ayarlar.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Açıklamalar

Önerilen yöntem, proje boyunca kültüre bağımlı olmayan sabit değerler veya biçimler kullanmaktır. Ancak, bir proje kültüre özgü sabit değerler kullanıyorsa, bu sınıf bu sabit değerlerin hesaplama motoru tarafından ayrıştırılmasına yardımcı olmak için kullanılabilir.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


