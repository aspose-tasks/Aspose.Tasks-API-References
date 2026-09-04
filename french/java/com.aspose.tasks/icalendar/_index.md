---
title: "ICalendar"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une abstraction de calendrier qui peut être utilisée pour divers calculs de dates et de durées."
type: docs
weight: 376
url: /fr/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Représente une abstraction de calendrier qui peut être utilisée pour divers calculs de dates et de durées.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Calcule le début du prochain jour ouvrable pour la date spécifiée. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Calcule la fin de la journée ouvrable précédente à partir de la date spécifiée. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée de travail. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Calcule le début du prochain créneau de travail à partir de la date et de l'heure spécifiées. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Renvoie le nombre d'heures de travail à la date spécifiée. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Renvoie le nombre d'heures de travail entre les dates spécifiées. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Renvoie [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) des temps de travail pour la date spécifiée. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Détermine si le jour spécifié est un jour ouvrable selon le calendrier. |
| [isEmpty()](#isEmpty--) | Renvoie si le calendrier n'a pas d'heures de travail définies. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Date de début. |
| work | [Duration](../../com.aspose.tasks/duration) | Durée du travail. |

**Returns:**
java.util.Date - Date de fin.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Date de début. |
| travail | double | Durée du travail. |

**Returns:**
java.util.Date - Date de fin.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Calcule le début du prochain jour ouvrable pour la date spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| date | java.util.Date | La date pour obtenir le début du prochain jour ouvrable. |

**Returns:**
java.util.Date - Début du prochain jour ouvrable System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Calcule la fin de la journée ouvrable précédente à partir de la date spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| date | java.util.Date | la date pour calculer la fin du jour ouvrable précédent. |

**Returns:**
java.util.Date - La fin du jour ouvrable précédent
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Renvoie la date de début basée sur la date de fin et la durée spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fin | java.util.Date | La date de fin spécifiée. |
| duration | [Duration](../../com.aspose.tasks/duration) | La durée spécifiée. |

**Returns:**
java.util.Date - Date de début calculée.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Renvoie la date de début basée sur la date de fin et la durée spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fin | java.util.Date | La date de fin spécifiée. |
| durée | double | La durée spécifiée. |

**Returns:**
java.util.Date - Date de début calculée.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée de travail.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | La tâche pour calculer la date de fin. |
|  | durée | double | La durée à calculer. |

Renvoie DateTime.MinValue si la tâche est un résumé, null ou si sa date de début n'est pas définie. |

**Returns:**
java.util.Date - Date de fin de la tâche pour la date de début et la durée données.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Calcule le début du prochain créneau de travail à partir de la date et de l'heure spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| date | java.util.Date | La date et l'heure. |

**Returns:**
java.util.Date - Le début du temps ouvrable le plus proche.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Renvoie le nombre d'heures de travail à la date spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | La date pour obtenir les heures de travail. |

**Returns:**
double - Heures de travail à la date spécifiée.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Date de début de l'intervalle. |
| fin | java.util.Date | Date de fin de l'intervalle. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Renvoie le nombre d'heures de travail entre les dates spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Date de début de l'intervalle. |
| fin | java.util.Date | Date de fin de l'intervalle. |

**Returns:**
double - Quantité d'heures de travail selon l'instance du calendrier.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Renvoie [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) des temps de travail pour la date spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | La date pour obtenir les horaires de travail. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Détermine si le jour spécifié est un jour ouvrable selon le calendrier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | La date pour vérifier si le jour est ouvrable. |

**Returns:**
boolean - Vrai si le jour est ouvrable.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Renvoie si le calendrier n'a pas d'heures de travail définies.

**Returns:**
booléen - Vrai si le calendrier n'a pas d'heures de travail définies.
