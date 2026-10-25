---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectFileInfo. Restituisce le informazioni sull'applicazione del file di progetto"
type: docs
weight: 30
url: /it/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Restituisce le informazioni sull'applicazione del file di progetto.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


