---
title: "Prj.Author"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Автор проекта"
type: docs
weight: 40
url: /ru/net/aspose.tasks/prj/author/
---
## Prj.Author field

Автор проекта.

```csharp
public static readonly Key<string, PrjKey> Author;
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


