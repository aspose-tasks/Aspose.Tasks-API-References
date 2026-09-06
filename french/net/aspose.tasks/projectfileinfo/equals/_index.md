---
title: "ProjectFileInfo.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ProjectFileInfo. Retourne une valeur indiquant si cette instance est égale à un objet spécifié"
type: docs
weight: 50
url: /fr/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | ProjectFileInfo | L'objet spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie vrai si le ProjectFileInfo spécifié et cette instance ont le même format de fichier et les mêmes informations d'application.

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

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie vrai si le ProjectFileInfo spécifié et cette instance ont le même format de fichier et les mêmes informations d'application.

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


