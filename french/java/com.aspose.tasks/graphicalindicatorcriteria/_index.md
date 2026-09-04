---
title: "GraphicalIndicatorCriteria"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un critère d'indicateur graphique associé à un attribut étendu."
type: docs
weight: 115
url: /fr/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Représente un critère d'indicateur graphique associé à un attribut étendu.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialise une nouvelle instance du type [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initialise une nouvelle instance du type [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Obtient l'index de l'image à afficher lorsque le champ satisfait les critères. |
| [getRowType()](#getRowType--) | Obtient la valeur de l'énumération [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) qui indique pour quelles lignes l'indicateur est appliqué. |
| [getTest()](#getTest--) | Obtient le type de comparaison effectué entre la valeur de l'attribut étendu et les Valeurs qui servent de critère pour l'application de l'indicateur graphique. |
| [getValue1()](#getValue1--) | Obtient la valeur utilisée pour tester la valeur de l'attribut étendu. |
| [getValue2()](#getValue2--) | Obtient la deuxième valeur utilisée pour tester la valeur de l'attribut étendu dans le cas des types de comparaison 'IsWithin' et 'IsNotWithin'. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne de l'instance de la classe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Initialise une nouvelle instance du type [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowType | int | valeur de l'énumération [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) qui indique pour quelles lignes l'indicateur est appliqué |
| test | int | valeur de [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) indiquant le type de comparaison effectué par le critère. |
| imageIndex | int | l'index de l'image à afficher lorsque le champ satisfait les critères |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valeurs utilisées dans la vérification de condition. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | deuxième valeur (fin d'intervalle) utilisée dans la vérification de condition dans le cas des conditions 'IsWithin' et 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Initialise une nouvelle instance du type [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowType | int | valeur de l'énumération [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) qui indique pour quelles lignes l'indicateur est appliqué |
| test | int | valeur de [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) indiquant le type de comparaison effectué par le critère. |
| imageIndex | int | l'index de l'image à afficher lorsque le champ satisfait les critères |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valeur utilisée dans la vérification de condition. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Obtient l'index de l'image à afficher lorsque le champ satisfait les critères.

**Returns:**
int - l'index de l'image à afficher lorsque le champ satisfait les critères.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Obtient la valeur de l'énumération [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) qui indique pour quelles lignes l'indicateur est appliqué.

**Returns:**
int - la valeur de l'énumération [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) qui indique pour quelles lignes l'indicateur est appliqué.
### getTest() {#getTest--}
```
public final int getTest()
```


Obtient le type de comparaison effectué entre la valeur de l'attribut étendu et les Valeurs qui servent de critère pour l'application de l'indicateur graphique. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - le type de comparaison effectué entre la valeur de l'attribut étendu et les Valeurs qui servent de critère pour l'application de l'indicateur graphique.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Obtient la valeur utilisée pour tester la valeur de l'attribut étendu.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Obtient la deuxième valeur utilisée pour tester la valeur de l'attribut étendu dans le cas des types de comparaison 'IsWithin' et 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Renvoie la représentation sous forme de chaîne de l'instance de la classe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - représentation sous forme de chaîne de cet objet.
