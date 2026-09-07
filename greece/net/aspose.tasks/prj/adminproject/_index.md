---
title: "Prj.AdminProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν ένα έργο είναι διοικητικό έργο"
type: docs
weight: 20
url: /el/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

Καθορίζει εάν ένα έργο είναι διοικητικό έργο.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.AdminProject.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


