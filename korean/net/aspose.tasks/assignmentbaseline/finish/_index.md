---
title: "AssignmentBaseline.Finish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentBaseline 속성. 기준선이 저장될 때 리소스 할당의 예정 종료 날짜를 가져오거나 설정합니다. 이 기준선이 저장될 때 리소스 할당의 종료 날짜."
type: docs
weight: 20
url: /ko/net/aspose.tasks/assignmentbaseline/finish/
---
## AssignmentBaseline.Finish property

베이스라인이 저장될 때 리소스 할당의 예정 종료 날짜를 가져오거나 설정합니다. 이 베이스라인이 저장될 때 리소스 할당의 종료 날짜입니다.

```csharp
public DateTime? Finish { get; set; }
```

## 예제

할당의 베이스라인을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// 전체 프로젝트에 베이스라인을 설정하면 할당 베이스라인이 설정됩니다.
project.SetBaseline(BaselineType.Baseline);

// 할당 베이스라인 정보를 읽습니다.
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

// 베이스라인 동일성을 확인합니다.
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// 베이스라인은 'Equals' 메서드 오버로드를 사용하여 비교할 수 있습니다.
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// 또는 오버로드된 산술 연산을 사용합니다.
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// 베이스라인 해시코드는 베이스라인 번호를 기반으로 합니다.
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### 또 보기

* class [AssignmentBaseline](../)
* namespace [Aspose.Tasks](../../assignmentbaseline/)
* assembly [Aspose.Tasks](../../../)


