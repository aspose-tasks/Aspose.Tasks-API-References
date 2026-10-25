---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De datum en tijd waarop een project is aangemaakt"
type: docs
weight: 130
url: /nl/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

De datum en tijd waarop een project is aangemaakt.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Opmerkingen

Opgeslagen in UTC-formaat in mpp-bestanden. Type DateTime.

## Voorbeelden

Toont hoe de eigenschap Prj.CreationDate te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


