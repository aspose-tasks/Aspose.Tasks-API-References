---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Κόστη που προέκυψαν για υπερωριακή εργασία που ήδη εκτελέστηκε σε εργασίες από τους ανατεθειμένους πόρους."
type: docs
weight: 50
url: /el/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Κόστη που προκύπτουν για υπερωριακή εργασία που έχει ήδη εκτελεστεί σε εργασίες από τους εκχωρημένους πόρους.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


