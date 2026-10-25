---
title: "Baslinje"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar baslinjevärden för en resurs."
type: docs
weight: 26
url: /sv/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Representerar baslinjevärden för en resurs.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implementering av IComparable‑gränssnittet. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getBaselineNumber()](#getBaselineNumber--) | Hämtar det unika numret för en baslinjedata post. |
| [getBcwp()](#getBcwp--) | Hämtar den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt till dags dato. |
| [getBcws()](#getBcws--) | Hämtar budgetkostnaden för ett arbete schemalagt för en resurs. |
| [getCost()](#getCost--) | Hämtar den beräknade kostnaden för en resurs när baslinjen sparas. |
| [getWork()](#getWork--) | Hämtar arbetet som tilldelats en resurs när baslinjen sparas. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för baslinjen. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är större än ett angivet objekt. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Ställer in det unika numret för en baslinjedata post. |
| [setBcwp(double value)](#setBcwp-double-) | Ställer in den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt till dags datum. |
| [setBcws(double value)](#setBcws-double-) | Ställer in budgetkostnaden för ett arbete schemalagt för en resurs. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Ställer in den beräknade kostnaden för en resurs när baslinjen sparas. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ställer in arbetet som tilldelats en resurs när baslinjen sparas. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implementering av IComparable‑gränssnittet. Jämför denna instans med det angivna Baseline‑objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | det angivna Baseline‑objektet att jämföra denna instans med. |

**Returns:**
int – returnerar -1 om denna instans är mindre än det angivna objektet, 1 om den är större än det angivna objektet; annars returneras 0.
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | det angivna objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna objektet; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | det angivna objektet att jämföra med denna instans. |

**Returns:**
boolean – returnerar true om denna instans är lika med det angivna objektet; annars false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Hämtar det unika numret för en baslinjedata post.

**Returns:**
int - det unika numret för en baslinjedata post.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Hämtar den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt till dags dato.

**Returns:**
double - den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt till dags datum.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Hämtar budgetkostnaden för ett arbete schemalagt för en resurs.

**Returns:**
double - budgetkostnaden för ett arbete schemalagt för en resurs.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Hämtar den beräknade kostnaden för en resurs när baslinjen sparas.

**Returns:**
java.math.BigDecimal - den beräknade kostnaden för en resurs när baslinjen sparas.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Hämtar arbetet som tilldelats en resurs när baslinjen sparas.

Värde: Mängden tilldelat arbete till en resurs när baslinjen sparades.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för baslinjen.

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är lika med ett specificerat objekt
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt är större än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än ett specificerat objekt
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än eller lika med ett specificerat objekt
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt inte är lika med ett specificerat objekt
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än ett specificerat objekt
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Den första baslinjen. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Den andra baslinjen. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än eller lika med ett specificerat objekt
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Ställer in det unika numret för en baslinjedata post.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | det unika numret för en baslinjedatapost. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Ställer in den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt till dags datum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | den budgeterade kostnaden för ett arbete utfört av en resurs för ett projekt hittills. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Ställer in budgetkostnaden för ett arbete schemalagt för en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | budgetkostnaden för ett arbete schemalagt för en resurs. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Ställer in den beräknade kostnaden för en resurs när baslinjen sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | den beräknade kostnaden för en resurs när baslinjen sparas. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ställer in arbetet som tilldelats en resurs när baslinjen sparas.

Värde: Mängden tilldelat arbete till en resurs när baslinjen sparades.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | arbetet som tilldelas en resurs när baslinjen sparas. |

