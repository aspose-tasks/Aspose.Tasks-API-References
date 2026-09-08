---
title: "Класс CompoundDocumentHeaderException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.CompoundDocumentHeaderException. Представляет исключение, которое выбрасывается, когда заголовок файла MPP повреждён."
type: docs
weight: 280
url: /ru/net/aspose.tasks/compounddocumentheaderexception/
---
## CompoundDocumentHeaderException class

Представляет исключение, которое выбрасывается, когда заголовок файла MPP повреждён.

```csharp
public class CompoundDocumentHeaderException : ApplicationException
```

## Примеры

Показывает, как отловить исключение &lt;see cref=\"CompoundDocumentHeaderException\" /&gt;.

```csharp
try
{
    var project = new Project(DataDir + "Project1.mpp");

    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (CompoundDocumentHeaderException e)
{
    Console.WriteLine(e.Message);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


