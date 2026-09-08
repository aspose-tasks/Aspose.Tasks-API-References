---
title: "Baseline 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Baseline 클래스. 리소스의 기준값을 나타냅니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/baseline/
---
## Baseline class

리소스의 기준값을 나타냅니다.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Baseline](baseline/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | 베이스라인 데이터 레코드의 고유 번호를 가져오거나 설정합니다. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | 프로젝트에 대해 리소스가 수행한 작업의 현재까지 예산 비용을 가져오거나 설정합니다. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | 리소스에 예약된 작업의 예산 비용을 가져오거나 설정합니다. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | 베이스라인이 저장될 때 리소스의 예상 비용을 가져오거나 설정합니다. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | 베이스라인이 저장될 때 리소스에 할당된 작업을 가져오거나 설정합니다. 베이스라인이 저장될 때 리소스에 할당된 작업량입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable 인터페이스 구현입니다. 이 인스턴스를 지정된 Baseline 객체와 비교합니다. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | 기준값에 대한 해시 코드 값을 반환합니다. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


