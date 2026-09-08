---
title: "AssignmentBaseline.Finish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство AssignmentBaseline. Получает или задает запланированную дату завершения назначения ресурса, когда базовая линия была сохранена. Дата завершения назначения ресурса, когда эта базовая линия была сохранена."
type: docs
weight: 20
url: /ru/net/aspose.tasks/assignmentbaseline/finish/
---
## AssignmentBaseline.Finish property

Получает или задает запланированную дату завершения назначения ресурса при сохранении базовой линии. Дата завершения назначения ресурса при сохранении этой базовой линии.

```csharp
public DateTime? Finish { get; set; }
```

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

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


