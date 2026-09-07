---
title: "ProjectFileInfo.CanRead"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectFileInfo. Ottiene un valore che indica se le definizioni possono Aspose.Tasks elaborare il file di progetto"
type: docs
weight: 10
url: /it/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Restituisce un valore che indica se Aspose.Tasks può elaborare il file di progetto.

```csharp
public bool CanRead { get; }
```

## Esempi

Mostra come leggere le informazioni del file di progetto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


