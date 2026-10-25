---
title: "Prj.DurationFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η μορφή για την έκφραση της συνολικής διάρκειας"
type: docs
weight: 300
url: /el/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Η μορφή για την έκφραση της συνολικής διάρκειας.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


