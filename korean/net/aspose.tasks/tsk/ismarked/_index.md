---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 추가 작업을 위해 표시되었는지 또는 어떤 종류의 식별을 위해 표시되었는지를 보여줍니다"
type: docs
weight: 620
url: /ko/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

작업이 추가 작업이나 특정 식별을 위해 표시되었는지 여부를 보여줍니다.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## 비고

mpp 파일 형식에만 적용됩니다.

## 예제

Shows how to read/write Tsk.IsMarked property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


