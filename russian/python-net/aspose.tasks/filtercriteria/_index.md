---
title: "FilterCriteria"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 350
url: /ru/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Определяет критерии, которым задачи или ресурсы должны соответствовать, чтобы отображаться в представлении MSP.

Тип FilterCriteria раскрывает следующие члены:
## Конструкторы
| Имя | Описание |
| :- | :- |
| FilterCriteria() | Инициализирует новый экземпляр класса FilterCriteria |
## Свойства
| Имя | Описание |
| :- | :- |
| операция | Получает или задает критерий, установленный с FieldName, Test и Value, относящийся к другим критериям в фильтре. |
| field | Получает или задает [field](/tasks/python-net/aspose.tasks/filtercriteria/) для изменения. |
| test | Получает или задает тип сравнения, выполненного между FieldName и Value, который служит критерием выбора для фильтра.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Получает объектные значения для сравнения со значением поля, указанного с помощью FieldName. |
| criteria_rows | Получает список дочерних строк [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/).<br/>            Если фильтр содержит более одной строки критерия, то эффект оператора And заключается в том, что критерии обеих строк должны быть выполнены, чтобы задача или ресурс отобразились в результате этого фильтра.<br/>            Эффект оператора Or заключается в том, что критерий одной из строк должен быть выполнен. |
## Методы
| Имя | Описание |
| :- | :- |
| is_field_value() | Получает, является ли правое значение FilterCriteria ссылкой на поле, а не константным значением. |
| set_value_field(value) | Задает поле, значение которого будет сравниваться со значением поля, указанного с помощью FieldName. |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

