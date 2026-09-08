---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectServerManager. Obtiene los datos binarios del proyecto con fines de solución de problemas."
type: docs
weight: 60
url: /es/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Obtiene los datos binarios del proyecto con fines de solución de problemas.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectGuid | Guid | El Guid del proyecto a leer. |

### Valor devuelto

Flujo que contiene los datos sin procesar del proyecto.

## Ejemplos

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// GUID del proyecto que estás intentando obtener.
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

Muestra cómo recuperar los datos sin procesar del proyecto desde Microsoft Project Online con fines de solución de problemas.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // El usuario puede leer el proyecto como un flujo de datos sin procesar con fines de solución de problemas.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // Puedes pasar el archivo resultante al soporte.
}
```

### Ver también

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


