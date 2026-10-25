---
title: "Заметки"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Текстовые заметки, связанные с назначением."
type: docs
weight: 350
url: /ru/net/aspose.tasks/asn/notes/
---
## Asn.Notes field

Текстовые заметки, связанные с назначением.

```csharp
public static readonly Key<string, AsnKey> Notes;
```

### Примеры

Показывает, как получать/устанавливать заметки назначения ресурса.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// создать назначение ресурса
var assn = project.ResourceAssignments.Add(task, rsc);

// установить заметки назначения ресурса
assn.Set(Asn.Notes, "Newly added assignment");

Console.WriteLine("Notes: " + assn.Get(Asn.Notes));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [AsnKey](../../asnkey)
* class [Asn](../../asn)
* namespace [Aspose.Tasks](../../asn)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
