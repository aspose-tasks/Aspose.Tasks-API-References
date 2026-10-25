---
title: "Prj.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Το όνομα του έργου"
type: docs
weight: 540
url: /el/net/aspose.tasks/prj/name/
---
## Prj.Name field

Το όνομα του έργου.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε το όνομα του έργου.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


