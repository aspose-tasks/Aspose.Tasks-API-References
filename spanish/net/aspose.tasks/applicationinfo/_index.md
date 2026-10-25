---
title: "Enumeración ApplicationInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.ApplicationInfo. Especifica la versión del proyecto en la que se creó el archivo"
type: docs
weight: 10
url: /es/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Especifica la versión del proyecto en la que se creó el archivo.

```csharp
public enum ApplicationInfo
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `0` | No se puede definir. |
| MSP2000 | `1` | El archivo se creó en Microsoft Project 2000/2002. |
| MSP2003 | `2` | El archivo se creó en Microsoft Project 2003. |
| MSP2007 | `3` | El archivo se creó en Microsoft Project 2007. |
| MSP2010 | `4` | El archivo se creó en Microsoft Project 2010. |
| MSP2013 | `5` | El archivo se creó en Microsoft Project 2013. |
| MSP2016 | `6` | El archivo se creó en Microsoft Project 2016. |

## Ejemplos

Muestra cómo comprobar la información de la aplicación del proyecto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


