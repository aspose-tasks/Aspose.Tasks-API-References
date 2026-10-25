---
title: "Sınıf EntityFieldAttribute"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute sınıfı. Varlık özellikleri için bir özniteliği temsil eder"
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

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Varsayılan yapıcı. |

## Açıklamalar

[`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) ve [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) varlık özellikleri için yalnızca kullanılan bir öznitelik ve bunların sayımını basitleştirir.

## Örnekler

**EntityField** özniteliği kullanarak özellikleri nasıl sayımlarsınız:

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


