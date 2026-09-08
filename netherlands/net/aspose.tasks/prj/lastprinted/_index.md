---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Laatste afdruktijd van projecten. Opgeslagen in UTC-formaat in mpp-bestanden. Type DateTime"
type: docs
weight: 430
url: /nl/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Laatste afdruktijd van het project. Opgeslagen in UTC-formaat in mpp-bestanden. Type DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Voorbeelden

Toont hoe de eigenschap Prj.LastPrinted te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


