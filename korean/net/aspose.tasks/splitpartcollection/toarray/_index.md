---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SplitPartCollection 메서드. 컬렉션의 모든 파트를 새 배열로 복사합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

컬렉션의 모든 부분을 새 배열로 복사합니다.

```csharp
public SplitPart[] ToArray()
```

### 반환 값

[`SplitPart`](../../splitpart/) 객체들의 배열입니다.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


