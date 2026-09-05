---
title: "Basislijn"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt baseline-waarden van een resource voor."
type: docs
weight: 26
url: /nl/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Stelt baseline-waarden van een resource voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable interface-implementatie. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getBaselineNumber()](#getBaselineNumber--) | Haalt het unieke nummer van een basislijngegevensrecord op. |
| [getBcwp()](#getBcwp--) | Haalt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe op. |
| [getBcws()](#getBcws--) | Haalt de begrote kosten van een voor een resource gepland werk op. |
| [getCost()](#getCost--) | Haalt de geprojecteerde kosten van een resource op wanneer de basislijn wordt opgeslagen. |
| [getWork()](#getWork--) | Haalt het aan een resource toegewezen werk op wanneer de basislijn wordt opgeslagen. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor de basislijn. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Stelt het unieke nummer van een basislijngegevensrecord in. |
| [setBcwp(double value)](#setBcwp-double-) | Stelt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe in. |
| [setBcws(double value)](#setBcws-double-) | Stelt de begrote kosten van een voor een resource gepland werk in. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Stelt de geprojecteerde kosten van een resource in wanneer de basislijn wordt opgeslagen. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Stelt het aan een resource toegewezen werk in wanneer de basislijn wordt opgeslagen. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable interface-implementatie. Vergelijkt deze instantie met het opgegeven Baseline-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | het opgegeven Baseline-object om deze instantie mee te vergelijken. |

**Returns:**
int - retourneert -1 als deze instantie kleiner is dan het opgegeven object, 1 als deze instantie groter is dan het opgegeven object; retourneert anders 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | het opgegeven object om te vergelijken met deze instantie. |

**Returns:**
boolean - retourneert true als deze instantie gelijk is aan het opgegeven object; anders false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | het opgegeven object om te vergelijken met deze instantie. |

**Returns:**
boolean - retourneert true als deze instantie gelijk is aan het opgegeven object; anders false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Haalt het unieke nummer van een basislijngegevensrecord op.

**Returns:**
int - het unieke nummer van een basislijngegevensrecord.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Haalt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe op.

**Returns:**
double - de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Haalt de begrote kosten van een voor een resource gepland werk op.

**Returns:**
double - de begrote kosten van een voor een resource gepland werk.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Haalt de geprojecteerde kosten van een resource op wanneer de basislijn wordt opgeslagen.

**Returns:**
java.math.BigDecimal - de geprojecteerde kosten van een resource wanneer de basislijn wordt opgeslagen.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Haalt het aan een resource toegewezen werk op wanneer de basislijn wordt opgeslagen.

Waarde: De hoeveelheid toegewezen werk aan een resource toen de basislijn werd opgeslagen.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor de basislijn.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter is dan een opgegeven object
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | De eerste basislijn. |
| b | [Baseline](../../com.aspose.tasks/baseline) | De tweede basislijn. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Stelt het unieke nummer van een basislijngegevensrecord in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het unieke nummer van een basislijngegevensrecord. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Stelt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Stelt de begrote kosten van een voor een resource gepland werk in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | de begrote kosten van een voor een resource gepland werk. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Stelt de geprojecteerde kosten van een resource in wanneer de basislijn wordt opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | de geprojecteerde kosten van een resource wanneer de basislijn wordt opgeslagen. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Stelt het aan een resource toegewezen werk in wanneer de basislijn wordt opgeslagen.

Waarde: De hoeveelheid toegewezen werk aan een resource toen de basislijn werd opgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | het aan een resource toegewezen werk wanneer de basislijn wordt opgeslagen. |

