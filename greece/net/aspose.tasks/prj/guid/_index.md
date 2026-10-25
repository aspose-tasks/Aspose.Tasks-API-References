---
title: "Prj.Guid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Το GUID του έργου"
type: docs
weight: 360
url: /el/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

Το GUID του έργου.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


