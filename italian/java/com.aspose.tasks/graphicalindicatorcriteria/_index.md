---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un criterio di indicatore grafico associato a un attributo esteso."
type: docs
weight: 115
url: /it/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Rappresenta un criterio di indicatore grafico associato a un attributo esteso.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Inizializza una nuova istanza del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Inizializza una nuova istanza del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Restituisce l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri. |
| [getRowType()](#getRowType--) | Restituisce il valore dell'enumerazione [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) che indica per quali righe viene applicato l'indicatore. |
| [getTest()](#getTest--) | Restituisce il tipo di confronto effettuato tra il valore dell'attributo esteso e i Valori che fungono da criterio per l'applicazione dell'indicatore grafico. |
| [getValue1()](#getValue1--) | Restituisce il valore utilizzato per testare il valore dell'attributo esteso. |
| [getValue2()](#getValue2--) | Restituisce il secondo valore utilizzato per testare il valore dell'attributo esteso nel caso dei tipi di confronto 'IsWithin' e 'IsNotWithin'. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa dell'istanza della classe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Inizializza una nuova istanza del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowType | int | valore dell'enumerazione [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) che indica per quali righe viene applicato l'indicatore |
| test | int | valore di [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) che indica il tipo di confronto eseguito dal criterio. |
| imageIndex | int | l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valori utilizzati nella verifica della condizione. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | secondo valore (fine dell'intervallo) utilizzato nella verifica della condizione nel caso delle condizioni 'IsWithin' e 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Inizializza una nuova istanza del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowType | int | valore dell'enumerazione [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) che indica per quali righe viene applicato l'indicatore |
| test | int | valore di [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) che indica il tipo di confronto eseguito dal criterio. |
| imageIndex | int | l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valore utilizzato nella verifica della condizione. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Restituisce l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri.

**Returns:**
int - l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Restituisce il valore dell'enumerazione [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) che indica per quali righe viene applicato l'indicatore.

**Returns:**
int - il valore dell'enumerazione [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) che indica per quali righe viene applicato l'indicatore.
### getTest() {#getTest--}
```
public final int getTest()
```


Restituisce il tipo di confronto effettuato tra il valore dell'attributo esteso e i Valori che fungono da criterio per l'applicazione dell'indicatore grafico. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - il tipo di confronto effettuato tra il valore dell'attributo esteso e i Valori che fungono da criterio per l'applicazione dell'indicatore grafico.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Restituisce il valore utilizzato per testare il valore dell'attributo esteso.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Restituisce il secondo valore utilizzato per testare il valore dell'attributo esteso nel caso dei tipi di confronto 'IsWithin' e 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione stringa dell'istanza della classe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - rappresentazione stringa di questo oggetto.
