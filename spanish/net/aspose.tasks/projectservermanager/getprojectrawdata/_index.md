---
title: ProjectServerManager.GetProjectRawData
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ProjectServerManager método. Obtiene los datos binarios del proyecto para solucionar problemas.
type: docs
weight: 60
url: /es/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Obtiene los datos binarios del proyecto para solucionar problemas.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| projectGuid | Guid | El Guid del proyecto para leer. |

### Valor_devuelto

Secuencia que contiene los datos del proyecto sin procesar.

### Ejemplos

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "contraseña");
// GUID del proyecto que está tratando de obtener.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

### Ver también

* class [ProjectServerManager](../)
* espacio de nombres [Aspose.Tasks](../../projectservermanager/)
* asamblea [Aspose.Tasks](../../../)


