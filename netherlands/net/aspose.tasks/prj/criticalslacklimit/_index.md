---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Taken worden door MS Project als kritisch beschouwd als de totale speling minder dan of gelijk aan dit aantal dagen is"
type: docs
weight: 140
url: /nl/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Taken worden door MS Project als kritisch beschouwd als de totale speling kleiner of gelijk is aan dit aantal dagen.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Voorbeelden

Toont hoe de eigenschap Prj.CriticalSlackLimit te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


