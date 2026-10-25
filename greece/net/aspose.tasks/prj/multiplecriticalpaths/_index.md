---
title: "Prj.MultipleCriticalPaths"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν υπολογίζονται πολλαπλές κρίσιμες διαδρομές"
type: docs
weight: 530
url: /el/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

Καθορίζει εάν υπολογίζονται πολλαπλές κρίσιμες διαδρομές.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MultipleCriticalPaths.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


