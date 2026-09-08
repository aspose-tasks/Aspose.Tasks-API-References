---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het formaat dat wordt gebruikt om de duur van de taak weer te geven"
type: docs
weight: 790
url: /nl/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Het formaat dat wordt gebruikt om de duur van de taak weer te geven.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Voorbeelden

Toont hoe een duur te verkrijgen met het standaardwerkformaat.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// maak een werkwaarde met het standaard werkformaat van het project
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


