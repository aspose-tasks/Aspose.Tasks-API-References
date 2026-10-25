---
title: "Prj.Revision"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El número de veces que se guardó un proyecto"
type: docs
weight: 610
url: /es/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

El número de veces que se guardó un proyecto.

```csharp
public static readonly Key<int, PrjKey> Revision;
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


