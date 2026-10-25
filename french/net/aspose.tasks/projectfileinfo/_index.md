---
title: "Classe ProjectFileInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ProjectFileInfo. L'instance de la classe contient des informations sur le format du fichier de projet et la version de Microsoft Project avec laquelle le fichier a été créé"
type: docs
weight: 1460
url: /fr/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

L'instance de la classe contient des informations sur le format du fichier projet et la version de Microsoft Project avec laquelle le fichier a été créé.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Obtient une valeur indiquant si Aspose.Tasks peut traiter le fichier de projet. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Obtient une valeur indiquant si un projet est protégé par mot de passe. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Obtient les informations d'application du fichier de projet. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Obtient le format du fichier de projet. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Renvoie une valeur de code de hachage pour l'instance de la classe `ProjectFileInfo`. |

## Remarques

Utilisez la propriété CanRead pour définir que la bibliothèque peut traiter le fichier de projet.

## Exemples

Montre comment lire les informations du fichier de projet.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


