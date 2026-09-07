---
title: "Resource.ExtendedAttributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan nilai-nilai atribut ekstensi"
type: docs
weight: 320
url: /id/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Mendapatkan nilai-nilai atribut yang diperluas.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Catatan

Dua potongan data diperlukan - sebuah penunjuk kembali ke tabel atribut ekstensi yang ditentukan baik dengan ID unik atau Field ID, dan nilai yang ditentukan baik dengan nilai itu sendiri, atau penunjuk kembali ke daftar nilai.

## Contoh

Menampilkan cara menambahkan atribut ekstensi resource.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Definisikan atribut ekstensi
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Buat atribut ekstensi dan atur nilainya
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Tambahkan resource baru dan atribut ekstensinya
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


