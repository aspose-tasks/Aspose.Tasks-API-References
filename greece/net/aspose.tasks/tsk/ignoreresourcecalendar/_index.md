---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν ο προγραμματισμός της εργασίας λαμβάνει υπόψη τα ημερολόγια των πόρων που έχουν ανατεθεί στην εργασία"
type: docs
weight: 530
url: /el/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Καθορίζει εάν ο προγραμματισμός της εργασίας λαμβάνει υπόψη τα ημερολόγια των πόρων που έχουν ανατεθεί στην εργασία.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


