---
title: "Énumération LevelingOrder"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Leveling.LevelingOrder. Définit les valeurs possibles de l'ordre de nivellement"
type: docs
weight: 950
url: /fr/net/aspose.tasks.leveling/levelingorder/
---
## LevelingOrder enumeration

Définit les valeurs possibles de l'ordre de nivellement.

```csharp
public enum LevelingOrder
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Standard | `1` | Les propriétés suivantes sont prises en compte : relations de prédécesseur, marge totale (une tâche avec une marge totale plus élevée est retardée en premier), date de début, priorité. C’est la valeur par défaut. |
| IdOnly | `2` | Les tâches sont retardées par ordre croissant d'Id. |
| PriorityThenStandard | `3` | La priorité est considérée en premier, puis les mêmes propriétés que dans Standard. |

### Voir aussi

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


