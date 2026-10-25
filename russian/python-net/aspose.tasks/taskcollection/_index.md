---
title: "TaskCollection"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 1140
url: /ru/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

Представляет коллекцию объектов [Task](/tasks/python-net/aspose.tasks/task/).

Тип TaskCollection раскрывает следующие члены:
## Свойства
| Имя | Описание |
| :- | :- |
| parent_project | Получает родительский проект объекта TaskCollection. |
## Методы
| Имя | Описание |
| :- | :- |
| add() | Добавьте указанную задачу в экземпляр класса [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/).<br/>            Если ParentProject.CalculationMode имеет значение None, пользователь должен вызвать Project.Recalculate() после использования этого метода (это перенесёт расписание всех задач проекта (даты начала/окончания, устанавливает ранние/поздние даты) и вычислит зависимые поля, такие как запасы времени, трудозатраты и поля стоимости, идентификаторы и уровни структуры).<br/>            Если ParentProject.CalculationMode имеет значение Manual, метод вычислит только идентификатор задачи, уровень структуры и номера структуры автоматически.<br/>            Если ParentProject.CalculationMode имеет значение Automatic, метод автоматически перенесёт расписание всех задач проекта<br/>            (даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, трудозатраты и поля стоимости, пересчитывает  идентификаторы и уровни структуры). |
| add(task_name) | Добавляет новую задачу в коллекцию дочерних задач. |
| add(task_name, before_task_id) |  |
| add(parameters) | Вставляет новую задачу перед задачей с указанным идентификатором и на том же уровне структуры. |
| to_list() | Преобразует объект TaskCollection в список объектов [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | Возвращает задачу с указанным Uid, чей предок является родительской задачей этой коллекции . |
| get_by_id(id) | Возвращает задачу с указанным Id, чей предок является родительской задачей этой коллекции . |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

