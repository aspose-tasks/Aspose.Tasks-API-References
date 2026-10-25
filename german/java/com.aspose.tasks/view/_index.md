---
title: "Ansicht"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Ansicht in Project dar."
type: docs
weight: 342
url: /de/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Stellt eine Ansicht in Project dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [View()](#View--) | Initialisiert eine neue Instanz der [View](../../com.aspose/tasks/view)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Vergleicht die aktuelle Instanz mit einem anderen Objekt desselben Typs und gibt einen Integer zurück, der angibt, ob die aktuelle Instanz dem anderen Objekt im Sortierreihenfolge vorausgeht, folgt oder an derselben Position im Sortierreihenfolge steht. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Konstruiert eine neue Instanz der [View](../../com.aspose/tasks/view)-Klasse. |
| [getFilter()](#getFilter--) | Ruft einen Filter ab, der in einer einzelnen Ansicht verwendet wird. |
| [getGroup()](#getGroup--) | Ruft eine Gruppe der einzelnen Ansicht ab. |
| [getHighlightFilter()](#getHighlightFilter--) | Ruft einen Wert ab, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt. |
| [getName()](#getName--) | Ruft den Namen eines View-Objekts ab. |
| [getPageInfo()](#getPageInfo--) | Ruft eine Instanz der `PageInfo`([getPageInfo()](../../com.aspose/tasks/view\#getPageInfo--))-Klasse ab. |
| [getParentProject()](#getParentProject--) | Ruft das übergeordnete Element des View-Objekts ab. |
| [getScreen()](#getScreen--) | Ruft den Bildschirmentyp für die einzelne Ansicht ab. |
| [getShowInMenu()](#getShowInMenu--) | Ruft einen Wert ab, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown-Listen 'Ansicht' oder 'Weitere Ansichten' im Ribbon anzeigt. |
| [getTable()](#getTable--) | Ruft eine Tabelle der einzelnen Ansicht ab. |
| [getType()](#getType--) | Ruft den Typ des Elements in der einzelnen Ansicht ab, z. B. Aufgaben oder Ressourcen. |
| [getUid()](#getUid--) | Ruft den eindeutigen Bezeichner einer Ansicht ab. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Ruft eine Sammlung von Objekten ab, die die Platzierung und das Erscheinungsbild von [OleObject](../../com.aspose/tasks/oleobject) in der Ansicht darstellen. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse zurück. |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Legt einen Filter fest, der in einer einzelnen Ansicht verwendet wird. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Legt eine Gruppe der einzelnen Ansicht fest. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Legt einen Wert fest, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen eines View-Objekts fest. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Legt einen Wert fest, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown-Listen 'Ansicht' oder 'Weitere Ansichten' im Ribbon anzeigt. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Legt eine Tabelle der einzelnen Ansicht fest. |
### View() {#View--}
```
public View()
```


Initialisiert eine neue Instanz der [View](../../com.aspose/tasks/view)-Klasse.

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Vergleicht die aktuelle Instanz mit einem anderen Objekt desselben Typs und gibt einen Integer zurück, der angibt, ob die aktuelle Instanz dem anderen Objekt im Sortierreihenfolge vorausgeht, folgt oder an derselben Position im Sortierreihenfolge steht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | das angegebene View-Objekt, mit dem diese Instanz verglichen wird. |

**Returns:**
int - Ein 32‑Bit‑vorzeichenbehafteter Integer, der die relative Reihenfolge der verglichenen Objekte angibt. Der Rückgabewert hat folgende Bedeutungen: Wert Bedeutung Weniger als Null Diese Instanz geht `other` in der Sortierreihenfolge voraus. Null Diese Instanz befindet sich an derselben Position in der Sortierreihenfolge wie `other`. Größer als Null Diese Instanz folgt `other` in der Sortierreihenfolge.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True** wenn das angegebene Objekt eine View ist, die denselben Uid-Wert wie diese Instanz hat; andernfalls **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Konstruiert eine neue Instanz der [View](../../com.aspose/tasks/view)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| viewScreen | int | Der Bildschirms‑Typ, für den die Ansicht angezeigt werden kann. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Ruft einen Filter ab, der in einer einzelnen Ansicht verwendet wird.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Ruft eine Gruppe der einzelnen Ansicht ab.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Ruft einen Wert ab, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt.

**Returns:**
boolean - ein Wert, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Namen eines View-Objekts ab.

**Returns:**
java.lang.String - der Name eines View-Objekts.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Ruft eine Instanz der `PageInfo`([getPageInfo()](../../com.aspose/tasks/view\#getPageInfo--))‑Klasse ab. Stellt Seiteneinrichtungsdaten dar, die im mpp-Dateiformat vorhanden sind.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ruft das übergeordnete Element des View-Objekts ab. Nur lesbar [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Ruft den Bildschirms‑Typ für die einzelne Ansicht ab. Nur lesbar [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - der Bildschirms‑Typ für die einzelne Ansicht.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Ruft einen Wert ab, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown-Listen 'Ansicht' oder 'Weitere Ansichten' im Ribbon anzeigt.

**Returns:**
boolean - ein Wert, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown‑Listen Ansicht oder Andere Ansichten im Ribbon anzeigt.
### getTable() {#getTable--}
```
public final Table getTable()
```


Ruft eine Tabelle der einzelnen Ansicht ab.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Ruft den Typ des Elements in der einzelnen Ansicht ab, z. B. Aufgaben oder Ressourcen. Nur lesbar [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - der Typ des Elements in der einzelnen Ansicht, z. B. Aufgaben oder Ressourcen.
### getUid() {#getUid--}
```
public final int getUid()
```


Ruft den eindeutigen Bezeichner einer Ansicht ab.

**Returns:**
int - der eindeutige Bezeichner einer Ansicht.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Ruft eine Sammlung von Objekten ab, die die Platzierung und das Erscheinungsbild von [OleObject](../../com.aspose/tasks/oleobject) in der Ansicht darstellen.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - eine Sammlung von Objekten, die Platzierung und Aussehen von [OleObject](../../com.aspose.tasks/oleobject) in der Ansicht darstellen.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Die erste Ansicht. |
| b | [View](../../com.aspose.tasks/view) | Die zweite Ansicht. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Die erste Ansicht. |
| b | [View](../../com.aspose.tasks/view) | Die zweite Ansicht. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer als ein angegebenes Objekt ist
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Die erste Ansicht. |
| b | [View](../../com.aspose.tasks/view) | Die zweite Ansicht. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz größer oder gleich einem angegebenen Objekt ist
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Die erste Ansicht. |
| b | [View](../../com.aspose.tasks/view) | Die zweite Ansicht. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz nicht gleich einem angegebenen Objekt ist
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Der erste Filter. |
| b | [View](../../com.aspose.tasks/view) | Der zweite Filter. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner als ein angegebenes Objekt ist
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Die erste Ansicht. |
| b | [View](../../com.aspose.tasks/view) | Die zweite Ansicht. |

**Returns:**
boolean - ein Wert, der angibt, ob diese Instanz kleiner oder gleich einem angegebenen Objekt ist
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Legt einen Filter fest, der in einer einzelnen Ansicht verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | ein Filter, der in einer einzelnen Ansicht verwendet wird. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Legt eine Gruppe der einzelnen Ansicht fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | eine Gruppe der einzelnen Ansicht. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Legt einen Wert fest, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Microsoft Project den Filter für eine einzelne Ansicht hervorhebt. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Legt den Namen eines View-Objekts fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Name eines View-Objekts. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Legt einen Wert fest, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown-Listen 'Ansicht' oder 'Weitere Ansichten' im Ribbon anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Microsoft Project den Namen der einzelnen Ansicht in den Dropdown‑Listen Ansicht oder Andere Ansichten im Ribbon anzeigt. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Legt eine Tabelle der einzelnen Ansicht fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | eine Tabelle der einzelnen Ansicht. |

