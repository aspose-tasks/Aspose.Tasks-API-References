---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Verzamelt recursief alle onderliggende taken van de hoofdtaak"
type: docs
weight: 1230
url: /nl/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Verzamelt recursief alle onderliggende taken van de hoofdtaak.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Retourwaarde

De verzameling van taken.

## Voorbeelden

Toont hoe de WBS-codes van geselecteerde taken opnieuw genummerd worden.

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

### Zie ook

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


