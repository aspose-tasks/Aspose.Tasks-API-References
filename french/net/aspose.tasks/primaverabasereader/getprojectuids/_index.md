---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode PrimaveraBaseReader. Retourne une liste des identifiants uniques des projets"
type: docs
weight: 20
url: /fr/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Retourner une liste des identifiants uniques des projets.

```csharp
public List<int> GetProjectUids()
```

### Valeur de retour

Liste des identifiants uniques des projets.

## Exemples

Montre comment importer un projet à partir d'un fichier XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### Voir aussi

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


