---
title: "WorkingTime"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un temps de travail pendant un jour de la semaine."
type: docs
weight: 365
url: /fr/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Représente un temps de travail pendant un jour de la semaine.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Initialise une nouvelle instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime) avec un intervalle avec les heures de début et de fin spécifiées. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Initialise une nouvelle instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime) avec un élément d'intervalle avec les heures de début et de fin spécifiées. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Initialise une nouvelle instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime) avec un élément d'intervalle avec les heures de début et de fin spécifiées. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Vérifie que les objets sont égaux. |
| [getFrom()](#getFrom--) | Obtient le début d'un temps de travail. |
| [getTo()](#getTo--) | Obtient la fin d'un temps de travail. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Initialise une nouvelle instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime) avec un intervalle avec les heures de début et de fin spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fromTime | java.util.Date | heure de début de l'intervalle |
| toTime | java.util.Date | heure de fin de l'intervalle |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Initialise une nouvelle instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime) avec un élément d'intervalle avec les heures de début et de fin spécifiées.

--------------------

&gt; ```
&gt; La surcharge du constructeur WorkingTime peut être utilisée pour initialiser le début et la fin de l'intervalle à l'aide de TimeSpans:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fromHours | int | Heure de début de l'intervalle représentée par un nombre entier d'heures (0-24). |
| toHours | int | Heure de fin de l'intervalle représentée par un nombre entier d'heures (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Vérifie que les objets sont égaux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | Deuxième objet à comparer. |

**Returns:**
booléen - Vrai si les objets sont égaux, faux sinon.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Obtient le début d'un temps de travail.

**Returns:**
java.util.Date - le début d'un temps de travail.
### getTo() {#getTo--}
```
public final Date getTo()
```


Obtient la fin d'un temps de travail.

**Returns:**
java.util.Date - la fin d'un temps de travail.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
