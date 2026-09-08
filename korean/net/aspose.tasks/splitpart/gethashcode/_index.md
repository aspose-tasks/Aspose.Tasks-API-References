---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SplitPart 메서드. SplitPart 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

[`SplitPart`](../) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

분할 부분의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// 먼저 리소스 할당 시간 단계 데이터를 생성해야 합니다.
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// 작업을 분할합니다.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// 분할 부분의 동일성은 시작, 종료 및 인덱스와 비교하여 확인됩니다.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// 분할 부분의 시작, 종료 및 인덱스를 기반으로 한 해시 코드입니다.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### 또 보기

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


