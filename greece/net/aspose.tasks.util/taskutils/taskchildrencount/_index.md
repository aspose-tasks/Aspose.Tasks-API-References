---
title: "TaskUtils.TaskChildrenCount"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskUtils. Υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών σε όλα τα επίπεδα"
type: docs
weight: 40
url: /el/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών μιας εργασίας σε όλα τα επίπεδα.

```csharp
public static int TaskChildrenCount(Task task)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Η εργασία της οποίας τα παιδιά υπολογίζονται. |

### Τιμή Επιστροφής

Ο αριθμός των παιδιών.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη μέθοδο &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// υπολογίζει αναδρομικά τον αριθμό των παιδικών εργασιών μιας εργασίας σε όλα τα επίπεδα
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


