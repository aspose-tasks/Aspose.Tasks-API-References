---
title: "FilterCriteria.CriteriaRows"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété FilterCriteria. Obtient la liste des lignes FilterCriteria enfants. Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur And est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource soit affichée en résultat de ce filtre. L'effet d'un opérateur Or est que les critères de l'une ou l'autre ligne doivent être remplis"
type: docs
weight: 20
url: /fr/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

Obtient la liste des lignes [`FilterCriteria`](../) enfants. Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur And est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource soit affichée en résultat de ce filtre. L'effet d'un opérateur Or est que les critères de l'une ou l'autre ligne doivent être remplis.

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

## Exemples

Montre comment lire les critères de filtre de tâche.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// Imprimer les critères de filtre sous forme de chaîne 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Voir aussi

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


