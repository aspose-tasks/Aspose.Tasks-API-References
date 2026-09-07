---
title: "Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν οι χειροκίνητες εργασίες πρέπει να διατηρούνται στην πλησιέστερη εργάσιμη ώρα όταν γίνονται αυτόματα προγραμματισμένες."
type: docs
weight: 400
url: /el/net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

Καθορίζει εάν οι χειροκίνητες εργασίες πρέπει να διατηρούνται στην πλησιέστερη εργάσιμη ώρα όταν ορίζονται ως αυτόματα προγραμματισμένες.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


