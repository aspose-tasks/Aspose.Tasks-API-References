---
title: ProjectServerManager.GetProjectRawData
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ProjectServerManager metodo. Ottiene i dati binari del progetto per la risoluzione dei problemi.
type: docs
weight: 60
url: /it/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Ottiene i dati binari del progetto per la risoluzione dei problemi.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectGuid | Guid | La guida del progetto da leggere. |

### Valore di ritorno

Flusso contenente i dati del progetto non elaborati.

### Esempi

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guida del progetto che stai cercando di ottenere.
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

### Guarda anche

* class [ProjectServerManager](../)
* spazio dei nomi [Aspose.Tasks](../../projectservermanager/)
* assemblea [Aspose.Tasks](../../../)


