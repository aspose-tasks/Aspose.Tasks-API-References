---
title: "Класс AssignmentBaseline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.AssignmentBaseline. Представляет базовую линию назначения ресурса."
type: docs
weight: 50
url: /ru/net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Представает базовую линию назначения ресурса.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Получает или задает уникальный номер записи данных базовой линии. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Получает или задает запланированную стоимость работы, выполненной ресурсом для проекта на текущую дату. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Получает или задает бюджетную стоимость запланированной работы для ресурса. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Получает или задает прогнозируемую стоимость ресурса при сохранении базовой линии. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Получает или задает запланированную дату завершения назначения ресурса при сохранении базовой линии. Дата завершения назначения ресурса при сохранении этой базовой линии. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Получает или задает запланированную дату начала назначения ресурса при сохранении базовой линии. Дата начала назначения ресурса при сохранении этой базовой линии. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Получает или задает экземпляр [`TimephasedDataCollection`](../timephaseddatacollection/) для этого объекта. Временные данные, связанные с базовой линией назначения ресурса. Возвращает экземпляр [`TimephasedDataCollection`](../timephaseddatacollection/) для этого объекта. Коллекция временных данных, связанных с этой базовой линией. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Получает или задает работу, назначенную ресурсу при сохранении базовой линии. Объём назначенной работы ресурсу при сохранении базовой линии. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | Реализация интерфейса IComparable. Сравнивает этот экземпляр с указанным объектом Baseline. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Реализация интерфейса IComparable. Сравнивает этот экземпляр с указанным объектом Baseline. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту AssignmentBaseline. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

## Примеры

Показывает, как работать с базовыми линиями назначений.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Базовые линии назначений устанавливаются, когда задаётся базовая линия для всего проекта.
project.SetBaseline(BaselineType.Baseline);

// читать информацию о базовой линии назначения
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// проверить равенство базовых линий
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// базовые линии можно сравнивать, используя перегрузки метода 'Equals'
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// или используя перегруженную арифметическую операцию
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// хеш-код базовой линии основан на её номере
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### См. также

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


