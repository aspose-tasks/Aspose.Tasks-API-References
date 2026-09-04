---
title: "CalendarException"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente des périodes de temps exceptionnelles dans un calendrier."
type: docs
weight: 43
url: /fr/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Représente des périodes de temps exceptionnelles dans un calendrier.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CalendarException()](#CalendarException--) | Initialise une nouvelle instance de la classe [CalendarException](../../com.aspose.tasks/calendarexception). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Renvoie true si l'instance spécifiée de la structure java.util.Date correspond au jour d'exception. |
| [delete()](#delete--) | Supprime l'instance Exception de l'objet CalendarExceptionCollection du calendrier parent. |
| [getDayWorking()](#getDayWorking--) | Obtient une valeur indiquant si la date ou le type de jour spécifié est ouvrable. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Obtient le DayTypeCollection pour cet objet. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Obtient une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. |
| [getExceptionDates()](#getExceptionDates--) | Renvoie les dates auxquelles l'exception du calendrier s'applique. |
| [getFromDate()](#getFromDate--) | Obtient le début de la période d'exception. |
| [getMonth()](#getMonth--) | Obtient le mois pour lequel une récurrence d'exception est prévue. |
| [getMonthDay()](#getMonthDay--) | Obtient le jour du mois auquel une récurrence d'exception est prévue. |
| [getMonthItem()](#getMonthItem--) | Obtient l'élément du mois pour lequel une récurrence d'exception est prévue. |
| [getMonthPosition()](#getMonthPosition--) | Obtient la position d'un élément du mois au sein d'un mois. |
| [getName()](#getName--) | Obtient le nom de l'exception. |
| [getOccurrences()](#getOccurrences--) | Obtient le nombre d'occurrences pendant lesquelles l'exception du calendrier est valide. |
| [getParentCalendar()](#getParentCalendar--) | Obtient le calendrier parent de cet objet. |
| [getPeriod()](#getPeriod--) | Obtient la période de récurrence de l'exception. |
| [getToDate()](#getToDate--) | Obtient la fin de la période d'exception. |
| [getType()](#getType--) | Obtient le type d'exception. |
| [getWorkingTime()](#getWorkingTime--) | Renvoie le temps de travail pour une exception de calendrier. |
| [getWorkingTimes()](#getWorkingTimes--) | Obtient l'objet WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Définit une valeur indiquant si la date ou le type de jour spécifié est ouvrable. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Définit le début de la période d'exception. |
| [setMonth(int value)](#setMonth-int-) | Définit le mois pour lequel une récurrence d'exception est planifiée. |
| [setMonthDay(int value)](#setMonthDay-int-) | Définit le jour du mois auquel une récurrence d'exception est planifiée. |
| [setMonthItem(int value)](#setMonthItem-int-) | Définit l'élément de mois pour lequel une récurrence d'exception est planifiée. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Définit la position d'un élément de mois au sein d'un mois. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de l'exception. |
| [setOccurrences(int value)](#setOccurrences-int-) | Définit le nombre d'occurrences pendant lesquelles l'exception de calendrier est valide. |
| [setPeriod(int value)](#setPeriod-int-) | Définit la période de récurrence de l'exception. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Définit la fin de la période d'exception. |
| [setType(int value)](#setType-int-) | Définit le type d'exception. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Définit l'objet WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Initialise une nouvelle instance de la classe [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Renvoie true si l'instance spécifiée de la structure java.util.Date correspond au jour d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dt | java.util.Date | l'instance spécifiée de la structure java.util.Date. |

**Returns:**
boolean - Retourne true si la valeur java.util.Date est le jour d'exception ; sinon, false.
### delete() {#delete--}
```
public final void delete()
```


Supprime l'instance Exception de l'objet CalendarExceptionCollection du calendrier parent.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Obtient une valeur indiquant si la date ou le type de jour spécifié est ouvrable.

**Returns:**
booléen - une valeur indiquant si la date ou le type de jour spécifié est ouvré.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Obtient le DayTypeCollection pour cet objet. Les jours de la semaine pendant lesquels l'exception est valide.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Obtient une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False indique que la plage de récurrence est définie en saisissant une date de fin.

**Returns:**
boolean - une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Renvoie les dates auxquelles l'exception du calendrier s'applique.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - dates auxquelles l'exception de calendrier s'applique.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Obtient le début de la période d'exception.

**Returns:**
java.util.Date - le début de la période d'exception.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Obtient le mois pour lequel une récurrence d'exception est prévue.

**Returns:**
int - le mois pour lequel une récurrence d'exception est planifiée.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Obtient le jour du mois auquel une récurrence d'exception est prévue.

**Returns:**
int - le jour du mois auquel une récurrence d'exception est planifiée.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Obtient l'élément du mois pour lequel une récurrence d'exception est prévue.

**Returns:**
int - l'élément de mois pour lequel une récurrence d'exception est planifiée.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Obtient la position d'un élément du mois au sein d'un mois.

**Returns:**
int - la position d'un élément de mois au sein d'un mois.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'exception.

**Returns:**
java.lang.String - le nom de l'exception.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Obtient le nombre d'occurrences pendant lesquelles l'exception du calendrier est valide.

**Returns:**
int - le nombre d'occurrences pendant lesquelles l'exception de calendrier est valide.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Obtient le calendrier parent de cet objet.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Obtient la période de récurrence de l'exception.

**Returns:**
int - la période de récurrence de l'exception.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Obtient la fin de la période d'exception.

**Returns:**
java.util.Date - la fin du temps d'exception.
### getType() {#getType--}
```
public final int getType()
```


Obtient le type d'exception.

**Returns:**
int - le type d'exception.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Renvoie le temps de travail pour une exception de calendrier.

**Returns:**
double - Retourne le temps de travail pour cette exception de calendrier.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Obtient l'objet WorkingTimeCollection. La collection des temps de travail qui définit le temps travaillé pendant le jour de la semaine.

--------------------

Au moins un temps de travail doit être présent, et il ne peut pas y en avoir plus de cinq.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Définit une valeur indiquant si la date ou le type de jour spécifié est ouvrable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la date ou le type de jour spécifié est ouvré. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False indique que la plage de récurrence est définie en saisissant une date de fin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Définit le début de la période d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | le début du temps d'exception. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Définit le mois pour lequel une récurrence d'exception est planifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le mois pour lequel une récurrence d'exception est planifiée. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Définit le jour du mois auquel une récurrence d'exception est planifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le jour du mois auquel une récurrence d'exception est planifiée. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Définit l'élément de mois pour lequel une récurrence d'exception est planifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'élément de mois pour lequel une récurrence d'exception est planifiée. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Définit la position d'un élément de mois au sein d'un mois.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la position d'un élément de mois au sein d'un mois. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Définit le nom de l'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom de l'exception. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Définit le nombre d'occurrences pendant lesquelles l'exception de calendrier est valide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le nombre d'occurrences pour lesquelles l'exception de calendrier est valide. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Définit la période de récurrence de l'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la période de récurrence de l'exception. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Définit la fin de la période d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la fin du temps d'exception. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Définit le type d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type d'exception. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Définit l'objet WorkingTimeCollection. La collection des temps de travail qui définit le temps travaillé pendant le jour de la semaine.

--------------------

Au moins un temps de travail doit être présent, et il ne peut pas y en avoir plus de cinq.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | l'objet WorkingTimeCollection. |

