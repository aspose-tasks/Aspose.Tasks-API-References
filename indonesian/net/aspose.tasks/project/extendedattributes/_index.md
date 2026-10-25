---
title: "Project.ExtendedAttributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan objek ExtendedAttributeDefinitionCollection. Kumpulan definisi bidang khusus atribut ekstensi yang terkait dengan sebuah proyek"
type: docs
weight: 410
url: /id/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Mendapatkan objek ExtendedAttributeDefinitionCollection. Koleksi definisi atribut tambahan (field khusus) yang terkait dengan sebuah proyek.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Contoh

Menampilkan cara bekerja dengan atribut ekstensi.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Jika bidang Kustom tidak ada dalam Proyek, buatlah.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Hasilkan Atribut Ekstensi dari definisi
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Tambahkan atribut ekstensi ke tugas
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


