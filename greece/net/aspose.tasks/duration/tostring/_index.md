---
title: "Duration.ToString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Επιστρέφει μια αναπαράσταση κειμένου αυτού του αντικειμένου"
type: docs
weight: 120
url: /el/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Επιστρέφει μια αναπαράσταση string αυτής της παρουσίας.

```csharp
public override string ToString()
```

### Τιμή Επιστροφής

μια αναπαράσταση κειμένου αυτού του αντικειμένου.

## Παραδείγματα

Δείχνει πώς να μετατρέψετε μια διάρκεια σε κείμενο.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// λάβετε τη διάρκεια της εργασίας
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


