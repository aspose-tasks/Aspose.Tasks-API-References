---
title: "Prj.Autolink"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν οι εισαχθείσες ή μετακινημένες εργασίες συνδέονται αυτόματα"
type: docs
weight: 70
url: /el/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Καθορίζει εάν οι εισαχθείσες ή μετακινημένες εργασίες συνδέονται αυτόματα.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


