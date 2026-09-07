---
title: "Project.GlobalizationSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan atau mengatur pengaturan spesifik bahasa globalisasi proyek"
type: docs
weight: 460
url: /id/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Mendapatkan atau mengatur pengaturan globalisasi (spesifik bahasa) proyek.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Catatan

Cara yang disarankan adalah menggunakan literal atau format yang tidak bergantung pada budaya di seluruh proyek. Namun, jika sebuah proyek menggunakan literal yang spesifik budaya, kelas ini dapat digunakan untuk membantu mesin perhitungan mengurai literal tersebut.

## Contoh

Menampilkan cara mengatur pengaturan bahasa khusus proyek.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Buat atribut tambahan
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Lihat Juga

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


