---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ProjectFileInfo. Ottiene il formato del file di progetto"
type: docs
weight: 40
url: /it/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Restituisce il formato del file di progetto.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


