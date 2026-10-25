---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν όλες οι ιδιότητες αρχείου θα αφαιρεθούν κατά την αποθήκευση"
type: docs
weight: 600
url: /el/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Καθορίζει εάν όλες οι ιδιότητες του αρχείου θα αφαιρεθούν κατά την αποθήκευση.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


