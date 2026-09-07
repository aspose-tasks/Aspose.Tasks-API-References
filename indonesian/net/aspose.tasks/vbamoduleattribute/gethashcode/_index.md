---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode VbaModuleAttribute. Mengembalikan nilai kode hash untuk VbaModuleAttribute ini."
type: docs
weight: 40
url: /id/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Mengembalikan nilai kode hash untuk [`VbaModuleAttribute`](../) ini.

```csharp
public override int GetHashCode()
```

### Nilai Kembali

Mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah atribut modul VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// cetak kode hash dari atribut modul VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Lihat Juga

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


