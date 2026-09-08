---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectFileInfo-eigenschap. Haalt de toepassingsinformatie van het projectbestand op"
type: docs
weight: 30
url: /nl/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Haalt de toepassingsinformatie van het projectbestand op.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


