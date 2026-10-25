---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор GraphicalIndicatorCriteria. Инициализирует новый экземпляр типа GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /ru/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Инициализирует новый экземпляр типа [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | значение перечисления [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/), которое указывает, для каких строк применяется индикатор |
| test | FilterComparisonType | значение [`FilterComparisonType`](../../filtercomparisontype/), обозначающее тип сравнения, выполняемого критериями. |
| imageIndex | Int32 | индекс изображения, которое будет отображаться, когда поле соответствует критерию |
| value1 | GraphicalIndicatorCriteriaValue | значения, используемые при проверке условия. |
| value2 | GraphicalIndicatorCriteriaValue | второе значение (конец интервала), используемое при проверке условия в случае условий 'IsWithin' и 'IsNotWithing'. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Выбрасывается, когда в конструктор передаётся некорректная комбинация аргументов. |

### См. также

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Инициализирует новый экземпляр типа [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | значение перечисления [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/), которое указывает, для каких строк применяется индикатор |
| test | FilterComparisonType | значение [`FilterComparisonType`](../../filtercomparisontype/), обозначающее тип сравнения, выполняемого критериями. |
| imageIndex | Int32 | индекс изображения, которое будет отображаться, когда поле соответствует критерию |
| value | GraphicalIndicatorCriteriaValue | значение, используемое при проверке условия. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Выбрасывается, когда в конструктор передаётся некорректная комбинация аргументов. |
| ArgumentException | Когда значение IsWithin или IsNotWithing передаётся в тестовый аргумент. |

### См. также

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


