---
title: "Enumeración FileFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.FileFormat. Especifica el formato de archivo de los proyectos"
type: docs
weight: 590
url: /es/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Especifica el formato de archivo del proyecto.

```csharp
public enum FileFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `0` | No se puede definir. |
| P6XML | `1` | Representa el formato XML de Primavera P6. |
| XML | `2` | Formato XML de Microsoft Project. |
| MPP8 | `3` | Formato Microsoft Project 2000. |
| MPP9 | `4` | Formato Microsoft Project 2003. |
| MPP12 | `5` | Formato Microsoft Project 2007. |
| MPP14 | `6` | Formato Microsoft Project 2010. |
| MPT9 | `7` | Formato de plantilla Microsoft Project 2003. |
| MPT12 | `8` | Formato de plantilla Microsoft Project 2007. |
| MPT14 | `9` | Formato de plantilla de Microsoft Project 2010 (2013). |
| MPX | `10` | Formato de archivo Mpx |
| XER | `11` | Representa el formato Primavera XER |
| HTML | `12` | Representa el formato HTML |
| ProjectServer | `13` | El proyecto se leyó de Project Server o Project Online |

## Ejemplos

Muestra cómo leer el formato de archivo de proyecto de verificación.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


