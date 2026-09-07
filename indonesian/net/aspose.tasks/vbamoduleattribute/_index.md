---
title: "Class VbaModuleAttribute"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.VbaModuleAttribute. Atribut dari objek VbaModule"
type: docs
weight: 2820
url: /id/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

Atribut dari objek [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Mendapatkan kunci atribut modul VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Mendapatkan nilai atribut modul VBA. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `VbaModuleAttribute` yang ditentukan. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `VbaModuleAttribute` yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Mengembalikan nilai kode hash untuk `VbaModuleAttribute` ini. |

## Contoh

Menampilkan cara bekerja dengan atribut modul VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


