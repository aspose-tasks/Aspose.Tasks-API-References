---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ProjectFileInfo propiedad. Obtiene el formato del archivo del proyecto"
type: docs
weight: 40
url: /es/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Obtiene el formato del archivo de proyecto.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


