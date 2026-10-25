---
title: "Class GlobalizationSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.GlobalizationSettings class. Mewakili pengaturan globalisasi proyek."
type: docs
weight: 720
url: /id/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Mewakili pengaturan globalisasi proyek.

```csharp
public class GlobalizationSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Mendapatkan string untuk literal boolean 'false' yang digunakan dalam formula. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Mendapatkan literal "NA" (nilai kosong) yang digunakan dalam formula untuk bidang tanggal. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Mendapatkan string untuk literal boolean 'true' yang digunakan dalam sebuah rumus. |

## Catatan

Cara yang disarankan adalah menggunakan literal atau format yang tidak bergantung pada budaya di seluruh proyek. Namun, jika sebuah proyek menggunakan literal yang spesifik budaya, kelas ini dapat digunakan untuk membantu mesin perhitungan formula mengurai literal tersebut.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


