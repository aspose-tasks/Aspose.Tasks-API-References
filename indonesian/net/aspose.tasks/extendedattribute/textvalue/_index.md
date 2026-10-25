---
title: "ExtendedAttribute.TextValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttribute. Mendapatkan atau mengatur nilai untuk atribut dengan tipe Teks"
type: docs
weight: 80
url: /id/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

Mendapatkan atau mengatur nilai untuk atribut dengan tipe 'Text'.

```csharp
public string TextValue { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Dilempar jika properti [`AttributeDefinition`](../attributedefinition/) tidak diinisialisasi atau atribut saat ini bukan atribut teks. |

## Contoh

Menampilkan cara menambahkan atribut yang diperluas yang menggunakan formula tanggal/waktu MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Atur formula ProjDateDiff dan cetak nilai atribut yang diperluas
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

// Atur formula ProjDateSub dan cetak nilai atribut yang diperluas
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Kita dapat mengatur formula ProjDurConv ke atribut dengan nilai durasi maupun ke atribut dengan nilai teks.
// Atur formula ProjDurConv ke atribut yang diperluas dengan nilai durasi dan cetak nilainya.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Atur formula ProjDurConv ke atribut yang diperluas dengan nilai teks dan cetak nilainya.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Atur formula Second dan cetak nilai atribut yang diperluas
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Atur formula Weekday dan cetak nilai atribut yang diperluas
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Lihat Juga

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


