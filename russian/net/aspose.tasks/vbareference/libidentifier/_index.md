---
title: "VbaReference.LibIdentifier"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaReference. Получает идентификатор библиотеки"
type: docs
weight: 20
url: /ru/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Получает идентификатор библиотеки.

```csharp
public string LibIdentifier { get; }
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


