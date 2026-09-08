---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Aangepast datumnotatie voor projectweergave. Wordt gebruikt om datums te formatteren wanneer de eigenschap DateFormat is ingesteld op Custom"
type: docs
weight: 200
url: /nl/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Aangepast datumnotatie voor projectweergave. Wordt gebruikt om datums te formatteren wanneer de eigenschap [`DateFormat`](../dateformat/) is ingesteld op Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Voorbeelden

Toont hoe de eigenschap Prj.CustomDateFormat te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


