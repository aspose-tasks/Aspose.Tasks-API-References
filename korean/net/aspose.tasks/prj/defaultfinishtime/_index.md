---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj field. 새 작업의 기본 종료 시간"
type: docs
weight: 230
url: /ko/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

새 작업의 기본 종료 시간.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## 예제

Prj.DefaultFinishTime 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


