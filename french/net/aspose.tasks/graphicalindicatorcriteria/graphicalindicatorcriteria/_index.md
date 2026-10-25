---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur GraphicalIndicatorCriteria. Initialise une nouvelle instance du type GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /fr/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Initialise une nouvelle instance du type [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valeur de l'énumération [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) qui indique pour quelles lignes l'indicateur est appliqué |
| test | FilterComparisonType | valeur de [`FilterComparisonType`](../../filtercomparisontype/) indiquant le type de comparaison effectué par le critère. |
| imageIndex | Int32 | l'index de l'image à afficher lorsque le champ satisfait les critères |
| value1 | GraphicalIndicatorCriteriaValue | valeurs utilisées dans la vérification de condition. |
| value2 | GraphicalIndicatorCriteriaValue | deuxième valeur (fin d'intervalle) utilisée dans la vérification de condition dans le cas des conditions 'IsWithin' et 'IsNotWithing'. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancée lorsque une combinaison incorrecte d'arguments est passée au constructeur. |

### Voir aussi

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Initialise une nouvelle instance du type [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valeur de l'énumération [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) qui indique pour quelles lignes l'indicateur est appliqué |
| test | FilterComparisonType | valeur de [`FilterComparisonType`](../../filtercomparisontype/) indiquant le type de comparaison effectué par le critère. |
| imageIndex | Int32 | l'index de l'image à afficher lorsque le champ satisfait les critères |
| value | GraphicalIndicatorCriteriaValue | valeur utilisée dans la vérification de condition. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancée lorsque une combinaison incorrecte d'arguments est passée au constructeur. |
| ArgumentException | Lorsque la valeur de IsWithin ou IsNotWithing est passée à l'argument de test. |

### Voir aussi

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


