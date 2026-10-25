---
title: "Clase BuildVersionInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.BuildVersionInfo. Contiene la versión de compilación y la información del producto"
type: docs
weight: 160
url: /es/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Contiene la versión de compilación y la información del producto.

```csharp
public static class BuildVersionInfo
```

## Campos

| Nombre | Descripción |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | El número de versión informativa del ensamblado. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Versión del ensamblado. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Versión del archivo. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Nombre del producto. |

## Ejemplos

Muestra cómo leer la información de la versión de compilación de Aspose.Tasks.

```csharp
// leer información común sobre la versión actual de Aspose.Tasks
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


