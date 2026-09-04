---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts im Primavera-XER-Format."
type: docs
weight: 208
url: /de/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts im Primavera-XER-Format.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Initialisiert eine neue Instanz der Klasse [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Gibt das Inkrement zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Gibt das Präfix zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Gibt das Suffix zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Gibt einen Wert zurück, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Gibt einen Wert zurück, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Setzt das Inkrement, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Setzt das Präfix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Setzt das Suffix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Setzt einen Wert, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Setzt einen Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Gibt das Inkrement zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Returns:**
int - das Inkrement, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Gibt das Präfix zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Returns:**
java.lang.String - das Präfix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Gibt das Suffix zurück, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Returns:**
int - das Suffix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Gibt einen Wert zurück, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist.

**Returns:**
boolean - ein Wert, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Gibt einen Wert zurück, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.

Die Primavera-Software unterstützt keine Zuweisungen von Ressourcen zu Zusammenfassungs‑ (WBS‑) Aufgaben. Daher kann der Export solcher Zuweisungen zu einer ungültigen Datei gemäß dem Primavera‑Modell führen. Wenn true, werden Zuweisungen zu Zusammenfassungsaufgaben beim Export übersprungen. Wenn false (der Standardwert), wird eine Ausnahme ausgelöst, wenn beim Export eine Zuweisung zu einer Zusammenfassungsaufgabe gefunden wird.

**Returns:**
boolean – ein Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Setzt das Inkrement, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Inkrement, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Setzt das Präfix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | das Präfix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Setzt das Suffix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Suffix, das bei der Neunummerierung von Aktivitäts-IDs verwendet wird. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Setzt einen Wert, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob die Neunummerierung von Aktivitäts-IDs erforderlich ist. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Setzt einen Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.

Die Primavera-Software unterstützt keine Zuweisungen von Ressourcen zu Zusammenfassungs‑ (WBS‑) Aufgaben. Daher kann der Export solcher Zuweisungen zu einer ungültigen Datei gemäß dem Primavera‑Modell führen. Wenn true, werden Zuweisungen zu Zusammenfassungsaufgaben beim Export übersprungen. Wenn false (der Standardwert), wird eine Ausnahme ausgelöst, wenn beim Export eine Zuweisung zu einer Zusammenfassungsaufgabe gefunden wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen. |

