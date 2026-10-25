---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API Reference"
description: "Hilfsklasse, die nützliche Operationen mit Feldern bereitstellt."
type: docs
weight: 88
url: /de/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Hilfsklasse, die nützliche Operationen mit Feldern bereitstellt.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Gibt einen Standardtitel des jeweiligen Feldes zurück. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Gibt einen Standardtitel des jeweiligen Aufgabenfeldes zurück. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Gibt einen Standardtitel des jeweiligen Feldes zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| field | int | Feld, um einen Standardtitel zu erhalten. |

**Returns:**
java.lang.String - Ein Standardtitel des jeweiligen Feldes, wenn das Feld in der Ansicht von MS Project angezeigt werden kann, andernfalls null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Gibt einen Standardtitel des jeweiligen Aufgabenfeldes zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| taskKey | byte | Aufgabenfeld, um einen Standardtitel zu erhalten. |

**Returns:**
java.lang.String - Ein Standardtitel des jeweiligen Aufgabenfeldes, wenn das Feld in der Ansicht von MS Project angezeigt werden kann, andernfalls null.
