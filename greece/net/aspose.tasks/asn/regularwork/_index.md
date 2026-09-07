---
title: "Asn.RegularWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Asn. Η ποσότητα μη υπερωριακής εργασίας που έχει προγραμματιστεί για μια ανάθεση"
type: docs
weight: 420
url: /el/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

Το ποσό της μη υπερωριακής εργασίας που έχει προγραμματιστεί για μια ανάθεση.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Asn.RegularWork.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


