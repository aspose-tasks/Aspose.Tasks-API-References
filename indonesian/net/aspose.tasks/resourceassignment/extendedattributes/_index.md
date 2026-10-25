---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceAssignment. Mendapatkan atau mengatur sebuah instance dari kelas ExtendedAttributeCollection untuk objek ini"
type: docs
weight: 250
url: /id/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Mendapatkan atau mengatur instance kelas ExtendedAttributeCollection untuk objek ini.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Catatan

Pembacaan hanya didukung untuk format XML.

## Contoh

Menampilkan cara menambahkan atribut ekstensi untuk sebuah penugasan.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Tetapkan sumber daya "1 TRG: Trade Group" ke "TASK 1" dengan membuat objek ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Buat definisi atribut kustom dengan pencarian.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Nilai ini dapat dilihat di tampilan "Resource usage" pada MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Lihat Juga

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


