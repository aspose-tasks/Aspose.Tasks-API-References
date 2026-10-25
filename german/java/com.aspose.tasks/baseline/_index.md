---
title: "Basislinie"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Basiswerte einer Ressource dar."
type: docs
weight: 26
url: /de/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Stellt Basiswerte einer Ressource dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implementierung des IComparable-Interfaces. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getBaselineNumber()](#getBaselineNumber--) | Ruft die eindeutige Nummer eines Basisliniendatensatzes ab. |
| [getBcwp()](#getBcwp--) | Ruft die budgetierten Kosten einer von einer Ressource für ein Projekt bis zum heutigen Datum ausgeführten Arbeit ab. |
| [getBcws()](#getBcws--) | Ruft die Budgetkosten einer für eine Ressource geplanten Arbeit ab. |
| [getCost()](#getCost--) | Ruft die prognostizierten Kosten einer Ressource ab, wenn die Basislinie gespeichert wird. |
| [getWork()](#getWork--) | Ruft die einer Ressource zugewiesene Arbeit ab, wenn die Basislinie gespeichert wird. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Basislinie zurück. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Legt die eindeutige Nummer eines Basisliniendatensatzes fest. |
| [setBcwp(double value)](#setBcwp-double-) | Legt die budgetierten Kosten einer von einer Ressource für ein Projekt bis zum heutigen Datum ausgeführten Arbeit fest. |
| [setBcws(double value)](#setBcws-double-) | Legt die Budgetkosten einer für eine Ressource geplanten Arbeit fest. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Legt die prognostizierten Kosten einer Ressource fest, wenn die Basislinie gespeichert wird. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Legt die einem Ressourcen zugewiesene Arbeit fest, wenn die Basislinie gespeichert wird. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implementierung des IComparable-Interfaces. Vergleicht diese Instanz mit dem angegebenen Baseline-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | das angegebene Baseline-Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
int - gibt -1 zurück, wenn diese Instanz kleiner als das angegebene Objekt ist, 1 wenn sie größer ist; andernfalls wird 0 zurückgegeben.
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | das angegebene Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
boolean - gibt true zurück, wenn diese Instanz dem angegebenen Objekt gleich ist; andernfalls false.
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
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Ruft die eindeutige Nummer eines Basisliniendatensatzes ab.

**Returns:**
int - die eindeutige Nummer eines Basisliniendatensatzes.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Ruft die budgetierten Kosten einer von einer Ressource für ein Projekt bis zum heutigen Datum ausgeführten Arbeit ab.

**Returns:**
double - die budgetierten Kosten einer von einer Ressource für ein Projekt bis heute ausgeführten Arbeit.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Ruft die Budgetkosten einer für eine Ressource geplanten Arbeit ab.

**Returns:**
double - die Budgetkosten einer für eine Ressource geplanten Arbeit.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ruft die prognostizierten Kosten einer Ressource ab, wenn die Basislinie gespeichert wird.

**Returns:**
java.math.BigDecimal - die prognostizierten Kosten einer Ressource, wenn die Basislinie gespeichert wird.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ruft die einer Ressource zugewiesene Arbeit ab, wenn die Basislinie gespeichert wird.

Wert: Die Menge der einer Ressource zugewiesenen Arbeit, als die Basislinie gespeichert wurde.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Basislinie zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Die erste Basislinie. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Die zweite Basislinie. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Legt die eindeutige Nummer eines Basisliniendatensatzes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die eindeutige Nummer eines Basisliniendatensatzes. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Legt die budgetierten Kosten einer von einer Ressource für ein Projekt bis zum heutigen Datum ausgeführten Arbeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | die budgetierten Kosten einer von einer Ressource für ein Projekt bis heute ausgeführten Arbeit. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Legt die Budgetkosten einer für eine Ressource geplanten Arbeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | die Budgetkosten einer für eine Ressource geplanten Arbeit. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Legt die prognostizierten Kosten einer Ressource fest, wenn die Basislinie gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | die prognostizierten Kosten einer Ressource, wenn die Basislinie gespeichert wird. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Legt die einem Ressourcen zugewiesene Arbeit fest, wenn die Basislinie gespeichert wird.

Wert: Die Menge der einer Ressource zugewiesenen Arbeit, als die Basislinie gespeichert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | die einer Ressource zugewiesene Arbeit, wenn die Basislinie gespeichert wird. |

