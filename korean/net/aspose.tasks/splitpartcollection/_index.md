---
title: "SplitPartCollection 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.SplitPartCollection 클래스. 작업의 부분을 나타내는 컬렉션입니다."
type: docs
weight: 2300
url: /ko/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

작업의 부분을 나타내는 컬렉션입니다.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | 컬렉션에 있는 부분 수를 가져옵니다. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | 주어진 인덱스에서 작업의 분할 부분을 검색합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | 컬렉션의 모든 부분을 새 배열로 복사합니다. |

## 예제

분할 부분 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// 분할 부분을 반복합니다
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// 인덱스로 부분을 가져옵니다
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// 작업의 첫 번째 분할 부분을 사용하여 작업을 수행합니다
```

### 또 보기

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


