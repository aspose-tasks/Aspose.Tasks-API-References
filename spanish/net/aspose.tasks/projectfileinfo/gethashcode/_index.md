---
title: "ProjectFileInfo.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ProjectFileInfo método. Devuelve un valor de código hash para la instancia de la clase ProjectFileInfo"
type: docs
weight: 60
url: /es/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

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


