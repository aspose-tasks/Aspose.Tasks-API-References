---
title: "ProjectFileInfo.CanRead"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ProjectFileInfo propiedad. Obtiene un valor que indica si Aspose.Tasks puede procesar el archivo del proyecto"
type: docs
weight: 10
url: /es/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Obtiene un valor que indica si Aspose.Tasks puede procesar el archivo de proyecto.

```csharp
public bool CanRead { get; }
```

## Ejemplos

Muestra cómo leer la información del archivo del proyecto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


