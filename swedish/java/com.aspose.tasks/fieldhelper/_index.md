---
title: "FieldHelper"
second_title: "Aspose.Tasks for Java API-referens"
description: "Hjälparklass som tillhandahåller användbara operationer med fält."
type: docs
weight: 88
url: /sv/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Hjälparklass som tillhandahåller användbara operationer med fält.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Returnerar en standardtitel för det specifika fältet. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Returnerar en standardtitel för det specifika uppgiftsfältet. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Returnerar en standardtitel för det specifika fältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fält | int | Fält för att hämta en standardtitel. |

**Returns:**
java.lang.String - En standardtitel för det specifika fältet om fältet kan visas i MS Projects vy, annars null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Returnerar en standardtitel för det specifika uppgiftsfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| taskKey | byte | Uppgiftsfält för att hämta en standardtitel. |

**Returns:**
java.lang.String - En standardtitel för det specifika uppgiftsfältet om fältet kan visas i MS Projects vy, annars null.
