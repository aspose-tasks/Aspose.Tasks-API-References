---
title: "ProjectServerSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen, wenn das Projekt auf Project Server oder Project Online gespeichert wird."
type: docs
weight: 227
url: /de/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen, wenn das Projekt auf Project Server oder Project Online gespeichert wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Initialisiert eine neue Instanz der Klasse [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Ermittelt das Intervall zwischen Anfragen zum Status von Warteschlangenjobs. |
| [getProjectGuid()](#getProjectGuid--) | Liefert die eindeutige Kennung eines Projekts. |
| [getProjectName()](#getProjectName--) | Liefert den Namen eines Projekts, der in der Projektliste von Project Server \\ Project Online angezeigt wird. |
| [getTimeout()](#getTimeout--) | Liefert das Timeout, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Legt das Intervall zwischen Anfragen zum Warteschlangen-Job-Status fest. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Legt die eindeutige Kennung eines Projekts fest. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Legt den Namen eines Projekts fest, der in der Projektliste von Project Server \\ Project Online angezeigt wird. |
| [setTimeout(double value)](#setTimeout-double-) | Legt das Timeout fest, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Initialisiert eine neue Instanz der Klasse [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Liefert das Intervall zwischen Anfragen zum Warteschlangen-Job-Status. Der Standardwert beträgt 2 Sekunden.

**Returns:**
double – Intervall zwischen Anfragen zum Warteschlangen-Job-Status.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Liefert die eindeutige Kennung eines Projekts. Sollte innerhalb einer Project Server \\ Project Online-Instanz eindeutig sein.

**Returns:**
java.util.UUID – eindeutige Kennung eines Projekts.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Liefert den Namen eines Projekts, der in der Projektliste von Project Server \\ Project Online angezeigt wird. Sollte innerhalb einer Project Server \\ Project Online-Instanz eindeutig sein. Wird der Wert weggelassen, wird stattdessen der Wert der Eigenschaft Prj.Name verwendet.

**Returns:**
java.lang.String – Name eines Projekts, das in der Projektliste von Project Server \\ Project Online angezeigt wird.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Liefert das Timeout, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird. Der Standardwert für diese Eigenschaft beträgt 1 Minute.

--------------------

Die Verarbeitungszeit kann bei großen Projekten oder wenn die Project Server-Instanz zu stark mit anderen Anfragen beschäftigt ist, länger sein.

**Returns:**
double – Timeout, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Legt das Intervall zwischen Anfragen zum Warteschlangen-Job-Status fest. Der Standardwert beträgt 2 Sekunden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Intervall zwischen Anfragen zum Warteschlangen-Job-Status. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Legt die eindeutige Kennung eines Projekts fest. Sollte innerhalb einer Project Server \\ Project Online-Instanz eindeutig sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID | Eindeutige Kennung eines Projekts. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Legt den Namen eines Projekts fest, der in der Projektliste von Project Server \\ Project Online angezeigt wird. Sollte innerhalb einer Project Server \\ Project Online-Instanz eindeutig sein. Wird der Wert weggelassen, wird stattdessen der Wert der Eigenschaft Prj.Name verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Name eines Projekts, das in der Projektliste von Project Server \\ Project Online angezeigt wird. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Legt das Timeout fest, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird. Der Standardwert für diese Eigenschaft beträgt 1 Minute.

--------------------

Die Verarbeitungszeit kann bei großen Projekten oder wenn die Project Server-Instanz zu stark mit anderen Anfragen beschäftigt ist, länger sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | Timeout, das beim Warten auf die Verarbeitung einer Speicherprojekt-Anforderung durch den Warteschlangenverarbeitungsdienst von Project Server verwendet wird. |

