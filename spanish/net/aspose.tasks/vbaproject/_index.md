---
title: "Clase VbaProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaProject. Representa VbaProject"
type: docs
weight: 2860
url: /es/net/aspose.tasks/vbaproject/
---
## VbaProject class

Representa `VbaProject`.

```csharp
public class VbaProject
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Obtiene los argumentos de compilación condicional |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Obtiene una descripción del proyecto. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Obtiene el Id de contexto de ayuda del proyecto |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Obtiene el nombre del archivo de ayuda |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Obtiene una colección de [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Obtiene el nombre del proyecto |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Obtiene una colección de [`VbaReferenceCollection`](../vbareferencecollection/) |

## Ejemplos

Muestra cómo leer las propiedades del proyecto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


