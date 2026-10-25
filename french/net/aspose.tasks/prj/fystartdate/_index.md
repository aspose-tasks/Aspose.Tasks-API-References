---
title: "Prj.FyStartDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le mois où l'année fiscale commence"
type: docs
weight: 350
url: /fr/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

Le mois où l'exercice fiscal commence.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


