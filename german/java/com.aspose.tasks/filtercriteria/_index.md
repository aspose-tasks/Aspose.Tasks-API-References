---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definiert die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden."
type: docs
weight: 94
url: /de/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Definiert die Kriterien, die Aufgaben oder Ressourcen erfüllen müssen, um in der MSP-Ansicht angezeigt zu werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Ruft die Liste der untergeordneten [FilterCriteria](../../com.aspose.tasks/filtercriteria) Zeilen ab. |
| [getField()](#getField--) | Ruft ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern ab. |
| [getOperation()](#getOperation--) | Ruft das Kriterium ab, das mit FieldName, Test und Value festgelegt wurde und sich auf andere Kriterien im Filter bezieht. |
| [getTest()](#getTest--) | Ruft den Vergleichstyp ab, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient. |
| [getValues()](#getValues--) | Ruft die Objektwerte ab, die mit dem Wert des mit FieldName angegebenen Feldes verglichen werden. |
| [isValueAField()](#isValueAField--) | Ruft ab, ob der rechte Wert von FilterCriteria eine Feldreferenz und kein konstanter Wert ist. |
| [isValueAField(int index)](#isValueAField-int-) | Ruft ab, ob der Wert am Index von FilterCriteria eine Feldreferenz und kein konstanter Wert ist. |
| [setField(int value)](#setField-int-) | Setzt ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern. |
| [setOperation(int value)](#setOperation-int-) | Legt das mit FieldName, Test und Value festgelegte Kriterium fest, das sich auf andere Kriterien im Filter bezieht. |
| [setTest(int value)](#setTest-int-) | Legt den Vergleichstyp fest, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Legt den Objektwert am Index fest, der mit dem Wert des durch FieldName angegebenen Feldes verglichen wird. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Legt den Objektwert fest, der mit dem Wert des durch FieldName angegebenen Feldes verglichen wird. |
| [setValueByField(int value)](#setValueByField-int-) | Legt das Feld fest, dessen Wert mit dem Wert des durch FieldName angegebenen Feldes verglichen wird. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Legt das Feld am Index fest, dessen Wert mit dem Wert des durch FieldName angegebenen Feldes verglichen wird. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [FilterCriteria](../../com.aspose.tasks/filtercriteria) zurück. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Ruft die Liste der untergeordneten Zeilen von [FilterCriteria](../../com.aspose.tasks/filtercriteria) ab. Enthält der Filter mehr als eine Kriterienzeile, bewirkt ein And‑Operator, dass die Kriterien beider Zeilen erfüllt sein müssen, damit die Aufgabe oder Ressource als Ergebnis dieses Filters angezeigt wird. Ein Or‑Operator bewirkt, dass die Kriterien der einen oder der anderen Zeile erfüllt sein müssen.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; – die Liste der untergeordneten Zeilen von [FilterCriteria](../../com.aspose.tasks/filtercriteria).
### getField() {#getField--}
```
public final int getField()
```


Ruft ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern ab.

**Returns:**
int – ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Ruft das Kriterium ab, das mit FieldName, Test und Value festgelegt wurde und sich auf andere Kriterien im Filter bezieht.

**Returns:**
int – das mit FieldName, Test und Value festgelegte Kriterium bezieht sich auf andere Kriterien im Filter.
### getTest() {#getTest--}
```
public final int getTest()
```


Ruft den Vergleichstyp ab, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int – der Vergleichstyp, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Ruft die Objektwerte ab, die mit dem Wert des mit FieldName angegebenen Feldes verglichen werden.

**Returns:**
java.lang.Object[] – die Objektwerte, die mit dem Wert des durch FieldName angegebenen Feldes verglichen werden.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Ruft ab, ob der rechte Wert von FilterCriteria eine Feldreferenz und kein konstanter Wert ist.

**Returns:**
boolean – ob der rechte Wert von FilterCriteria eine Feldreferenz und kein konstanter Wert ist.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Ruft ab, ob der Wert am Index von FilterCriteria eine Feldreferenz und kein konstanter Wert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des Wertes |

**Returns:**
boolean – ob der rechte Wert am Index von FilterCriteria eine Feldreferenz und kein konstanter Wert ist.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Setzt ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | int | ein `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) zum Ändern. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Legt das mit FieldName, Test und Value festgelegte Kriterium fest, das sich auf andere Kriterien im Filter bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das mit FieldName, Test und Value festgelegte Kriterium bezieht sich auf andere Kriterien im Filter. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Legt den Vergleichstyp fest, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Vergleichstyp, der zwischen FieldName und Value durchgeführt wird und als Auswahlkriterium für den Filter dient. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Legt den Objektwert am Index fest, der mit dem Wert des durch FieldName angegebenen Feldes verglichen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des Wertes. |
| Wert | java.lang.Object | Objektwert, der als rechter Wert am Index der Filterkriterien dient. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Legt den Objektwert fest, der mit dem Wert des durch FieldName angegebenen Feldes verglichen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Objektwert, der als rechter Wert der Filterkriterien dient. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Legt das Feld fest, dessen Wert mit dem Wert des durch FieldName angegebenen Feldes verglichen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Feld, das als rechter Wert der Filterkriterien dient. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Legt das Feld am Index fest, dessen Wert mit dem Wert des durch FieldName angegebenen Feldes verglichen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | der Index des Wertes |
| Wert | int | Feld, das am Index der Filterkriterien als Rechtswert dient. |

### toString() {#toString--}
```
public String toString()
```


Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [FilterCriteria](../../com.aspose.tasks/filtercriteria) zurück.

**Returns:**
java.lang.String - Zeichenkettenrepräsentation dieses Objekts.
