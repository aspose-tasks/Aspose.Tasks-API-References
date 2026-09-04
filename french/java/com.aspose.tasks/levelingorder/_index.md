---
title: "LevelingOrder"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Définit les valeurs possibles de l'ordre de nivellement."
type: docs
weight: 143
url: /fr/java/com.aspose.tasks/levelingorder/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class LevelingOrder extends System.Enum
```

Définit les valeurs possibles de l'ordre de nivellement.
## Champs

| Champ | Description |
| --- | --- |
| [IdOnly](#IdOnly) | Les tâches sont retardées par ordre croissant d'Id. |
| [PriorityThenStandard](#PriorityThenStandard) | La priorité est considérée en premier, puis les mêmes propriétés que dans Standard. |
| [Standard](#Standard) | Les propriétés suivantes sont prises en compte : relations de prédécesseur, marge totale (une tâche avec une marge totale plus élevée est retardée en premier), date de début, priorité. |
### IdOnly {#IdOnly}
```
public static final int IdOnly
```


Les tâches sont retardées par ordre croissant d'Id.

### PriorityThenStandard {#PriorityThenStandard}
```
public static final int PriorityThenStandard
```


La priorité est considérée en premier, puis les mêmes propriétés que dans Standard.

### Standard {#Standard}
```
public static final int Standard
```


Les propriétés suivantes sont prises en compte : relations de prédécesseur, marge totale (une tâche avec une marge totale plus élevée est retardée en premier), date de début, priorité. C’est la valeur par défaut.

