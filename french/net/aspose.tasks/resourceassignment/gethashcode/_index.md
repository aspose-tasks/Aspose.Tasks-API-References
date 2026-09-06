---
title: "ResourceAssignment.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Retourne une valeur de code de hachage pour l'instance de la classe ResourceAssignment"
type: docs
weight: 710
url: /fr/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une affectation de ressource.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// imprimer les codes de hachage de l'affectation
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


