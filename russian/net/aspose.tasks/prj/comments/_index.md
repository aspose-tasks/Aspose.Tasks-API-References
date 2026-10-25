---
title: "Prj.Comments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Комментарии проекта"
type: docs
weight: 110
url: /ru/net/aspose.tasks/prj/comments/
---
## Prj.Comments field

Комментарии проекта.

```csharp
public static readonly Key<string, PrjKey> Comments;
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


