---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectFileInfo. Obtient le format du fichier de projet"
type: docs
weight: 40
url: /fr/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Obtient le format du fichier de projet.

```csharp
public FileFormat ProjectFileFormat { get; }
```

## Exemples

Montre comment lire les informations du fichier de projet.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Voir aussi

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


