---
title: "VbaProject.CompilationArguments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaProject. Obtiene los argumentos de compilación condicionales"
type: docs
weight: 10
url: /es/net/aspose.tasks/vbaproject/compilationarguments/
---
## VbaProject.CompilationArguments property

Obtiene los argumentos de compilación condicional

```csharp
public string CompilationArguments { get; }
```

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

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


