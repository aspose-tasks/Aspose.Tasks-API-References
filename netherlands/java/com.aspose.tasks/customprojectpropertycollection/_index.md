---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een verzameling van aangepaste projecteigenschappen."
type: docs
weight: 61
url: /nl/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Vertegenwoordigt een verzameling van aangepaste projecteigenschappen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Initialiseert een nieuw exemplaar van de [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Maakt een nieuwe aangepaste eigenschap aan. |
| [add(String name, double value)](#add-java.lang.String-double-) | Maakt een nieuwe aangepaste eigenschap aan. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Maakt een nieuwe aangepaste eigenschap aan. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Maakt een nieuwe aangepaste eigenschap aan. |
| [clear()](#clear--) | Leegt de PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders false. |
| [remove(String name)](#remove-java.lang.String-) | Verwijdert een eigenschap met de opgegeven naam uit de collectie. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Initialiseert een nieuw exemplaar van de [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) klasse.

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Maakt een nieuwe aangepaste eigenschap aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van de eigenschap. |
| waarde | boolean | De nieuw aangemaakte waarde van het property-object. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Maakt een nieuwe aangepaste eigenschap aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van de eigenschap. |
| waarde | double | De nieuw aangemaakte waarde van het property-object. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Maakt een nieuwe aangepaste eigenschap aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van de eigenschap. |
| waarde | java.lang.String | De nieuw aangemaakte waarde van het property-object. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Maakt een nieuwe aangepaste eigenschap aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van de eigenschap. |
| waarde | java.util.Date | De nieuw aangemaakte waarde van het property-object. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Leegt de PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders false.

**Returns:**
boolean - een waarde die aangeeft of deze collectie alleen-lezen is; anders false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Verwijdert een eigenschap met de opgegeven naam uit de collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De hoofdletterongevoelige naam van de property. |

**Returns:**
boolean - True als het element succesvol is gevonden en verwijderd; anders false.
