---
title: "Rsc.NotesText"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Текст заметок в простом виде, извлечённый из данных RTF"
type: docs
weight: 480
url: /ru/net/aspose.tasks/rsc/notestext/
---
## Rsc.NotesText field

Обычный текст заметок, извлечённый из данных RTF.

```csharp
public static readonly Key<string, RscKey> NotesText;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.NotesText.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.NotesText, "Resource Notes");

Console.WriteLine("Notes text: " + resource.Get(Rsc.NotesText));
Console.WriteLine("Notes RTF: " + resource.Get(Rsc.NotesRTF));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


