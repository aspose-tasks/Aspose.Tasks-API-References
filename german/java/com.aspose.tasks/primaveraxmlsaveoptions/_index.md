---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts im Primavera-Xml-Format."
type: docs
weight: 212
url: /de/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Speichern eines Projekts im Primavera-Xml-Format.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Initialisiert eine neue Instanz der Klasse [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Gibt einen Wert zurück, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Gibt einen Wert zurück, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Setzt einen Wert, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Setzt einen Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Gibt einen Wert zurück, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht.

**Returns:**
boolean – ein Wert, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Gibt einen Wert zurück, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.

Die Primavera-Software unterstützt keine Zuweisungen von Ressourcen zu Zusammenfassungs‑ (WBS‑) Aufgaben. Daher kann der Export solcher Zuweisungen zu einer ungültigen Datei gemäß dem Primavera‑Modell führen. Wenn true, werden Zuweisungen zu Zusammenfassungsaufgaben beim Export übersprungen. Wenn false (der Standardwert), wird eine Ausnahme ausgelöst, wenn beim Export eine Zuweisung zu einer Zusammenfassungsaufgabe gefunden wird.

**Returns:**
boolean – ein Wert, der angibt, ob Zuweisungen von Ressourcen zu Zusammenfassungsaufgaben beim Export übersprungen werden sollen.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Setzt einen Wert, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob eine Stammaufgabe gespeichert werden soll oder nicht. |

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

