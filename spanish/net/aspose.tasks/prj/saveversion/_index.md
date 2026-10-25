---
title: "Prj.SaveVersion"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La versión de Microsoft Office Project con la que se guardó un archivo de proyecto"
type: docs
weight: 620
url: /es/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

La versión de Microsoft Office Project con la que se guardó un archivo de proyecto.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
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


