---
title: "View"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en vy i Project."
type: docs
weight: 342
url: /sv/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Representerar en vy i Project.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [View()](#View--) | Initierar en ny instans av klassen [View](../../com.aspose.tasks/view). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Jämför den aktuella instansen med ett annat objekt av samma typ och returnerar ett heltal som indikerar om den aktuella instansen föregår, följer eller ligger på samma position i sorteringsordningen som det andra objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Skapar en ny instans av klassen [View](../../com.aspose.tasks/view). |
| [getFilter()](#getFilter--) | Hämtar ett filter som används i en enskild vy. |
| [getGroup()](#getGroup--) | Hämtar en grupp av den enkla vyn. |
| [getHighlightFilter()](#getHighlightFilter--) | Hämtar ett värde som indikerar om Microsoft Project markerar filtret för en enkel vy. |
| [getName()](#getName--) | Hämtar namnet på ett View-objekt. |
| [getPageInfo()](#getPageInfo--) | Hämtar en instans av klassen `PageInfo`([getPageInfo()](../../com.aspose/tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Hämtar föräldern till View-objektet. |
| [getScreen()](#getScreen--) | Hämtar skärmtypen för den enkla vyn. |
| [getShowInMenu()](#getShowInMenu--) | Hämtar ett värde som indikerar om Microsoft Project visar namnet på den enkla vyn i View eller Other Views‑rullgardinslistorna i Ribbon. |
| [getTable()](#getTable--) | Hämtar en tabell för den enkla vyn. |
| [getType()](#getType--) | Hämtar typen av objekt i den enkla vyn, till exempel uppgifter eller resurser. |
| [getUid()](#getUid--) | Hämtar den unika identifieraren för en vy. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Hämtar en samling av objekt som representerar placering och utseende av [OleObject](../../com.aspose/tasks/oleobject) i vyn. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av klassen [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt är större än ett angivet objekt. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Ställer in ett filter som används i en enkel vy. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Ställer in en grupp för den enkla vyn. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Ställer in ett värde som indikerar om Microsoft Project markerar filtret för en enkel vy. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på ett View-objekt. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Ställer in ett värde som indikerar om Microsoft Project visar namnet på den enkla vyn i View eller Other Views‑rullgardinslistorna i Ribbon. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Ställer in en tabell för den enkla vyn. |
### View() {#View--}
```
public View()
```


Initierar en ny instans av klassen [View](../../com.aspose.tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Jämför den aktuella instansen med ett annat objekt av samma typ och returnerar ett heltal som indikerar om den aktuella instansen föregår, följer eller ligger på samma position i sorteringsordningen som det andra objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | det angivna View-objektet att jämföra denna instans med. |

**Returns:**
int - En 32-bitars signerat heltal som indikerar den relativa ordningen för de objekt som jämförs. Returvärdet har följande betydelser: Värde Betydelse Mindre än noll Denna instans föregår `other` i sorteringsordningen. Noll Denna instans har samma position i sorteringsordningen som `other`. Större än noll Denna instans följer `other` i sorteringsordningen.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolean - **True** om det angivna objektet är en View som har samma Uid‑värde som denna instans; annars **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Skapar en ny instans av klassen [View](../../com.aspose.tasks/view).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| viewScreen | int | Skärmtypen för vilken vyn kan visas. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Hämtar ett filter som används i en enskild vy.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Hämtar en grupp av den enkla vyn.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Hämtar ett värde som indikerar om Microsoft Project markerar filtret för en enkel vy.

**Returns:**
boolean - ett värde som indikerar om Microsoft Project markerar filtret för en enkel vy.
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på ett View-objekt.

**Returns:**
java.lang.String - namnet på ett View-objekt.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Hämtar en instans av `PageInfo`([getPageInfo()](../../com.aspose/tasks/view\#getPageInfo--))-klassen. Representerar sidinställningsdata som finns i mpp‑filformat.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldern till View-objektet. Skrivskyddad [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Hämtar skärmtypen för den enskilda vyn. Skrivskyddad [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - skärmtypen för den enskilda vyn.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Hämtar ett värde som indikerar om Microsoft Project visar namnet på den enkla vyn i View eller Other Views‑rullgardinslistorna i Ribbon.

**Returns:**
boolean - ett värde som indikerar om Microsoft Project visar den enskilda vy-namnet i View- eller Other Views-rullgardinslistorna i Ribbon.
### getTable() {#getTable--}
```
public final Table getTable()
```


Hämtar en tabell för den enkla vyn.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Hämtar typen av objekt i den enskilda vyn, såsom uppgifter eller resurser. Skrivskyddad [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - typen av objekt i den enskilda vyn, såsom uppgifter eller resurser.
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar den unika identifieraren för en vy.

**Returns:**
int - den unika identifieraren för en vy.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Hämtar en samling av objekt som representerar placering och utseende av [OleObject](../../com.aspose/tasks/oleobject) i vyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - en samling av objekt som representerar placering och utseende för [OleObject](../../com.aspose.tasks/oleobject) i vyn.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av klassen [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Den första vyn. |
| b | [View](../../com.aspose.tasks/view) | Den andra vyn. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är lika med ett specificerat objekt
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Returnerar ett värde som anger om detta objekt är större än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Den första vyn. |
| b | [View](../../com.aspose.tasks/view) | Den andra vyn. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än ett specificerat objekt
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Returnerar ett värde som anger om detta objekt är större än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Den första vyn. |
| b | [View](../../com.aspose.tasks/view) | Den andra vyn. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är större än eller lika med ett specificerat objekt
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Returnerar ett värde som anger om detta objekt inte är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Den första vyn. |
| b | [View](../../com.aspose.tasks/view) | Den andra vyn. |

**Returns:**
boolean - ett värde som indikerar om detta objekt inte är lika med ett specificerat objekt
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Returnerar ett värde som anger om detta objekt är mindre än ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Det första filtret. |
| b | [View](../../com.aspose.tasks/view) | Det andra filtret. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än ett specificerat objekt
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Returnerar ett värde som anger om detta objekt är mindre än eller lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Den första vyn. |
| b | [View](../../com.aspose.tasks/view) | Den andra vyn. |

**Returns:**
boolean - ett värde som indikerar om detta objekt är mindre än eller lika med ett specificerat objekt
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Ställer in ett filter som används i en enkel vy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | ett filter som används i en enskild vy. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Ställer in en grupp för den enkla vyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | en grupp av den enskilda vyn. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Ställer in ett värde som indikerar om Microsoft Project markerar filtret för en enkel vy.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Microsoft Project markerar filtret för en enskild vy. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ställer in namnet på ett View-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namnet på ett View-objekt. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Ställer in ett värde som indikerar om Microsoft Project visar namnet på den enkla vyn i View eller Other Views‑rullgardinslistorna i Ribbon.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Microsoft Project visar namnet på den enskilda vyn i View- eller Other Views-rullgardinslistorna i Ribbon. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Ställer in en tabell för den enkla vyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | en tabell för den enskilda vyn. |

