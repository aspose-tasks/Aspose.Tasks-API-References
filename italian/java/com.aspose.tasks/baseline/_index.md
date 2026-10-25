---
title: "Linea di base"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta i valori di baseline di una risorsa."
type: docs
weight: 26
url: /it/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Rappresenta i valori di baseline di una risorsa.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implementazione dell'interfaccia IComparable. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getBaselineNumber()](#getBaselineNumber--) | Restituisce il numero univoco di un record dati baseline. |
| [getBcwp()](#getBcwp--) | Ottiene il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |
| [getBcws()](#getBcws--) | Ottiene il costo di budget di un lavoro programmato per una risorsa. |
| [getCost()](#getCost--) | Ottiene il costo previsto di una risorsa quando la baseline viene salvata. |
| [getWork()](#getWork--) | Ottiene il lavoro assegnato a una risorsa quando la baseline viene salvata. |
| [hashCode()](#hashCode--) | Restituisce un valore di hash code per la baseline. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Imposta il numero univoco di un record di dati della baseline. |
| [setBcwp(double value)](#setBcwp-double-) | Imposta il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |
| [setBcws(double value)](#setBcws-double-) | Imposta il costo di budget di un lavoro programmato per una risorsa. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Imposta il costo previsto di una risorsa quando la baseline viene salvata. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Imposta il lavoro assegnato a una risorsa quando la baseline viene salvata. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implementazione dell'interfaccia IComparable. Confronta questa istanza con l'oggetto Baseline specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | l'oggetto Baseline specificato con cui confrontare questa istanza. |

**Returns:**
int - restituisce -1 se questa istanza è inferiore all'oggetto specificato, 1 se questa istanza è superiore all'oggetto specificato; altrimenti restituisce 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | l'oggetto specificato da confrontare con questa istanza. |

**Returns:**
boolean - restituisce true se questa istanza è uguale all'oggetto specificato; altrimenti, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | l'oggetto specificato da confrontare con questa istanza. |

**Returns:**
boolean - restituisce true se questa istanza è uguale all'oggetto specificato; altrimenti, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Restituisce il numero univoco di un record dati baseline.

**Returns:**
int - il numero univoco di un record di dati della baseline.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Ottiene il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi.

**Returns:**
double - il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Ottiene il costo di budget di un lavoro programmato per una risorsa.

**Returns:**
double - il costo di budget di un lavoro programmato per una risorsa.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ottiene il costo previsto di una risorsa quando la baseline viene salvata.

**Returns:**
java.math.BigDecimal - il costo previsto di una risorsa quando la baseline viene salvata.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ottiene il lavoro assegnato a una risorsa quando la baseline viene salvata.

Valore: La quantità di lavoro assegnato a una risorsa quando la baseline è stata salvata.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di hash code per la baseline.

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza è uguale a un oggetto specificato
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore di un oggetto specificato
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza non è uguale a un oggetto specificato
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza è minore di un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza è minore di un oggetto specificato
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | La prima baseline. |
| b | [Baseline](../../com.aspose.tasks/baseline) | La seconda baseline. |

**Returns:**
boolean - un valore che indica se questa istanza è minore o uguale a un oggetto specificato
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Imposta il numero univoco di un record di dati della baseline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il numero univoco di un record di dati della baseline. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Imposta il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | il costo preventivato di un lavoro eseguito da una risorsa per un progetto fino ad oggi. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Imposta il costo di budget di un lavoro programmato per una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | il costo di budget di un lavoro programmato per una risorsa. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Imposta il costo previsto di una risorsa quando la baseline viene salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | il costo previsto di una risorsa quando la baseline viene salvata. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Imposta il lavoro assegnato a una risorsa quando la baseline viene salvata.

Valore: La quantità di lavoro assegnato a una risorsa quando la baseline è stata salvata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | il lavoro assegnato a una risorsa quando la baseline viene salvata. |

