---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraReadOptions. Λαμβάνει ή ορίζει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα"
type: docs
weight: 30
url: /el/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Λαμβάνει ή ορίζει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα.

```csharp
public int ProjectUid { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML ή Primavera XER που περιέχει πολλαπλά έργα.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Επιστρέφει έργο με ειδικό UID
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


