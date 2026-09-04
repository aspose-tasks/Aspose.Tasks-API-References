---
title: "TaskStatus"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Spécifie le statut d'une tâche."
type: docs
weight: 301
url: /fr/java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

Spécifie le statut d'une tâche.
## Champs

| Champ | Description |
| --- | --- |
| [Complete](#Complete) | La tâche est terminée à 100 %. |
| [Future](#Future) | 'Future' le statut de la tâche est défini lorsque la date de début de la tâche est supérieure à la date du statut. |
| [Late](#Late) | La tâche est en retard si le pourcentage cumulé temporel ne atteint pas minuit la veille de la date du statut. |
| [OnSchedule](#OnSchedule) | La tâche est à l'heure si le pourcentage cumulé temporel est réparti jusqu'au moins la veille de la date du statut. |
| [Undefined](#Undefined) | Statut de tâche non défini. |
### Complete {#Complete}
```
public static final int Complete
```


La tâche est terminée à 100 %.

### Future {#Future}
```
public static final int Future
```


'Future' le statut de la tâche est défini lorsque la date de début de la tâche est supérieure à la date du statut.

### Late {#Late}
```
public static final int Late
```


La tâche est en retard si le pourcentage cumulé temporel ne atteint pas minuit la veille de la date du statut.

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


La tâche est à l'heure si le pourcentage cumulé temporel est réparti jusqu'au moins la veille de la date du statut.

### Undefined {#Undefined}
```
public static final int Undefined
```


Statut de tâche non défini.

