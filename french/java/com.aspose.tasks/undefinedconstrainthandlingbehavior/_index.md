---
title: "UndefinedConstraintHandlingBehavior"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Spécifie le comportement utilisé pour gérer les tâches avec des contraintes indéfinies."
type: docs
weight: 329
url: /fr/java/com.aspose.tasks/undefinedconstrainthandlingbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class UndefinedConstraintHandlingBehavior extends System.Enum
```

Spécifie le comportement utilisé pour gérer les tâches avec des contraintes indéfinies.
## Champs

| Champ | Description |
| --- | --- |
| [None](#None) | Le comportement par défaut lors du chargement au format XER. |
| [SubstituteWithStartNoEarlierThan](#SubstituteWithStartNoEarlierThan) | Des contraintes de type 'ConstraintType.StartNoEarlierThan' et date = Start sont ajoutées aux tâches avec la contrainte 'Undefined'. |
### None {#None}
```
public static final int None
```


Le comportement par défaut lors du chargement au format XER. Aucune action n'est effectuée. Le type de contrainte d'une tâche est défini sur 'ConstraintType.Undefined'.

### SubstituteWithStartNoEarlierThan {#SubstituteWithStartNoEarlierThan}
```
public static final int SubstituteWithStartNoEarlierThan
```


Des contraintes de type 'ConstraintType.StartNoEarlierThan' et date = Start sont ajoutées aux tâches avec la contrainte 'Undefined'.

