---
title: "Prj.Comments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. Comentarios del proyecto"
type: docs
weight: 110
url: /es/net/aspose.tasks/prj/comments/
---
## Prj.Comments field

Comentarios del proyecto.

```csharp
public static readonly Key<string, PrjKey> Comments;
```

## Ejemplos

Muestra cómo establecer la información meta del proyecto.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Establecer información del proyecto
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

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


