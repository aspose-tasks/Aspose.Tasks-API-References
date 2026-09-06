---
title: "Prj.CurrencyCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le code de devise à trois lettres tel que défini dans ISO 4217. Exemple de valeurs valides : USD"
type: docs
weight: 150
url: /fr/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

Le code de devise à trois lettres tel que défini dans ISO 4217. Exemple de valeurs valides : "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
```

## Exemples

Montre comment écrire les propriétés monétaires du projet.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Définir les propriétés monétaires
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Afficher les propriétés monétaires
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


