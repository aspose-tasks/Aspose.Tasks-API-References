---
title: Class FilterCriteria
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.FilterCriteria сорт. Определяет критерии которым должны соответствовать задачи или ресурсы для отображения в представлении MSP.
type: docs
weight: 630
url: /ru/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Определяет критерии, которым должны соответствовать задачи или ресурсы для отображения в представлении MSP.

```csharp
public class FilterCriteria
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Получает список дочерних`FilterCriteria` rows. Если фильтр содержит более одной строки критерия, то эффект оператора И заключается в том, что критерии для обеих строк должны быть соблюдены, чтобы задача или ресурс отображались в результате этого фильтра. Эффект оператора Или заключается в том, что критерии для той или иной строки должны быть соблюдены. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Получает или задает[`Field`](./field/) изменить. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Получает или задает критерий, установленный с помощью FieldName, Test и Value, связанный с другими критериями в фильтре. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Получает или задает тип сравнения между FieldName и Value, который действует как критерий выбора для фильтра. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Получает значения объекта для сравнения со значением поля, указанного с помощью FieldName. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Возвращает строковое представление экземпляра`FilterCriteria` класс. |

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


