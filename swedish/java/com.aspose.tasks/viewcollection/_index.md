---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Innehåller en lista med  objekt."
type: docs
weight: 343
url: /sv/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Innehåller en lista med [View](../../com.aspose.tasks/view)-objekt. Ärver `AbstractCollection`-klassen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Lägger till det angivna objektet i denna samling. |
| [clear()](#clear--) | Tar bort alla objekt från denna samling. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Returnerar true om det angivna objektet hittas i denna samling; annars false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Kopierar elementen i denna samling till den angivna arrayen, med start vid det angivna arrayindexet. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Söker efter en View med namnet och returnerar den första förekomsten i samlingen. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Söker efter en View med den angivna Screen-egenskapen och returnerar den första förekomsten i samlingen. |
| [getParentProject()](#getParentProject--) | Hämtar föräldern till View-objektet. |
| [iterator()](#iterator--) | Returnerar en iterator över elementen som finns i denna samling. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Tar bort den första förekomsten av ett specifikt objekt från denna samling. |
| [size()](#size--) | Hämtar antalet element som finns i denna samling. |
| [toList()](#toList--) | Konverterar en view-samling till en lista med [View](../../com.aspose.tasks/view)-objekt. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Lägger till det angivna objektet i denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | det angivna objektet att lägga till i denna samling. |

**Returns:**
boolean - true om operationen lyckades.
### clear() {#clear--}
```
public final void clear()
```


Tar bort alla objekt från denna samling.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Returnerar true om det angivna objektet hittas i denna samling; annars false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | det angivna objektet att hitta. |

**Returns:**
boolean - true om det angivna objektet hittas i denna samling; annars false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Kopierar elementen i denna samling till den angivna arrayen, med start vid det angivna arrayindexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | den angivna endimensionella arrayen att kopiera element till |
| arrayIndex | int | det nollbaserade indexet för den angivna arrayen där kopieringen börjar. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Söker efter en View med namnet och returnerar den första förekomsten i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| viewName | java.lang.String | Namnet på den View som ska sökas. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Söker efter en View med den angivna Screen-egenskapen och returnerar den första förekomsten i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) enumerationsvärde. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldern till View-objektet. Skrivskyddad [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Returnerar en iterator över elementen som finns i denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - samlings-iterator.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Tar bort den första förekomsten av ett specifikt objekt från denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | det angivna objektet att ta bort. |

**Returns:**
boolean - true om det angivna objektet framgångsrikt togs bort från denna samling; annars false.
### size() {#size--}
```
public final int size()
```


Hämtar antalet element som finns i denna samling.

**Returns:**
int - antalet element som finns i denna samling.
### toList() {#toList--}
```
public final List<View> toList()
```


Konverterar en view-samling till en lista med [View](../../com.aspose.tasks/view)-objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Generisk lista med [View](../../com.aspose.tasks/view)-objekt.
