---
title: "VbaProject.References"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaProject. Возвращает коллекцию VbaReferenceCollection."
type: docs
weight: 70
url: /ru/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Возвращает коллекцию [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Примеры

Показывает, как читать информацию о ссылках проекта VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### См. также

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


