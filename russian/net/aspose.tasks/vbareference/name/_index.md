---
title: "VbaReference.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaReference. Получает или задает имя VBA‑ссылки"
type: docs
weight: 30
url: /ru/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Получает или задает имя VBA‑ссылки.

```csharp
public string Name { get; set; }
```

## Примеры

Показывает, как читать VBA‑ссылки.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


