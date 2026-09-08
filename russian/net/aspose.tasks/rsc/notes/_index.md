---
title: "Заметки"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Текстовые заметки, связанные с ресурсом."
type: docs
weight: 470
url: /ru/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

Текстовые заметки, связанные с ресурсом.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### Примеры

Показывает, как читать/записывать свойство Rsc.Notes.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
