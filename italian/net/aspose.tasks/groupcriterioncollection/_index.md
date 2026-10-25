---
title: "Classe GroupCriterionCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.GroupCriterionCollection. Contiene una raccolta di oggetti GroupCriterion. Implementa l'interfaccia ICollectionGroupCriterion."
type: docs
weight: 800
url: /it/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Contiene una raccolta di oggetti [`GroupCriterion`](../groupcriterion/). Implementa l'interfaccia ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Converte una raccolta di GroupCriterion in un elenco di oggetti [`GroupCriterion`](../groupcriterion/). |

## Esempi

Mostra come lavorare con una raccolta di criteri di gruppo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// itera sui criteri di gruppo
Console.WriteLine("Print group criteria of the group '{0}': ", group.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Field: " + criterion.Field);
    Console.WriteLine("Group On: " + criterion.GroupOn);
    Console.WriteLine();
}

group.GroupCriteria.Clear();

if (!group.GroupCriteria.IsReadOnly)
{
    List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
    foreach (var criterion in groupCriteria)
    {
        group.GroupCriteria.Remove(criterion);
    }
}

var criterionToAdd = new GroupCriterion
{
    Ascending = true,
    Field = Field.TaskActive
};

if (!group.GroupCriteria.Contains(criterionToAdd))
{
    group.GroupCriteria.Add(criterionToAdd);
}

// copia i criteri in un altro gruppo
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Vedi anche

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


