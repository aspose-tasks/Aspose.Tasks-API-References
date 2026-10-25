---
title: "Rsc.StandardRateFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Les unités utilisées par Microsoft Project pour afficher le taux standard"
type: docs
weight: 630
url: /fr/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Les unités utilisées par Microsoft Project pour afficher le taux standard.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


