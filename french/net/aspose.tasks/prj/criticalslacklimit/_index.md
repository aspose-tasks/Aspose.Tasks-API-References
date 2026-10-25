---
title: "Prj.CriticalSlackLimit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Les tâches sont considérées critiques par MS Project si le total de marge est inférieur ou égal à ce nombre de jours"
type: docs
weight: 140
url: /fr/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Les tâches sont considérées comme critiques par MS Project si le flottement total est inférieur ou égal à ce nombre de jours.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Exemples

Montre comment lire/écrire la propriété Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


