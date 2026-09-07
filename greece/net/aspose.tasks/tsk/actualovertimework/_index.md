---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η πραγματική ποσότητα υπερωριακής εργασίας που έχει ήδη εκτελεστεί από τους πόρους που έχουν ανατεθεί σε εργασίες"
type: docs
weight: 60
url: /el/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

Το πραγματικό ποσό υπερωριακής εργασίας που έχει ήδη εκτελεστεί από τους πόρους που έχουν ανατεθεί σε έργα.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


