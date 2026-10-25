---
title: "Classe GroupCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.GroupCollection. Contiene un elenco di oggetti Group. Implementa l'interfaccia ICollectionGroup"
type: docs
weight: 780
url: /it/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Contiene un elenco di oggetti [`Group`](../group/). Implementa l'interfaccia ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Ottiene un valore che indica se questa collezione è di sola lettura. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Converte una raccolta di gruppi in un elenco di oggetti [`Group`](../group/). |

## Esempi

Mostra come lavorare con una raccolta di gruppi.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// itera sui gruppi di attività
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// itera sui gruppi di risorse
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// cancella i gruppi di altri progetti
otherProject.TaskGroups.Clear();

// copia i gruppi in un altro progetto
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// aggiungi un gruppo di attività personalizzato
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// rimuovi tutti i gruppi
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Vedi anche

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


