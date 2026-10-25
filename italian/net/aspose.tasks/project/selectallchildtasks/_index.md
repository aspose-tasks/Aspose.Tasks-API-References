---
title: "Project.SelectAllChildTasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Raccoglie ricorsivamente tutti i task figli del task radice"
type: docs
weight: 1230
url: /it/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Raccoglie ricorsivamente tutte le attività figlio dell'attività radice.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valore di ritorno

La raccolta dei task.

## Esempi

Mostra come rinumerare i codici WBS dei task selezionati.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// output: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// output: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Vedi anche

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


