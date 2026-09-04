---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben von Parametern für die Ressourcen‑Ausgleichung."
type: docs
weight: 142
url: /de/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Ermöglicht das Angeben von Parametern für die Ressourcen‑Ausgleichung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Initialisiert eine neue Instanz der Klasse [LevelingOptions](../../com.aspose.tasks/levelingoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Ruft ein Token ab, das verwendet werden kann, um einen Projekt‑Leveling‑Vorgang abzubrechen. |
| [getFinishDate()](#getFinishDate--) | Ruft das Enddatum des Leveling‑Zeitraums ab. |
| [getLevelingOrder()](#getLevelingOrder--) | Ruft die Reihenfolge ab, in der der Leveling‑Algorithmus Aufgaben mit Überbelegungen verzögert. |
| [getMessageHandler()](#getMessageHandler--) | Ruft den Nachrichten‑Handler‑Callback ab, der verwendet werden kann, um Protokollnachrichten abzufangen, die von Aspose.Tasks während der Ressourcen‑Leveling erzeugt werden. |
| [getMessageLevel()](#getMessageLevel--) | Ruft das Protokollierungsniveau der von Aspose.Tasks während des Ressourcen‑Leveling ausgegebenen Nachrichten ab. |
| [getResources()](#getResources--) | Ruft die Liste der Ressourcen ab, die levelt werden. |
| [getStartDate()](#getStartDate--) | Ruft das Startdatum des Leveling‑Zeitraums ab. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Setzt ein Token, das verwendet werden kann, um einen Projekt‑Leveling‑Vorgang abzubrechen. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Setzt das Enddatum des Leveling‑Zeitraums. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | Die Reihenfolge, in der der Leveling‑Algorithmus Aufgaben mit Überbelegungen verzögert. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Setzt den Nachrichten‑Handler‑Callback, der verwendet werden kann, um Protokollnachrichten abzufangen, die von Aspose.Tasks während des Ressourcen‑Leveling erzeugt werden. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Setzt das Protokollierungsniveau der von Aspose.Tasks während des Ressourcen‑Leveling ausgegebenen Nachrichten. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Setzt die Liste der Ressourcen, die levelt werden. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Setzt das Startdatum des Leveling‑Zeitraums. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Initialisiert eine neue Instanz der Klasse [LevelingOptions](../../com.aspose.tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Ruft ein Token ab, das verwendet werden kann, um einen Projekt‑Leveling‑Vorgang abzubrechen.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Ruft das Enddatum des Leveling‑Zeitraums ab. Der Standardwert ist das Enddatum des Projekts.

**Returns:**
java.util.Date - Enddatum des Leveling‑Zeitraums.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Ermittelt die Reihenfolge, in der der Leveling‑Algorithmus Aufgaben mit Überbuchungen verzögert. Nach Bestimmung der Aufgaben, die die Überbuchung verursachen, und welcher Aufgaben verzögert werden können, wird die angegebene Reihenfolge verwendet, welche Aufgabe zuerst verzögert werden soll.

**Returns:**
int - die Reihenfolge, in der der Leveling‑Algorithmus Aufgaben mit Überbuchungen verzögert.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Ruft den Nachrichten‑Handler‑Callback ab, der verwendet werden kann, um Protokollnachrichten abzufangen, die von Aspose.Tasks während der Ressourcen‑Leveling erzeugt werden.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Ruft das Protokollierungsniveau der von Aspose.Tasks während des Ressourcen‑Leveling ausgegebenen Nachrichten ab.

**Returns:**
int - Ebene der von Aspose erzeugten Log‑Nachrichten.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Ermittelt die Liste der Ressourcen, die leveln werden. Wenn null gesetzt ist, werden alle Projektressourcen levelt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - die Liste der Ressourcen, die leveln werden.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Ermittelt das Startdatum des Leveling‑Zeitraums. Der Standardwert ist das Startdatum des project`s.

**Returns:**
java.util.Date - Startdatum des Leveling‑Zeitraums.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Setzt ein Token, das verwendet werden kann, um einen Projekt‑Leveling‑Vorgang abzubrechen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | Ein Token, das verwendet werden kann, um einen Projekt‑Leveling‑Vorgang abzubrechen. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Legt das Enddatum des Leveling‑Zeitraums fest. Der Standardwert ist das Enddatum des project`s.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | Enddatum des Leveling‑Zeitraums. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


Die Reihenfolge, in der der Leveling‑Algorithmus Aufgaben mit Überbuchungen verzögert. Nach Bestimmung der Aufgaben, die die Überbuchung verursachen, und welcher Aufgaben verzögert werden können, wird die angegebene Reihenfolge verwendet, welche Aufgabe zuerst verzögert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Reihenfolge, in der der Leveling‑Algorithmus Aufgaben mit Überbuchungen verzögert. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Setzt den Nachrichten‑Handler‑Callback, der verwendet werden kann, um Protokollnachrichten abzufangen, die von Aspose.Tasks während des Ressourcen‑Leveling erzeugt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | Message‑Handler‑Callback, der verwendet werden kann, um von Aspose erzeugte Log‑Nachrichten abzufangen. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Setzt das Protokollierungsniveau der von Aspose.Tasks während des Ressourcen‑Leveling ausgegebenen Nachrichten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Ebene der von Aspose erzeugten Log‑Nachrichten. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Legt die Liste der Ressourcen fest, die leveln werden. Wenn null gesetzt ist, werden alle Projektressourcen levelt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.List&lt;com.aspose.tasks.Resource&gt; | die Liste der Ressourcen, die leveln werden. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Legt das Startdatum des Leveling‑Zeitraums fest. Der Standardwert ist das Startdatum des project`s.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | Startdatum des Leveling‑Zeitraums. |

