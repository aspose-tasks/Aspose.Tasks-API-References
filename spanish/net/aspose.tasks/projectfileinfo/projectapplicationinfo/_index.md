---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ProjectFileInfo. Obtiene la información de la aplicación del archivo de proyecto"
type: docs
weight: 30
url: /es/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Obtiene la información de la aplicación del archivo de proyecto.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


