---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Bevat een lijst van objecten."
type: docs
weight: 343
url: /nl/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Bevat een lijst van [View](../../com.aspose.tasks/view)-objecten. Breidt de `AbstractCollection`-klasse uit.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Voegt het opgegeven item toe aan deze collectie. |
| [clear()](#clear--) | Verwijdert alle items uit deze collectie. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Zoekt naar een View met de naam en retourneert de eerste vondst binnen de collectie. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Zoekt naar een View met de opgegeven Screen-eigenschap en retourneert de eerste vondst binnen de collectie. |
| [getParentProject()](#getParentProject--) | Haalt de ouder op van het View-object. |
| [iterator()](#iterator--) | Retourneert een iterator over de elementen die zich in deze collectie bevinden. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [size()](#size--) | Haalt het aantal elementen op dat in deze collectie zit. |
| [toList()](#toList--) | Converteert een view-collectie naar een lijst van [View](../../com.aspose.tasks/view)-objecten. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Voegt het opgegeven item toe aan deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | het opgegeven item om toe te voegen aan deze collectie. |

**Returns:**
boolean - true als de bewerking succesvol was.
### clear() {#clear--}
```
public final void clear()
```


Verwijdert alle items uit deze collectie.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | het opgegeven item om te vinden. |

**Returns:**
boolean - true als het opgegeven item in deze collectie wordt gevonden; anders false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | de opgegeven één-dimensionale array om elementen naar te kopiëren |
| arrayIndex | int | de nulgebaseerde index van de opgegeven array waarop het kopiëren begint. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Zoekt naar een View met de naam en retourneert de eerste vondst binnen de collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| viewName | java.lang.String | Naam van de View om te zoeken. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Zoekt naar een View met de opgegeven Screen-eigenschap en retourneert de eerste vondst binnen de collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen)-enumeratiewaarde. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt de ouder op van het View-object. Alleen-lezen [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Retourneert een iterator over de elementen die zich in deze collectie bevinden.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - collectie‑iterator.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Verwijdert de eerste instantie van een specifiek object uit deze collectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | het opgegeven object om te verwijderen. |

**Returns:**
boolean - true als het opgegeven object succesvol uit deze collectie is verwijderd; anders false.
### size() {#size--}
```
public final int size()
```


Haalt het aantal elementen op dat in deze collectie zit.

**Returns:**
int - het aantal elementen dat in deze collectie zit.
### toList() {#toList--}
```
public final List<View> toList()
```


Converteert een view-collectie naar een lijst van [View](../../com.aspose.tasks/view)-objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Generieke lijst van [View](../../com.aspose.tasks/view) objecten.
