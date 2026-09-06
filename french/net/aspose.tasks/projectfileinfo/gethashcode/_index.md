---
title: "ProjectFileInfo.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectFileInfo. Retourne une valeur de code de hachage pour l'instance de la classe ProjectFileInfo"
type: docs
weight: 60
url: /fr/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

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


