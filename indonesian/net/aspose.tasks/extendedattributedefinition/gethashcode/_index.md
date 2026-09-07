---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Mengembalikan kode hash untuk instance kelas ExtendedAttributeDefinition."
type: docs
weight: 330
url: /id/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Mengembalikan kode hash untuk instance kelas [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

sebuah kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah definisi atribut ekstensi.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// kode hash dari sebuah definisi atribut ekstensi sama dengan sebuah id bidang.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Lihat Juga

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


