---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Lesen von Primavera-Xml- oder Primavera-Xer-Dateien."
type: docs
weight: 206
url: /de/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Lesen von Primavera-Xml- oder Primavera-Xer-Dateien.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Initialisiert eine neue Instanz der [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Liefert ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten beibehalten werden sollen. |
| [getProjectUid()](#getProjectUid--) | Liefert die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Liefert ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen, die aus dem XER-Format gelesen wurden, zu verarbeiten. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Setzt ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten beibehalten werden sollen. |
| [setProjectUid(int value)](#setProjectUid-int-) | Setzt die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Setzt ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen, die aus dem XER-Format gelesen wurden, zu verarbeiten. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Initialisiert eine neue Instanz der [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) Klasse.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Liefert ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten beibehalten werden sollen.

**Returns:**
boolean - ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten beibehalten werden sollen.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Liefert die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll.

**Returns:**
int - die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Liefert ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen. Der Standardwert ist true.

--------------------

Das Flag gilt für Primavera-XML-Dateien, die Basislinienprojekte enthalten (Basislinien werden vom XER-Format nicht unterstützt). Die Option kann auf false gesetzt werden, um das Laden eines großen Projekts mit Basislinien zu beschleunigen, wenn Basisliniendaten nicht benötigt werden.

**Returns:**
boolean - ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen, die aus dem XER-Format gelesen wurden, zu verarbeiten.

**Returns:**
int - das Verhalten, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen, die aus dem XER-Format gelesen wurden, zu verarbeiten.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Setzt ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten beibehalten werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Flag, das angibt, ob die ursprünglichen eindeutigen Bezeichner von Entitäten erhalten bleiben sollen. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Setzt die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die UID eines Projekts, das aus einer Datei mit mehreren Projekten gelesen werden soll. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Setzt ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen. Der Standardwert ist true.

--------------------

Das Flag gilt für Primavera-XML-Dateien, die Basislinienprojekte enthalten (Basislinien werden vom XER-Format nicht unterstützt). Die Option kann auf false gesetzt werden, um das Laden eines großen Projekts mit Basislinien zu beschleunigen, wenn Basisliniendaten nicht benötigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Flag, das angibt, ob Basislinienprojekte geladen werden sollen. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Gibt das Verhalten an, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen, die aus dem XER-Format gelesen wurden, zu verarbeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Verhalten, das verwendet wird, um Aufgaben mit undefinierten Einschränkungen aus dem XER-Format zu verarbeiten. |

