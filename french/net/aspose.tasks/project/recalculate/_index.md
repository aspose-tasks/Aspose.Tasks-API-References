---
title: Project.Recalculate
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Project méthode. Replanifie tous les identifiants de tâches du projet les niveaux hiérarchiques les dates de début/fin définit les dates anticipées/tardives calcule les marges les champs de travail et de coût.
type: docs
weight: 1120
url: /fr/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Replanifie tous les identifiants de tâches du projet, les niveaux hiérarchiques, les dates de début/fin, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût.

```csharp
public void Recalculate()
```

### Voir également

* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Replanifie tous les identifiants de tâches du projet, les niveaux hiérarchiques, les dates de début/fin, définit les dates anticipées/tardives, calcule les marges, les champs de travail et de coût avec validation facultative.

```csharp
public void Recalculate(bool validate)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| validate | Boolean | Si vrai, la validation du recalcul sera effectuée. Quelles données sont validées : Pour le moment, seule la validation de base des plages de dates des tâches et des liens de tâches est implémentée. Les plages de dates de la tâche (par exemple, ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc. ) ainsi que les dates des liens de tâche seront vérifiées par rapport aux critères de date selon lesquels la date de début est inférieure ou égale à la date de fin. Si l'une des conditions décrites ci-dessus échoue, alors[`RecalculationValidationException`](../../recalculationvalidationexception/)sera lancé. |

### Voir également

* class [Project](../)
* espace de noms [Aspose.Tasks](../../project/)
* Assemblée [Aspose.Tasks](../../../)


