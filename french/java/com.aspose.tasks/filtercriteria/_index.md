---
title: "FilterCriteria"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP."
type: docs
weight: 94
url: /fr/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Obtient la liste des lignes enfants [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
| [getField()](#getField--) | Obtient un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier. |
| [getOperation()](#getOperation--) | Obtient le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre. |
| [getTest()](#getTest--) | Obtient le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. |
| [getValues()](#getValues--) | Obtient les valeurs d'objet à comparer avec la valeur du champ spécifié par FieldName. |
| [isValueAField()](#isValueAField--) | Obtient si la valeur à droite de FilterCriteria est une référence de champ, et non une valeur constante. |
| [isValueAField(int index)](#isValueAField-int-) | Obtient si la valeur à l'index de FilterCriteria est une référence de champ, et non une valeur constante. |
| [setField(int value)](#setField-int-) | Définit un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier. |
| [setOperation(int value)](#setOperation-int-) | Définit le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre. |
| [setTest(int value)](#setTest-int-) | Définit le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Définit la valeur d'objet à l'index pour la comparer avec la valeur du champ spécifié par FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit la valeur d'objet à comparer avec la valeur du champ spécifié par FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Définit le champ dont la valeur sera comparée à la valeur du champ spécifié par FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Définit le champ à l'index dont la valeur sera comparée à la valeur du champ spécifié par FieldName. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne de l'instance de la classe [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Obtient la liste des lignes enfants [FilterCriteria](../../com.aspose.tasks/filtercriteria). Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur And est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource soit affichée en résultat de ce filtre. L'effet d'un opérateur Or est que les critères d'une ou l'autre ligne doivent être remplis.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - la liste des lignes enfants [FilterCriteria](../../com.aspose.tasks/filtercriteria).
### getField() {#getField--}
```
public final int getField()
```


Obtient un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier.

**Returns:**
int - un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Obtient le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre.

**Returns:**
int - le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre.
### getTest() {#getTest--}
```
public final int getTest()
```


Obtient le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Obtient les valeurs d'objet à comparer avec la valeur du champ spécifié par FieldName.

**Returns:**
java.lang.Object[] - les valeurs d'objet à comparer avec la valeur du champ spécifié par FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Obtient si la valeur à droite de FilterCriteria est une référence de champ, et non une valeur constante.

**Returns:**
boolean - indique si la valeur à droite de FilterCriteria est une référence de champ, et non une valeur constante.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Obtient si la valeur à l'index de FilterCriteria est une référence de champ, et non une valeur constante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | l'index de la valeur |

**Returns:**
booléen - indique si la valeur à droite à l'index de FilterCriteria est une référence de champ, et non une valeur constante.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Définit un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | un `Field`([getField()](../../com.aspose/tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) à modifier. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Définit le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le critère établi avec FieldName, Test et Value se rapporte aux autres critères du filtre. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Définit le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Définit la valeur d'objet à l'index pour la comparer avec la valeur du champ spécifié par FieldName.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | l'index de la valeur. |
| valeur | java.lang.Object | valeur d'objet qui servira de valeur à droite à l'index du critère de filtre. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Définit la valeur d'objet à comparer avec la valeur du champ spécifié par FieldName.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | valeur d'objet qui servira de valeur à droite du critère de filtre. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Définit le champ dont la valeur sera comparée à la valeur du champ spécifié par FieldName.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | Champ qui servira de valeur à droite du critère de filtre. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Définit le champ à l'index dont la valeur sera comparée à la valeur du champ spécifié par FieldName.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | l'index de la valeur |
| valeur | int | Champ qui servira de valeur à droite à l'index du critère de filtre. |

### toString() {#toString--}
```
public String toString()
```


Renvoie la représentation sous forme de chaîne de l'instance de la classe [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - représentation sous forme de chaîne de cet objet.
