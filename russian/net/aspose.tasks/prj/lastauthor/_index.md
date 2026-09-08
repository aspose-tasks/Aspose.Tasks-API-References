---
title: "Prj.LastAuthor"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Последний автор проекта"
type: docs
weight: 420
url: /ru/net/aspose.tasks/prj/lastauthor/
---
## Prj.LastAuthor field

Последний автор проекта.

```csharp
public static readonly Key<string, PrjKey> LastAuthor;
```

## Примеры

Показывает, как установить метаданные проекта.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Установить информацию о проекте
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


