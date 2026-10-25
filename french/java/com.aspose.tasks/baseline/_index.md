---
title: "Base de référence"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les valeurs de référence d'une ressource."
type: docs
weight: 26
url: /fr/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Représente les valeurs de référence d'une ressource.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implémentation de l'interface IComparable. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getBaselineNumber()](#getBaselineNumber--) | Obtient le numéro unique d'un enregistrement de données de base de référence. |
| [getBcwp()](#getBcwp--) | Obtient le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |
| [getBcws()](#getBcws--) | Obtient le coût budgétaire d'un travail planifié pour une ressource. |
| [getCost()](#getCost--) | Obtient le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |
| [getWork()](#getWork--) | Obtient le travail assigné à une ressource lorsque la ligne de base est enregistrée. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour la ligne de base. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Définit le numéro unique d'un enregistrement de données de ligne de base. |
| [setBcwp(double value)](#setBcwp-double-) | Définit le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |
| [setBcws(double value)](#setBcws-double-) | Définit le coût budgétaire d'un travail planifié pour une ressource. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Définit le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Définit le travail assigné à une ressource lorsque la ligne de base est enregistrée. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implémentation de l'interface IComparable. Compare cette instance à l'objet Baseline spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | l'objet Baseline spécifié avec lequel comparer cette instance. |

**Returns:**
int - renvoie -1 si cette instance est inférieure à l'objet spécifié, 1 si cette instance est supérieure à l'objet spécifié ; sinon renvoie 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | l'objet spécifié à comparer avec cette instance. |

**Returns:**
boolean - renvoie true si cette instance est égale à l'objet spécifié ; sinon, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | l'objet spécifié à comparer avec cette instance. |

**Returns:**
boolean - renvoie true si cette instance est égale à l'objet spécifié ; sinon, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Obtient le numéro unique d'un enregistrement de données de base de référence.

**Returns:**
int - le numéro unique d'un enregistrement de données de ligne de base.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Obtient le coût budgété d'un travail effectué par une ressource pour un projet à ce jour.

**Returns:**
double - le coût budgété d'un travail effectué par une ressource pour un projet à ce jour.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Obtient le coût budgétaire d'un travail planifié pour une ressource.

**Returns:**
double - le coût budgétaire d'un travail planifié pour une ressource.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtient le coût projeté d'une ressource lorsque la ligne de base est enregistrée.

**Returns:**
java.math.BigDecimal - le coût projeté d'une ressource lorsque la ligne de base est enregistrée.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtient le travail assigné à une ressource lorsque la ligne de base est enregistrée.

Valeur : Le montant du travail assigné à une ressource lorsque la ligne de base a été enregistrée.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour la ligne de base.

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance est égale à un objet spécifié
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure à un objet spécifié
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance n'est pas égale à un objet spécifié
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure à un objet spécifié
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La première ligne de base. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La deuxième ligne de base. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Définit le numéro unique d'un enregistrement de données de ligne de base.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le numéro unique d'un enregistrement de données de ligne de base. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Définit le coût budgété d'un travail effectué par une ressource pour un projet à ce jour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | le coût budgété d'un travail effectué par une ressource pour un projet à ce jour. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Définit le coût budgétaire d'un travail planifié pour une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | le coût budgétaire d'un travail planifié pour une ressource. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Définit le coût projeté d'une ressource lorsque la ligne de base est enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | le coût projeté d'une ressource lorsque la ligne de base est enregistrée. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Définit le travail assigné à une ressource lorsque la ligne de base est enregistrée.

Valeur : Le montant du travail assigné à une ressource lorsque la ligne de base a été enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | le travail assigné à une ressource lorsque la ligne de base est enregistrée. |

