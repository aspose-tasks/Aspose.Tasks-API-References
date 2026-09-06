---
title: "ProjectFileInfo.CanRead"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ProjectFileInfo. Obtient une valeur indiquant si les définitions peuvent être traitées par Aspose.Tasks le fichier de projet"
type: docs
weight: 10
url: /fr/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Obtient une valeur indiquant si Aspose.Tasks peut traiter le fichier de projet.

```csharp
public bool CanRead { get; }
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

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


