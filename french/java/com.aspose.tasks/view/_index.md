---
title: "Vue"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une vue dans Project."
type: docs
weight: 342
url: /fr/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Représente une vue dans Project.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [View()](#View--) | Initialise une nouvelle instance de la classe [View](../../com.aspose/tasks/view). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Compare l'instance actuelle avec un autre objet du même type et renvoie un entier qui indique si l'instance actuelle précède, suit ou se trouve à la même position dans l'ordre de tri que l'autre objet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Construit une nouvelle instance de la classe [View](../../com.aspose/tasks/view). |
| [getFilter()](#getFilter--) | Obtient un filtre utilisé dans une vue unique. |
| [getGroup()](#getGroup--) | Obtient un groupe de la vue unique. |
| [getHighlightFilter()](#getHighlightFilter--) | Obtient une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique. |
| [getName()](#getName--) | Obtient le nom d'un objet View. |
| [getPageInfo()](#getPageInfo--) | Obtient une instance de la classe `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Obtient le parent de l'objet View. |
| [getScreen()](#getScreen--) | Obtient le type d'écran pour la vue unique. |
| [getShowInMenu()](#getShowInMenu--) | Obtient une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans la liste déroulante Vue ou Autres Vues du ruban. |
| [getTable()](#getTable--) | Obtient un tableau de la vue unique. |
| [getType()](#getType--) | Obtient le type d'élément dans la vue unique, tel que les tâches ou les ressources. |
| [getUid()](#getUid--) | Obtient l'identifiant unique d'une vue. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Obtient une collection d'objets représentant le placement et l'apparence de [OleObject](../../com.aspose.tasks/oleobject) dans la vue. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Définit un filtre utilisé dans une vue unique. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Définit un groupe de la vue unique. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Définit une valeur indiquant si Microsoft Project met en surbrillance le filtre pour une vue unique. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom d'un objet View. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Définit une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes View ou Other Views du ruban. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Définit une table de la vue unique. |
### View() {#View--}
```
public View()
```


Initialise une nouvelle instance de la classe [View](../../com.aspose/tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Compare l'instance actuelle avec un autre objet du même type et renvoie un entier qui indique si l'instance actuelle précède, suit ou se trouve à la même position dans l'ordre de tri que l'autre objet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | l'objet View spécifié avec lequel comparer cette instance. |

**Returns:**
int - Un entier signé de 32 bits qui indique l'ordre relatif des objets comparés. La valeur de retour a les significations suivantes : Valeur Signification Inférieure à zéro Cette instance précède `other` dans l'ordre de tri. Zéro Cette instance se trouve à la même position dans l'ordre de tri que `other`. Supérieure à zéro Cette instance suit `other` dans l'ordre de tri.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet à comparer avec cette instance. |

**Returns:**
boolean - **True** si l'objet spécifié est un View dont la valeur Uid est identique à celle de cette instance ; sinon, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Construit une nouvelle instance de la classe [View](../../com.aspose/tasks/view).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| viewScreen | int | Le type d'écran pour lequel la vue peut être affichée. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Obtient un filtre utilisé dans une vue unique.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Obtient un groupe de la vue unique.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Obtient une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique.

**Returns:**
boolean - une valeur indiquant si Microsoft Project met en surbrillance le filtre pour une vue unique.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom d'un objet View.

**Returns:**
java.lang.String - le nom d'un objet View.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Obtient une instance de la classe `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). Représente les données de mise en page présentes dans le format de fichier mpp.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le parent de l'objet View. Lecture seule [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Obtient le type d'écran pour la vue unique. Lecture seule [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - le type d'écran pour la vue unique.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Obtient une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans la liste déroulante Vue ou Autres Vues du ruban.

**Returns:**
boolean - une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes View ou Other Views du ruban.
### getTable() {#getTable--}
```
public final Table getTable()
```


Obtient un tableau de la vue unique.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Obtient le type d'élément dans la vue unique, tel que les tâches ou les ressources. Lecture seule [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - le type d'élément dans la vue unique, tel que les tâches ou les ressources.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtient l'identifiant unique d'une vue.

**Returns:**
int - l'identifiant unique d'une vue.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Obtient une collection d'objets représentant le placement et l'apparence de [OleObject](../../com.aspose.tasks/oleobject) dans la vue.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - une collection d'objets représentant le placement et l'apparence de [OleObject](../../com.aspose.tasks/oleobject) dans la vue.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La première vue. |
| b | [View](../../com.aspose.tasks/view) | La deuxième vue. |

**Returns:**
booléen - une valeur indiquant si cette instance est égale à un objet spécifié
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La première vue. |
| b | [View](../../com.aspose.tasks/view) | La deuxième vue. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure à un objet spécifié
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La première vue. |
| b | [View](../../com.aspose.tasks/view) | La deuxième vue. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La première vue. |
| b | [View](../../com.aspose.tasks/view) | La deuxième vue. |

**Returns:**
booléen - une valeur indiquant si cette instance n'est pas égale à un objet spécifié
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | Le premier filtre. |
| b | [View](../../com.aspose.tasks/view) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure à un objet spécifié
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La première vue. |
| b | [View](../../com.aspose.tasks/view) | La deuxième vue. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Définit un filtre utilisé dans une vue unique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | un filtre utilisé dans une vue unique. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Définit un groupe de la vue unique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | un groupe de la vue unique. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Définit une valeur indiquant si Microsoft Project met en surbrillance le filtre pour une vue unique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si Microsoft Project met en évidence le filtre pour une vue unique. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Définit le nom d'un objet View.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom d'un objet Vue. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Définit une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans les listes déroulantes View ou Other Views du ruban.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si Microsoft Project affiche le nom de la vue unique dans la liste déroulante Vue ou Autres vues du ruban. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Définit une table de la vue unique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | un tableau de la vue unique. |

