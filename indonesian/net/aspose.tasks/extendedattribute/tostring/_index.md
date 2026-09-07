---
title: "ExtendedAttribute.ToString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttribute. Mengembalikan representasi string singkat dari atribut extended"
type: docs
weight: 110
url: /id/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Mengembalikan representasi string singkat dari sebuah atribut ekstended.

```csharp
public override string ToString()
```

### Nilai Kembali

Representasi string dari atribut extended.

## Contoh

Menampilkan cara membaca atribut extended.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Baca atribut ekstended untuk tugas
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // membaca info umum tentang atribut extended
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Lihat Juga

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


