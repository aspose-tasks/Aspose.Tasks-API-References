---
title: "ProjectFileInfo.CanRead"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectFileInfo eigenschap. Haalt een waarde op die aangeeft of definities Aspose.Tasks het projectbestand kunnen verwerken"
type: docs
weight: 10
url: /nl/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Haalt een waarde op die aangeeft of Aspose.Tasks het projectbestand kan verwerken.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


