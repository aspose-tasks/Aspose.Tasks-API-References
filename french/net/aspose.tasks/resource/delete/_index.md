---
title: "Resource.Delete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode de Resource. Supprime une ressource et ses affectations du projet"
type: docs
weight: 810
url: /fr/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Supprime une ressource et ses affectations du projet.

```csharp
public void Delete()
```

## Exemples

Montre comment supprimer une ressource.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// supprimer la ressource
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Voir aussi

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


