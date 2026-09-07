---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επανααριθμεί τον κωδικό WBS όλων των εργασιών."
type: docs
weight: 1180
url: /el/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

Αναριθμεί τον κωδικό WBS όλων των εργασιών.

```csharp
public void RenumberWBSCode()
```

## Παραδείγματα

Δείχνει πώς να επανααριθμήσετε τους κωδικούς WBS των εργασιών.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// έξοδος: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// έξοδος: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

Αναριθμεί τον κωδικό WBS των περασμένων εργασιών.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskIds | List`1 | Αναγνωριστικά εργασιών για επανααρίθμηση κωδίκων WBS. |

## Παραδείγματα

Δείχνει πώς να επανααριθμήσετε τους κωδικούς WBS των επιλεγμένων εργασιών.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// έξοδος: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// έξοδος: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


