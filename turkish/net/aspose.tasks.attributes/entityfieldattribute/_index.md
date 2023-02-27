---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Attributes.EntityFieldAttribute sınıf. Varlık özellikleri için bir özniteliği temsil eder.
type: docs
weight: 70
url: /tr/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Varlık özellikleri için bir özniteliği temsil eder.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Constructor |

### Notlar

için kullanılan öznitelik[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) ve[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) yalnızca varlık özellikleri ve numaralandırmasını basitleştirir.

### Örnekler

Kullanarak özellikler nasıl numaralandırılır? **varlık alanı** öznitelik:

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

### Ayrıca bakınız

* ad alanı [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* toplantı [Aspose.Tasks](../../)


