---
title: "PrimaveraProjectProperties"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 760
url: /ru/python-net/aspose.tasks/primaveraprojectproperties/
---

## PrimaveraProjectProperties class

Представляет специфичные для Primavera свойства проекта, считанного из файлов Primavera (XER или P6XML).

Тип PrimaveraProjectProperties раскрывает следующие члены:
## Свойства
| Имя | Описание |
| :- | :- |
| relationship_lag_calendar | Получает параметр, определяющий, какой календарь использовать для планирования задержки отношений в проектах Primavera |
| use_expected_finish_dates | Получает флаг, определяющий, следует ли планировать даты завершения активности как ожидаемые даты завершения. |
| make_open_ended_activities_critical | Получает флаг, определяющий, следует ли помечать активности как критические при планировании проекта. |
| ignore_other_project_relationships | Получает флаг, определяющий, следует ли игнорировать взаимосвязи активностей между проектами. |
| current_baseline_project_id | Получает Id текущего базового проекта.<br/>            Применяется к проектам, считанным из файлов Primavera XML, содержащих экспортированные базовые линии. |
| baseline_projects | Получает массив базовых проектов текущего проекта.<br/>            Применяется к проектам, считанным из файлов Primavera XML, содержащих экспортированные базовые линии. |
| critical_activities_defining_method | Получает метод определения критических задач: Longest Path или Total Float. |
| critical_total_float_limit | Получает пороговое значение, используемое для определения критических задач, если используется метод TotalFloat. |
| short_name | Получает короткое название проекта (Project ID). |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

