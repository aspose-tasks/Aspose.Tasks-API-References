---
title: "Kelas EntityFieldAttribute"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute class. Mewakili atribut untuk properti entitas."
type: docs
weight: 70
url: /id/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Mewakili atribut untuk properti entitas.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Konstruktor default. |

## Catatan

Atribut yang digunakan hanya untuk properti entitas [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) dan [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), dan menyederhanakan enumerasinya.

## Contoh

Cara mengenumerasi properti menggunakan atribut **EntityField**:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### Lihat Juga

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


