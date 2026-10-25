---
title: "GroupCollection.Contains"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo GroupCollection. Restituisce true se l'elemento specificato è trovato in questa raccolta, altrimenti false"
type: docs
weight: 50
url: /it/net/aspose.tasks/groupcollection/contains/
---
## GroupCollection.Contains method

Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false.

```csharp
public bool Contains(Group item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | Group | l'elemento specificato da trovare. |

### Valore di ritorno

true se l'elemento specificato è trovato in questa collezione; altrimenti, false.

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


