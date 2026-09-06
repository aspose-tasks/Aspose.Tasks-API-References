---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectFileInfo. Obtient les informations d’application du fichier de projet"
type: docs
weight: 30
url: /fr/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Obtient les informations d'application du fichier de projet.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


