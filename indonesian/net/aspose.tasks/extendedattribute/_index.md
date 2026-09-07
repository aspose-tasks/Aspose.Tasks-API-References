---
title: "Kelas ExtendedAttribute"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ExtendedAttribute. Mewakili atribut tambahan"
type: docs
weight: 520
url: /id/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Mewakili atribut yang diperluas.

```csharp
public class ExtendedAttribute
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Mendapatkan definisi atribut. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Mendapatkan atau mengatur nilai untuk atribut dengan tipe tanggal (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Mendapatkan atau mengatur nilai untuk atribut dengan tipe 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Mendapatkan id dari sebuah bidang. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah flag diatur untuk atribut dengan tipe 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Mendapatkan apakah perhitungan nilai atribut ekstended menghasilkan kesalahan. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Mendapatkan atau mengatur nilai untuk atribut dengan tipe numerik (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Mendapatkan atau mengatur nilai untuk atribut dengan tipe 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Mendapatkan guid dari nilai lookup. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah nilai dari instance `ExtendedAttribute` ini bersifat read-only. Mengembalikan true jika sebuah formula atau rollup didefinisikan dalam [`ExtendedAttributeDefinition`](../extendedattributedefinition/) untuk objek ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Mengembalikan representasi string singkat dari sebuah atribut ekstended. |

## Catatan

Saat ini mendukung semua tipe atribut Extended yang dibaca dari MSP Xml 2003/2007 dan mpp 2003. Untuk MSP mpp 2007 semua pembacaan atribut Extended didukung kecuali durasi dan flag.

## Contoh

Menampilkan cara menambahkan field khusus yang nilainya dihitung menggunakan formula yang ditentukan oleh pengguna.

```csharp
var project = new Project();

// buat definisi atribut ekstended tugas baru
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Tambahkan formula ke atribut.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Buat atribut tambahan
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Kami mengatur Formula untuk atribut ekstended, sehingga bersifat read only (nilai dihitung menggunakan formula).
// Output adalah "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Anda dapat mencoba mengatur nilai field read only, tetapi tidak akan berpengaruh.
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

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


