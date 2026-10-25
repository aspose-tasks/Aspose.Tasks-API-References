---
title: "Prj.LastSaved"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La fecha en que un proyecto se guardó por última vez. Guardado en formato UTC en archivos mpp. Tipo DateTime."
type: docs
weight: 440
url: /es/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

La fecha en que el proyecto se guardó por última vez. Guardada en formato UTC en archivos mpp. Tipo DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
```

## Ejemplos

Muestra cómo comprobar la versión de guardado del proyecto y la fecha de guardado.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Mostrar versión del proyecto
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


