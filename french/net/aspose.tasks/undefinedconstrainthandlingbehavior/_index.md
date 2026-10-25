---
title: "Énumération UndefinedConstraintHandlingBehavior"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.UndefinedConstraintHandlingBehavior. Spécifie le comportement utilisé pour gérer les tâches avec des contraintes non définies"
type: docs
weight: 2630
url: /fr/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

Spécifie le comportement utilisé pour gérer les tâches avec des contraintes indéfinies.

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Le comportement par défaut lors du chargement depuis le format XER. Aucune action n'est effectuée. Le type de contrainte d'une tâche est défini sur 'ConstraintType.Undefined'. |
| SubstituteWithStartNoEarlierThan | `1` | Des contraintes de type 'ConstraintType.StartNoEarlierThan' et date = Start sont ajoutées pour les tâches avec la contrainte 'Undefined'. |

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


