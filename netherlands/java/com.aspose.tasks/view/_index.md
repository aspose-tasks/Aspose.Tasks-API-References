---
title: "View"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een weergave in Project voor."
type: docs
weight: 342
url: /nl/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Stelt een weergave in Project voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [View()](#View--) | Initialiseert een nieuwe instantie van de [View](../../com.aspose/tasks/view) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Vergelijkt de huidige instantie met een ander object van hetzelfde type en retourneert een integer die aangeeft of de huidige instantie voorafgaat, volgt of zich op dezelfde positie in de sorteervolgorde bevindt als het andere object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Construeert een nieuwe instantie van de [View](../../com.aspose/tasks/view) klasse. |
| [getFilter()](#getFilter--) | Haalt een filter op dat wordt gebruikt in een enkele view. |
| [getGroup()](#getGroup--) | Haalt een groep van de enkele view op. |
| [getHighlightFilter()](#getHighlightFilter--) | Haalt een waarde op die aangeeft of Microsoft Project het filter voor een enkele view markeert. |
| [getName()](#getName--) | Haalt de naam op van een View-object. |
| [getPageInfo()](#getPageInfo--) | Haalt een instantie op van de `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) klasse. |
| [getParentProject()](#getParentProject--) | Haalt de ouder op van het View-object. |
| [getScreen()](#getScreen--) | Haalt het schermtype op voor de enkele view. |
| [getShowInMenu()](#getShowInMenu--) | Haalt een waarde op die aangeeft of Microsoft Project de naam van de enkele view weergeeft in de View- of de Other Views-keuzelijsten in het lint. |
| [getTable()](#getTable--) | Haalt een tabel op van de enkele view. |
| [getType()](#getType--) | Haalt het type item op in de enkele weergave, zoals taken of resources. |
| [getUid()](#getUid--) | Haalt de unieke identifier op van een weergave. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Haalt een collectie objecten op die de plaatsing en weergave van [OleObject](../../com.aspose.tasks/oleobject) in de weergave vertegenwoordigen. |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor de instantie van de [Resource](../../com.aspose.tasks/resource) klasse. |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Stelt een filter in dat wordt gebruikt in een enkele weergave. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Stelt een groep in voor de enkele weergave. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Stelt een waarde in die aangeeft of Microsoft Project het filter markeert voor een enkele weergave. |
| [setName(String value)](#setName-java.lang.String-) | Stelt de naam in van een View-object. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Stelt een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Other Views‑keuzelijsten in het Ribbon. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Stelt een tabel in voor de enkele weergave. |
### View() {#View--}
```
public View()
```


Initialiseert een nieuwe instantie van de [View](../../com.aspose/tasks/view) klasse.

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Vergelijkt de huidige instantie met een ander object van hetzelfde type en retourneert een integer die aangeeft of de huidige instantie voorafgaat, volgt of zich op dezelfde positie in de sorteervolgorde bevindt als het andere object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | het opgegeven View-object om deze instantie mee te vergelijken. |

**Returns:**
int - Een 32-bits ondertekend geheel getal dat de relatieve volgorde van de te vergelijken objecten aangeeft. De retourwaarde heeft de volgende betekenissen: Waarde Betekenis Minder dan nul Deze instantie komt vóór `other` in de sorteervolgorde. Nul Deze instantie bevindt zich op dezelfde positie in de sorteervolgorde als `other`. Meer dan nul Deze instantie komt na `other` in de sorteervolgorde.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als het opgegeven object een View is die dezelfde Uid-waarde heeft als deze instantie; anders, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Construeert een nieuwe instantie van de [View](../../com.aspose/tasks/view) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| viewScreen | int | Het schermtype waarvoor de weergave kan worden weergegeven. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Haalt een filter op dat wordt gebruikt in een enkele view.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Haalt een groep van de enkele view op.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Haalt een waarde op die aangeeft of Microsoft Project het filter voor een enkele view markeert.

**Returns:**
boolean - een waarde die aangeeft of Microsoft Project het filter markeert voor een enkele weergave.
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam op van een View-object.

**Returns:**
java.lang.String - de naam van een View-object.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Haalt een instantie op van de `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) klasse. Vertegenwoordigt paginainstellingsgegevens die aanwezig zijn in het mpp-bestandsformaat.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt de ouder op van het View-object. Alleen-lezen [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Haalt het schermtype op voor de enkele weergave. Alleen-lezen [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - het schermtype voor de enkele weergave.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Haalt een waarde op die aangeeft of Microsoft Project de naam van de enkele view weergeeft in de View- of de Other Views-keuzelijsten in het lint.

**Returns:**
boolean - een waarde die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Other Views‑keuzelijsten in het Ribbon.
### getTable() {#getTable--}
```
public final Table getTable()
```


Haalt een tabel op van de enkele view.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Haalt het type item op in de enkele weergave, zoals taken of resources. Alleen-lezen [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - het type item in de enkele weergave, zoals taken of resources.
### getUid() {#getUid--}
```
public final int getUid()
```


Haalt de unieke identifier op van een weergave.

**Returns:**
int - de unieke identifier van een weergave.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Haalt een collectie objecten op die de plaatsing en weergave van [OleObject](../../com.aspose.tasks/oleobject) in de weergave vertegenwoordigen.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - een collectie objecten die de plaatsing en weergave van [OleObject](../../com.aspose.tasks/oleobject) in de weergave vertegenwoordigen.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor de instantie van de [Resource](../../com.aspose.tasks/resource) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | De eerste weergave. |
| b | [View](../../com.aspose.tasks/view) | De tweede weergave. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | De eerste weergave. |
| b | [View](../../com.aspose.tasks/view) | De tweede weergave. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter is dan een opgegeven object
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | De eerste weergave. |
| b | [View](../../com.aspose.tasks/view) | De tweede weergave. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | De eerste weergave. |
| b | [View](../../com.aspose.tasks/view) | De tweede weergave. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Het eerste filter. |
| b | [View](../../com.aspose.tasks/view) | Het tweede filter. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | De eerste weergave. |
| b | [View](../../com.aspose.tasks/view) | De tweede weergave. |

**Returns:**
boolean - een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Stelt een filter in dat wordt gebruikt in een enkele weergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | een filter dat in een enkele weergave wordt gebruikt. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Stelt een groep in voor de enkele weergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | een groep van de enkele weergave. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Stelt een waarde in die aangeeft of Microsoft Project het filter markeert voor een enkele weergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Microsoft Project het filter voor een enkele weergave markeert. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Stelt de naam in van een View-object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de naam van een View-object. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Stelt een waarde in die aangeeft of Microsoft Project de naam van de enkele weergave toont in de View of de Other Views‑keuzelijsten in het Ribbon.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Microsoft Project de naam van de enkele weergave toont in de weergave- of de Andere weergaven‑keuzelijsten in het lint. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Stelt een tabel in voor de enkele weergave.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | een tabel van de enkele weergave. |

