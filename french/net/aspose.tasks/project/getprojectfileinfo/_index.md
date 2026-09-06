---
title: "Project.GetProjectFileInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Lit les informations du fichier de projet depuis le fichier"
type: docs
weight: 1280
url: /fr/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Lit les informations du fichier de projet depuis le fichier.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | Chaîne | Le nom de fichier du projet. |

### Valeur de retour

Les informations du fichier de projet [`ProjectFileInfo`](../../projectfileinfo/).

## Exemples

Montre comment lire les informations du fichier de projet à partir d'un fichier XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Voir aussi

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Obtient les informations du fichier de projet depuis le flux.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Flux | Le flux de données. |

### Valeur de retour

Les informations du fichier de projet [`ProjectFileInfo`](../../projectfileinfo/).

## Exemples

Montre comment lire les informations du fichier de projet d'un fichier XML lu depuis un flux.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Voir aussi

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


