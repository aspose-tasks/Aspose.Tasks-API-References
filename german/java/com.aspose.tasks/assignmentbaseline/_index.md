---
title: "AssignmentBaseline"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt die Basislinie einer Ressourcenzuweisung dar."
type: docs
weight: 17
url: /de/java/com.aspose.tasks/assignmentbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)
```
public class AssignmentBaseline extends Baseline
```

Stellt die Basislinie einer Ressourcenzuweisung dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AssignmentBaseline()](#AssignmentBaseline--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(AssignmentBaseline other)](#compareTo-com.aspose.tasks.AssignmentBaseline-) | Implementierung des IComparable-Interfaces. |
| [equals(AssignmentBaseline other)](#equals-com.aspose.tasks.AssignmentBaseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getFinish()](#getFinish--) | Ermittelt das geplante Enddatum der Ressourcen-Zuweisung, als die Basislinie gespeichert wurde. |
| [getStart()](#getStart--) | Ermittelt das geplante Startdatum der Ressourcen-Zuweisung, als die Basislinie gespeichert wurde. |
| [getTimephasedData()](#getTimephasedData--) | Ermittelt die Instanz von [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für diese AssignmentBaseline zurück. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Legt das geplante Enddatum der Ressourcen-Zuweisung fest, als die Basislinie gespeichert wurde. |
| [setStart(Date value)](#setStart-java.util.Date-) | Legt das geplante Startdatum der Ressourcen-Zuweisung fest, als die Basislinie gespeichert wurde. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Setzt die Instanz von [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt. |
### AssignmentBaseline() {#AssignmentBaseline--}
```
public AssignmentBaseline()
```


### compareTo(AssignmentBaseline other) {#compareTo-com.aspose.tasks.AssignmentBaseline-}
```
public final int compareTo(AssignmentBaseline other)
```


Implementierung des IComparable-Interfaces. Vergleicht diese Instanz mit dem angegebenen Baseline-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | das angegebene Baseline-Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
int - gibt -1 zurück, wenn diese Instanz kleiner als das angegebene Objekt ist, 1 wenn sie größer ist; andernfalls wird 0 zurückgegeben.
### equals(AssignmentBaseline other) {#equals-com.aspose.tasks.AssignmentBaseline-}
```
public final boolean equals(AssignmentBaseline other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [AssignmentBaseline](../../com.aspose.tasks/assignmentbaseline) | das angegebene AssignmentBaseline-Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen AssignmentBaseline-Objekt gleich ist; andernfalls false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | das angegebene Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen Objekt gleich ist; andernfalls false.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ermittelt das geplante Enddatum der Ressourcen-Zuweisung, als die Basislinie gespeichert wurde.

Wert: Das Enddatum der Ressourcenzuweisung, als diese Basislinie gespeichert wurde.

**Returns:**
java.util.Date - das geplante Enddatum der Ressourcenzuweisung, als die Basislinie gespeichert wurde.
### getStart() {#getStart--}
```
public final Date getStart()
```


Ermittelt das geplante Startdatum der Ressourcen-Zuweisung, als die Basislinie gespeichert wurde.

Wert: Das Startdatum der Ressourcenzuweisung, als diese Basislinie gespeichert wurde.

**Returns:**
java.util.Date - das geplante Startdatum der Ressourcenzuweisung, als die Basislinie gespeichert wurde.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Liefert die [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Instanz für dieses Objekt. Die zeitlich gestaffelten Daten, die mit der Ressourcenzuweisungs-Basislinie verknüpft sind.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) instance for this object. Value: The collection of Time phased data associated with this baseline.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für diese AssignmentBaseline zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Legt das geplante Enddatum der Ressourcen-Zuweisung fest, als die Basislinie gespeichert wurde.

Wert: Das Enddatum der Ressourcenzuweisung, als diese Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das geplante Enddatum der Ressourcenzuweisung, als die Basislinie gespeichert wurde. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Legt das geplante Startdatum der Ressourcen-Zuweisung fest, als die Basislinie gespeichert wurde.

Wert: Das Startdatum der Ressourcenzuweisung, als diese Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das geplante Startdatum der Ressourcenzuweisung, als die Basislinie gespeichert wurde. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Setzt die [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Instanz für dieses Objekt. Die zeitlich gestaffelten Daten, die mit der Ressourcenzuweisungs-Basislinie verknüpft sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | die [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Instanz für dieses Objekt. |

