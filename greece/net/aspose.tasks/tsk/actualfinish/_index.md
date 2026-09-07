---
title: "Tsk.ActualFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία ολοκλήρωσης μιας εργασίας"
type: docs
weight: 40
url: /el/net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

Η ημερομηνία κατά την οποία ολοκληρώθηκε ένα έργο.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
```

## Παραδείγματα

Δείχνει ότι οι ημερομηνίες του έργου επαναφέρονται σε λειτουργία αξιολόγησης.

```csharp
var project = new Project();

// δημιουργήστε νέες εργασίες
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


