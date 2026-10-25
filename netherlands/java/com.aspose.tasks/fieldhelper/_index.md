---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Helperklasse die nuttige bewerkingen met velden biedt."
type: docs
weight: 88
url: /nl/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Helperklasse die nuttige bewerkingen met velden biedt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Retourneert een standaardtitel van het specifieke veld. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Retourneert een standaardtitel van het specifieke taakveld. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Retourneert een standaardtitel van het specifieke veld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| veld | int | Veld om een standaardtitel op te halen. |

**Returns:**
java.lang.String - Een standaardtitel van het specifieke veld als het veld kan worden weergegeven in de weergave van MS Project, anders null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Retourneert een standaardtitel van het specifieke taakveld.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskKey | byte | Taakveld om een standaardtitel op te halen. |

**Returns:**
java.lang.String - Een standaardtitel van het specifieke taakveld als het veld kan worden weergegeven in de weergave van MS Project, anders null.
