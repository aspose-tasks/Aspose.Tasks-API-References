---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Mengembalikan sebuah flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan"
type: docs
weight: 320
url: /id/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | objek yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

sebuah flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

## Contoh

Menampilkan cara memeriksa kesetaraan definisi atribut ekstensi.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// kesetaraan kalender diperiksa terhadap id bidang definisi atribut.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Lihat Juga

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


