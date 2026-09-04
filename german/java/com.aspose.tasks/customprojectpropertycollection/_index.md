---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung benutzerdefinierter Projekteigenschaften dar."
type: docs
weight: 61
url: /de/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Stellt eine Sammlung benutzerdefinierter Projekteigenschaften dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Initialisiert eine neue Instanz der [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Erstellt eine neue benutzerdefinierte Eigenschaft. |
| [add(String name, double value)](#add-java.lang.String-double-) | Erstellt eine neue benutzerdefinierte Eigenschaft. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Erstellt eine neue benutzerdefinierte Eigenschaft. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Erstellt eine neue benutzerdefinierte Eigenschaft. |
| [clear()](#clear--) | Löscht die PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Ruft einen Wert ab, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false. |
| [remove(String name)](#remove-java.lang.String-) | Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Initialisiert eine neue Instanz der [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) Klasse.

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Erstellt eine neue benutzerdefinierte Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name der Eigenschaft. |
| Wert | boolean | Der neu erstellte Eigenschaftsobjektwert. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Erstellt eine neue benutzerdefinierte Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name der Eigenschaft. |
| Wert | double | Der neu erstellte Eigenschaftsobjektwert. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Erstellt eine neue benutzerdefinierte Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name der Eigenschaft. |
| Wert | java.lang.String | Der neu erstellte Eigenschaftsobjektwert. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Erstellt eine neue benutzerdefinierte Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name der Eigenschaft. |
| Wert | java.util.Date | Der neu erstellte Eigenschaftsobjektwert. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Löscht die PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Ruft einen Wert ab, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false.

**Returns:**
boolean - ein Wert, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der case‑insensitive Name der Eigenschaft. |

**Returns:**
boolescher Wert – True, wenn das Element erfolgreich gefunden und entfernt wurde; andernfalls false.
