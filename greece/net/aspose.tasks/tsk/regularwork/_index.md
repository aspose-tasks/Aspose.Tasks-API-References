---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το συνολικό ποσό μη υπερωριακής εργασίας που έχει προγραμματιστεί να εκτελεστεί από τους πόρους"
type: docs
weight: 940
url: /el/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

Το συνολικό ποσό μη υπερωριακής εργασίας που προγραμματίζεται να εκτελεστεί από τους πόρους.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


