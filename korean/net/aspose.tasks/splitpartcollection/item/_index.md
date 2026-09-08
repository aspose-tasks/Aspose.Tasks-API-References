---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SplitPartCollection 속성. 지정된 인덱스에서 작업의 분할 부분을 검색합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

주어진 인덱스에서 작업의 분할 부분을 검색합니다.

```csharp
public SplitPart this[int index] { get; set; }
```

| 매개변수 | 설명 |
| --- | --- |
| 인덱스 | 부분 인덱스. |

### 반환 값

분할 부분.

## 비고

인덱스는 0부터 시작합니다. 인덱스가 배열 범위를 벗어나면 null을 반환합니다.

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


