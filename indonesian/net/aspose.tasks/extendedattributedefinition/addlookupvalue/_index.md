---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeDefinition. Menambahkan nilai ke daftar lookup internal. Ini adalah cara yang disarankan untuk manipulasi dengan ValueList"
type: docs
weight: 300
url: /id/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Menambahkan nilai ke daftar lookup internal. Ini adalah cara yang disarankan untuk manipulasi dengan [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | Nilai | Nilai yang akan ditambahkan ke lookup. |

## Catatan

Metode ini hanya berfungsi untuk instance [`ExtendedAttributeDefinition`](../) yang memiliki [`CalculationType`](../calculationtype/) sama dengan Lookup.

## Contoh

Gunakan kode ini untuk menambahkan Nilai baru ke daftar lookup:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

Menampilkan cara menambahkan atribut tambahan dengan pencarian untuk penugasan.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Tetapkan sumber daya "1 TRG: Trade Group" ke "TASK 1" dengan membuat objek ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Buat definisi atribut kustom dengan pencarian.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Nilai ini dapat dilihat di tampilan "Resource usage" pada MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Buat definisi atribut kustom dengan pencarian.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Nilai ini dapat dilihat di tampilan "Task usage" pada MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// nilai yang salah dapat dihapus nanti
taskCostAttr.RemoveLookupValue(taskWrongValue);

// bekerja dengan proyek...
```

### Lihat Juga

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


