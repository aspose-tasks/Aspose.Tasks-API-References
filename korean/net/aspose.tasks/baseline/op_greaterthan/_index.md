---
title: "Baseline.op_GreaterThan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Baseline 메서드. 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/baseline/op_greaterthan/
---
## Baseline GreaterThan operator

이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다.

```csharp
public static bool operator >(Baseline a, Baseline b)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | Baseline | 첫 번째 기준선입니다. |
| b | Baseline | 두 번째 기준선입니다. |

### 반환 값

이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값

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

* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


