---
title: "Clase ProjectFileInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectFileInfo. La instancia de la clase contiene información sobre el formato del archivo de proyecto y la versión de Microsoft Project en la que se creó el archivo"
type: docs
weight: 1460
url: /es/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

La instancia de la clase contiene información sobre el formato del archivo de proyecto y la versión de Microsoft Project con la que se creó el archivo.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Obtiene un valor que indica si Aspose.Tasks puede procesar el archivo de proyecto. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Obtiene un valor que indica si un proyecto está protegido con contraseña. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Obtiene la información de la aplicación del archivo de proyecto. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Obtiene el formato del archivo de proyecto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `ProjectFileInfo`. |

## Observaciones

Utilice la propiedad CanRead para definir que la biblioteca puede procesar el archivo del proyecto.

## Ejemplos

Muestra cómo leer la información del archivo del proyecto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


