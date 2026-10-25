---
title: "Asn.NotesText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Текст заметок в простом виде, извлечённый из данных RTF."
type: docs
weight: 350
url: /ru/net/aspose.tasks/asn/notestext/
---
## Asn.NotesText field

Обычный текст заметок, извлечённый из данных RTF.

```csharp
public static readonly Key<string, AsnKey> NotesText;
```

## Примеры

Показывает, как получать/устанавливать заметки назначения ресурса.

```csharp
var project = new Project(DataDir + "UpdateResourceAssignment.mpp");
var task = project.RootTask.Children.GetById(1);
var rsc = project.Resources.GetById(1);

// создать назначение ресурса
var assn = project.ResourceAssignments.Add(task, rsc);

// установить заметки назначения ресурса
assn.Set(Asn.NotesText, "Newly added assignment");

Console.WriteLine("Notes text: " + assn.Get(Asn.NotesText));
Console.WriteLine("Notes RTF: " + assn.Get(Asn.NotesRTF));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


