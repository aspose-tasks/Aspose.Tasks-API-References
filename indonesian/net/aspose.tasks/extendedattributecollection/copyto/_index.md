---
title: "ExtendedAttributeCollection.CopyTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ExtendedAttributeCollection. Menyalin elemen koleksi ini ke array yang ditentukan mulai dari indeks array yang ditentukan"
type: docs
weight: 70
url: /id/net/aspose.tasks/extendedattributecollection/copyto/
---
## ExtendedAttributeCollection.CopyTo method

Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan.

```csharp
public void CopyTo(ExtendedAttribute[] array, int arrayIndex)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | ExtendedAttribute[] | array satu dimensi yang ditentukan untuk menyalin elemen ke |
| arrayIndex | Int32 | indeks berbasis nol dari array yang ditentukan di mana penyalinan dimulai. |

## Contoh

Menampilkan cara menggunakan koleksi atribut ekstended.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Dapatkan tugas indeks nol
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // hapus atribut ekstended
    task.ExtendedAttributes.Clear();
}

// buat definisi atribut ekstended untuk sebuah tugas
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Tambahkan atribut ekstended 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Tambahkan atribut ekstended 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// bekerja dengan atribut ekstended...

// hapus atribut ekstended berdasarkan indeks
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// gunakan akses indeks koleksi
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// salin atribut ke proyek lain
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// hapus semua definisi atribut ekstended
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Lihat Juga

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


