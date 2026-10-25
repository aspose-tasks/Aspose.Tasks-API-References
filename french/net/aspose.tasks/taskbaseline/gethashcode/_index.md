---
title: "TaskBaseline.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskBaseline. Retourne une valeur de code de hachage pour l'instance de la classe TaskBaseline"
type: docs
weight: 110
url: /fr/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir le code de hachage d'une ligne de base de tâche.

```csharp
var project = new Project();

// création de TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// afficher la durée de la baseline de la tâche
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// le code de hachage d'un calendrier est égal au numéro de la ligne de base 
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Voir aussi

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


