---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttribute. Mendapatkan apakah perhitungan nilai atribut yang diperluas menghasilkan kesalahan"
type: docs
weight: 60
url: /id/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Mendapatkan apakah perhitungan nilai atribut ekstended menghasilkan kesalahan.

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


