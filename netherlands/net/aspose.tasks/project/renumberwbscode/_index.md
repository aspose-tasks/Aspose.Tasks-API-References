---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Nummer de WBS-code van alle taken opnieuw"
type: docs
weight: 1180
url: /nl/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

Her nummer WBS-code van alle taken.

```csharp
public void RenumberWBSCode()
```

## Voorbeelden

Toont hoe de WBS-codes van taken opnieuw genummerd worden.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// output: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// output: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

Her nummer WBS-code van voltooide taken.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskIds | List`1 | Taak-id's om WBS-codes opnieuw te nummeren. |

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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


