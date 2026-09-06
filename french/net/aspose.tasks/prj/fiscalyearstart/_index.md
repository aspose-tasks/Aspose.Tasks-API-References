---
title: "Prj.FiscalYearStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si la numérotation de l'exercice fiscal est utilisée"
type: docs
weight: 340
url: /fr/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

Détermine si la numérotation de l'exercice fiscal est utilisée.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## Exemples

Montre comment écrire les propriétés de l'exercice fiscal.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// Définir les propriétés de l'année fiscale
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// Afficher les propriétés de l'année fiscale
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


