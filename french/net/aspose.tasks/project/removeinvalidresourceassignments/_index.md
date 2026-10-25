---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Élimine les affectations de ressources invalides de la liste des affectations de ressources du projet"
type: docs
weight: 1170
url: /fr/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Élimine les affectations de ressources invalides de la liste des affectations de ressources du projet.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Remarques

MS Project crée une affectation de ressource vide pour chaque tâche. Appelez la méthode pour les supprimer.

## Exemples

Montre comment supprimer les affectations invalides.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// supprimer les affectations invalides
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


