---
title: "Filter"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un filtre dans Project."
type: docs
weight: 91
url: /fr/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Représente un filtre dans Project.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Filter()](#Filter--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Compare cette instance à l'instance spécifiée de la classe [Filter](../../com.aspose.tasks/filter) et renvoie une indication de leur ordre relatif. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié. |
| [getCriteria()](#getCriteria--) | Obtient les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP. |
| [getFilterType()](#getFilterType--) | Obtient le type du filtre. |
| [getIndex()](#getIndex--) | Obtient l'index d'un objet [Filter](../../com.aspose.tasks/filter) dans l'objet contenant les filtres. |
| [getName()](#getName--) | Obtient le nom d'un objet Filter. |
| [getShowInMenu()](#getShowInMenu--) | Obtient une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filter sous l'onglet Affichage du ruban. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Obtient une valeur indiquant si les lignes de résumé associées sont affichées pour le filtre. |
| [getUid()](#getUid--) | Obtient l'identifiant unique d'un filtre. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour le filtre. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichées dans la vue MSP. |
| [setFilterType(int value)](#setFilterType-int-) | Le type du filtre. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom d'un objet Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Définit une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filter sous l'onglet Affichage du ruban. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Définit une valeur indiquant si les lignes de résumé associées sont affichées pour le filtre. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Compare cette instance à l'instance spécifiée de la classe [Filter](../../com.aspose.tasks/filter) et renvoie une indication de leur ordre relatif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | l'instance spécifiée de la classe [Filter](../../com.aspose.tasks/filter) à comparer à cet objet. |

**Returns:**
int - une indication de leur ordre relatif.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

**Returns:**
boolean - renvoie true si cette instance est égale à l'objet AssignmentBaseline spécifié ; sinon, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

**Returns:**
boolean - renvoie true si cette instance est égale à l'objet AssignmentBaseline spécifié ; sinon, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Obtient les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Obtient le type du filtre.

**Returns:**
int - le type du filtre.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtient l'index d'un objet [Filter](../../com.aspose.tasks/filter) dans l'objet contenant les filtres.

**Returns:**
int - l'index d'un objet [Filter](../../com.aspose.tasks/filter) dans l'objet contenant les filtres.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom d'un objet Filter.

**Returns:**
java.lang.String - le nom d'un objet Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Obtient une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filter sous l'onglet Affichage du ruban.

**Returns:**
booléen - une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filtre de l'onglet Affichage du ruban.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Obtient une valeur indiquant si les lignes de résumé associées sont affichées pour le filtre.

**Returns:**
booléen - une valeur indiquant si les lignes de synthèse associées sont affichées pour le filtre.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtient l'identifiant unique d'un filtre.

**Returns:**
int - l'identifiant unique d'un filtre.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour le filtre.

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est égale à un objet spécifié
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure à un objet spécifié
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance n'est pas égale à un objet spécifié
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure à un objet spécifié
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Le premier filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | Le deuxième filtre. |

**Returns:**
booléen - une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichées dans la vue MSP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Le type du filtre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type du filtre. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Définit le nom d'un objet Filter.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom d'un objet Filtre. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Définit une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filter sous l'onglet Affichage du ruban.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filtre de l'onglet Affichage du ruban. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Définit une valeur indiquant si les lignes de résumé associées sont affichées pour le filtre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les lignes de synthèse associées sont affichées pour le filtre. |

