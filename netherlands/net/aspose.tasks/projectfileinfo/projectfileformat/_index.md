---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectFileInfo eigenschap. Haalt het bestandsformaat van het project op"
type: docs
weight: 40
url: /nl/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Haalt het projectbestandsformaat op.

```csharp
public FileFormat ProjectFileFormat { get; }
```

## Voorbeelden

Toont hoe je projectbestandsinformatie kunt lezen.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


